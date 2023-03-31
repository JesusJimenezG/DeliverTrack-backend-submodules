# DeliverTrack microservices backend

This is the backend for DeliverTrack, a microservices based application that allows users to order food from restaurants and track their delivery robots in real time.

## Microservices

The backend is composed of the following microservices:

- [auth](https://github.com/JesusJimenezG/DeliverTrack-auth-service.git)
- [orders](/)
- [real time tracking](https://github.com/JesusJimenezG/DeliverTrack-live-tracking-service.git)

## Tech stack

- [Node.js](https://nodejs.org/en/)
- [Express](https://expressjs.com/)
- [Redis](https://redis.io/)
- [PostgreSQL](https://www.postgresql.org/)
- [Prisma](https://www.prisma.io/)
- [JWT](https://jwt.io/)
- [Socket.io](https://socket.io/)
- [Docker](https://www.docker.com/)

## Getting started

### Prerequisites

- [Node.js](https://nodejs.org/en/)
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)
- [PostgreSQL](https://www.postgresql.org/)
- [Redis](https://redis.io/)

### Installation

1. Clone the repo

    ```sh
    git clone https://github.com/JesusJimenezG/DeliverTrack-backend-submodules
    ```

2. Install NPM packages

    ```sh
    npm install
    ```

3. Start the services

    ```sh
    docker-compose up
    ```

4. Run the migrations within the `auth` service

    ```sh
    cd auth-servide
    npm run docker:db:migrate
    npm run docker:rebuild
    ```

<!-- 5. Run the migrations within the `orders` service

    ```sh
    cd orders-service
    npm run docker:db:migrate
    npm run docker:rebuild
    ```

6. Run the migrations within the `real time tracking` service

    ```sh
    cd live-tracking-service
    npm run docker:db:migrate
    npm run docker:rebuild
    ```

7. Add some mock data to the database -->
