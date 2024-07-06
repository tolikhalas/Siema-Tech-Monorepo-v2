# Siema Tech Monorepo

> <div style="display: flex; align-items: center;">
> <span>🔥 Powered with <a href="https://bun.sh/">Bun.js</a></span>
> <img style="margin-left: 5px;" width="24px" src="https://user-images.githubusercontent.com/709451/182802334-d9c42afe-f35d-4a7b-86ea-9985f73f20c3.png" alt="bun.js icon">
> </div>

---

## Description

:bulb: Project for maintaining & analizing IoT data.

### Quick overview

List of technologies used in this project:

- :hammer: Built as monorepo with [lerna](https://lerna.js.org/) support.
- :gear: Backend built with [Nest.js](https://nestjs.com/).
- :floppy_disk: [PostgreSQL](floppy_disk) as store database & [Redis](https://redis.io/) as cache database.
- :mailbox_with_mail: [Apache Kafka](https://kafka.apache.org/) as a message brocker.
- :globe_with_meridians: Client built with [Next.js](https://nextjs.org/)
- :art: UI built with [TailwindCSS](https://tailwindcss.com/) & [Aceternity UI](https://ui.aceternity.com/)

## Prerequires

---

### Native usage

In ability to run following project you need to have following packages installed in you machine:

- `Node.js` >= v22.4.0
- `lerna` >= 8.1.5
- `Bun.js` >= 1.1.17

### Run with docker

In ability to run following project you need to have following packages installed in you machine:

- `docker` >= 27.0.3
- `docker-compose` >= 2.28.1

## Monorepo maintain

---

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

----
