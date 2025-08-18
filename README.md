# Prisma API with NestJS
> A complete REST API built with NestJS, Prisma ORM, Swagger for documentation, and Docker for containerization.

[![NPM Version][npm-image]][npm-url]
[![Build Status][travis-image]][travis-url]
[![Downloads Stats][npm-downloads]][npm-url]

This project is part of my learning journey from the [NestJS from Zero](https://www.udemy.com/course/nestjs-do-zero/) course on Udemy.  
It demonstrates how to build a modular, scalable, and production-ready API using **NestJS**, **Prisma**, **Docker**, and **Swagger** for interactive API documentation.

![](header.png)

---

## 🚀 Features
- **NestJS Framework**: Modern Node.js framework for scalable backend applications.
- **Prisma ORM**: Type-safe database access with auto-generated queries.
- **Swagger UI**: Interactive API documentation at `/api/docs`.
- **Docker Support**: Easy containerization and deployment with `docker-compose`.
- **Environment Variables**: Configurable `.env` setup for database and application configs.

---

## ⚙️ Installation

### Requirements
- Node.js (>= 18.x)
- Docker & Docker Compose
- npm or yarn package manager

### Setup

#### OS X & Linux
```sh
git clone https://github.com/stanycruz/prisma-api.git
cd prisma-api
npm install
```

#### Windows
```sh
git clone https://github.com/stanycruz/prisma-api.git
cd prisma-api
npm install
```

---

## ▶️ Running the Project

### Run with Docker (Recommended)
```sh
docker-compose up --build
```

### Run locally
```sh
npm run start:dev
```

API will be available at: [http://localhost:3000](http://localhost:3000)  
Swagger documentation: [http://localhost:3000/api/docs](http://localhost:3000/api/docs)

---

## 💻 Usage Example

Example request using **cURL**:

```sh
curl -X GET http://localhost:3000/users
```

Example request with **Axios** in Node.js/React:

```ts
import axios from 'axios';

const users = await axios.get('http://localhost:3000/users');
console.log(users.data);
```

---

## 🛠 Development Setup

To reset database and run migrations:

```sh
npx prisma migrate dev
```

To open Prisma Studio (GUI for database):
```sh
npx prisma studio
```

To run tests:
```sh
npm run test
```

---

## 📦 Release History

* 0.2.0
    * ADD: Swagger integration at `/api/docs`
    * ADD: Docker support with docker-compose
    * CHANGE: Improved Prisma schema and migrations
* 0.1.0
    * Initial NestJS project with Prisma integration

---

## 👤 Author

Stany Cruz – [@stanycruz](https://github.com/stanycruz)

Distributed under the MIT license. See ``LICENSE`` for more information.

[https://github.com/stanycruz/prisma-api](https://github.com/stanycruz/prisma-api)

---

## 🤝 Contributing

1. Fork it (<https://github.com/stanycruz/prisma-api/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

<!-- Markdown link & img dfn's -->
[npm-image]: https://img.shields.io/npm/v/datadog-metrics.svg?style=flat-square
[npm-url]: https://npmjs.org/package/datadog-metrics
[npm-downloads]: https://img.shields.io/npm/dm/datadog-metrics.svg?style=flat-square
[travis-image]: https://img.shields.io/travis/dbader/node-datadog-metrics/master.svg?style=flat-square
[travis-url]: https://travis-ci.org/dbader/node-datadog-metrics
[wiki]: https://github.com/stanycruz/prisma-api/wiki
