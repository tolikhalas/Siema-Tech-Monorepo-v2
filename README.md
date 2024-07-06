# Siema Tech Monorepo :tada:

> <div style="display: flex; align-items: center;">
> <span>🔥 Powered with <a href="https://bun.sh/">Bun.js</a></span>
> <img style="margin-left: 5px;" width="24px" src="https://user-images.githubusercontent.com/709451/182802334-d9c42afe-f35d-4a7b-86ea-9985f73f20c3.png" alt="bun.js icon">
> </div>

---

<div style="display:grid; gap: 32px;">
<div style="width: 100%; margin: 0 8px; display: flex; justify-items: center; align-items: center; gap: 16px">
<img height="120px" src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a8/NestJS.svg/256px-NestJS.svg.png" alt="nest.js logo">
<p style="font-size: 36px">+</p>
<img style="margin-left: 5px;" height="120px" src="https://www.svgrepo.com/show/354113/nextjs-icon.svg" alt="bun.js icon">
<p style="font-size: 36px">+</p>
<img style="margin-left: 5px;" height="120px" src="https://static-00.iconduck.com/assets.00/lerna-icon-512x364-cdlzyj6z.png" alt="bun.js icon">
</div>

<div style="width: 100wv; margin: 0 115px; display: flex; justify-items: center align-items: center; gap: 16px; font-size: 18px;">
<p>🌿 Modern</p>
<p>🥇 Robust</p>
<p>🧘 Reliable</p>
</div>
</div>

<div style="display: grid; grid-template-columns: auto auto auto">
<p>✅ Distribute events</p>
<p>✅ Guarded data</p>
<p>✅ Efficient storage<p>
<p>✅ Caching response</p>
<p>✅ Modular features</p>
<p>✅ Realtime charts</p>
</div>

## Table of Contents :books:

- [Siema Tech Monorepo :tada:](#siema-tech-monorepo-tada)
  - [Table of Contents :books:](#table-of-contents-books)
  - [Description :writing_hand:](#description-writing_hand)
    - [Quick overview :eyes:](#quick-overview-eyes)
  - [Prerequires :building_construction:](#prerequires-building_construction)
    - [Native usage :man_technologist:](#native-usage-man_technologist)
    - [Run with docker :package:](#run-with-docker-package)
  - [Installation :electric_plug:](#installation-electric_plug)
    - [Native usage installation :man_technologist:](#native-usage-installation-man_technologist)
    - [Run as docker container installation :package:](#run-as-docker-container-installation-package)
  - [Monorepo maintain :toolbox:](#monorepo-maintain-toolbox)
  - [Packages Overview :teacher:](#packages-overview-teacher)
    - [Client Package :desktop_computer:](#client-package-desktop_computer)
    - [Components Package :art:](#components-package-art)
    - [Server Package :gear:](#server-package-gear)
    - [Shared Package :link:](#shared-package-link)

---

## Description :writing_hand:

> :bulb: Project for maintaining & analizing IoT data :link:.

### Quick overview :eyes:

List of technologies used in this project:

- :hammer: Built as monorepo with [lerna](https://lerna.js.org/) support.
- :gear: Backend built with [Nest.js](https://nestjs.com/).
- :floppy_disk: [PostgreSQL](floppy_disk) as store database & [Redis](https://redis.io/) as cache database.
- :mailbox_with_mail: [Apache Kafka](https://kafka.apache.org/) as a message brocker.
- :globe_with_meridians: Client built with [Next.js](https://nextjs.org/)
- :art: UI built with [TailwindCSS](https://tailwindcss.com/) & [Aceternity UI](https://ui.aceternity.com/)

---

## Prerequires :building_construction:

### Native usage :man_technologist:

<img width="200px" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTTogwU6U5z0Zf2lUxTE72JAKxVd52klwPe-Q&s" alt="node.js logo">

In ability to run following project you need to have following packages installed in you machine:

- `Node.js` >= v22.4.0
- `lerna` >= 8.1.5
- `Bun.js` >= 1.1.17

### Run with docker :package:

<img width="200px" src="https://cdn.worldvectorlogo.com/logos/docker.svg" alt="node.js logo">

In ability to run following project you need to have following packages installed in you machine:

- `docker` >= 27.0.3
- `docker-compose` >= 2.28.1

---

## Installation :electric_plug:

### Native usage installation :man_technologist:

This project is for the Node.js **22.4.0 release or later**.

> `$ node --version` > `$ v22.4.0`

To install just clone this repo

> `$ git clone https://github.com/tolikhalas/Siema-Tech-Monorepo-v2` > `$ Cloning into 'Siema-Tech-Monorepo-v2 ...`

### Run as docker container installation :package:

This project is for the Node.js **22.4.0 release or later**.

> `$ node --version` > `$ v22.4.0`

... docker **27.0.3 release or later**.

> `$ docker --version` > `$ 27.0.3`
>
> ... & docker-compose **27.0.3 release or later**.

> `$ docker-compose --version` > `$ Docker Compose version 2.28.1`

To install just clone this repo

> `$ git clone https://github.com/tolikhalas/Siema-Tech-Monorepo-v2` > `$ Cloning into 'Siema-Tech-Monorepo-v2 ...`

## Monorepo maintain :toolbox:

Project built with [lerna](https://lerna.js.org/) & consists of 4 packages:

- `shared` - package for DTOs, interfaces & etc.
- `backend` - package for RESTful API with Nest.js
- `client` - package for front-end UI
- `components` - package for shared front-end components

Run project:

> `$ bun dev`

Test project:

> `$ bun test`

Build project:

> `$ bun build`

---

## Packages Overview :teacher:

### Client Package :desktop_computer:

This package contains the Next.js application for the client-side UI. It utilizes TypeScript, TailwindCSS, Framer Motion for animations, and Aceternity UI for consistent design components.

### Components Package :art:

This package provides reusable UI components built with Next.js, TypeScript, TailwindCSS, Framer Motion, and Aceternity UI. These components are designed to be shared across different parts of the project to ensure a cohesive design and functionality.

### Server Package :gear:

This package contains the server-side code built with Nest.js, TypeScript, TypeORM, PostgreSQL, JWT for authentication, Kafka for messaging, and Redis for caching. It serves as the core of the project's RESTful API.

### Shared Package :link:

This package includes cross-project DTOs, types, interfaces, and other shared utilities. It ensures consistency and type safety across the client, components, and backend packages.
