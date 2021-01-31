# oddalecise-Dockerized

Последната домашна  задача беше да се рефакторира кодот и апликацијата да се подели на микросевиси кои ќе се контејнеризираат со помош на докер.

За делот на рефакторирање на кодот не искористивме нови дизајн патерни затоа што немаше каде да се имплементираат во веќе постоечкиот код,
доволно е чист и едноставен како што веќе е.

Во однос на микросервисите, имаме три микросервиси од кои што се состои нашата аплиакција
  1. Database (Mongo DB)
  2. Frontend (Angular 9)
  3. Backend (Node.js and Express)

За сите микросервиси користиме соодветни слики од `https://hub.docker.com/` за секоја од технологиите.
Тие како такви треба да се контејнеризираат поединечно и да функционираат автономно.
Откако ќе бидат контејнеризирани во docker-compose.yml фајлот навигираме да бидат интерконектирани и како таков тој фајл го deploynuvame(orchestraton).


Конкренто во овој репозиротиум oddalecise-Dockerized има линкови кон посебните сервиси, а самите сервиси имаат посебни репозитории и само се апдејтирани од
претходната домашна, во овој репозиториум целта е нивната оркестрација со docker-compose.

Во прилог се линкови од останатите засегнати репозиториуми.

https://github.com/StefanVelkoski/oddaleciseAPP-API
https://github.com/StefanVelkoski/oddaleciseAPP

