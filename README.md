# OddaleciSe

Инструкции за работа на цефката:


Користиме податоци од Google Maps кој преку third party software phantobuster.com бустер ја конвертира во csv фајл.

Како таков таа датотека е обемен и не ни треба целосно па затоа наишавме скрипта која што го филтрира тој csv фајл и додада филтер екстензија во името како би се знаело дека новата создадена датотека е исфилтиран, во него чуваме само информации кои што ни се потребни на нас за остварување на нашата замисла.

За да исфилтираме одиме до фолдерот каде што ни се наоѓаат нефилтрираните фајлови со податоци и ја пишуваме следната команда

    ./filter-script.sh planini.csv >> planiniFilter.csv | ./filter-script.sh ezera1.csv >> ezeraFilter.csv


Откако ќе ги исфилтираме податоците, спремни сме да ги искористиме.

Навигираме до датотеката каде што ни се наоѓа скриптата преку која што корисникот внесува податоци за да се поврзе со базата.

За тоа да го направиме потребна ни е база на податоци која ја направивме преку командна линија.

Ние користиме postgres, за да му работи корисникот треба да ја има симнато на својата машина.

    ./database.sh

Со извршување на скриптата корисникот треба да внесе неколку параметри име, хостиме, база, кои што се претходно дефинирани преку postgres cli.

Тие информации скриптата ги користи да ја започне postgres апликацијата(psql) и да навигира до датотеката database.sql која направи табели во базата соодветно
со исфилтираните податоци.



