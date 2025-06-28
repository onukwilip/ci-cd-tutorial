# CI/CD Tutorial

This project demonstrates a simple Node.js/Express web server with a CI/CD pipeline setup using GitHub Actions and Docker.

## Features

- Node.js Express server
- Jest tests with Supertest
- Docker support
- CI/CD pipelines for testing and deployment (GitHub Actions)

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- [npm](https://www.npmjs.com/)
- [Docker](https://www.docker.com/) (optional, for containerization)

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/onukwilip/ci-cd-tutorial.git
    cd ci-cd-tutorial
    ```

2. Install dependencies:
    ```sh
    npm install
    ```

### Running Locally

Start the server:
```sh
npm start

Collecting workspace information```markdown
# CI/CD Tutorial

This project demonstrates a simple Node.js/Express web server with a CI/CD pipeline setup using GitHub Actions and Docker.

## Features

- Node.js Express server
- Jest tests with Supertest
- Docker support
- CI/CD pipelines for testing and deployment (GitHub Actions)

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- [npm](https://www.npmjs.com/)
- [Docker](https://www.docker.com/) (optional, for containerization)

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/onukwilip/ci-cd-tutorial.git
    cd ci-cd-tutorial
    ```

2. Install dependencies:
    ```sh
    npm install
    ```

### Running Locally

Start the server:
```sh
npm start
```
The app will be available at [http://localhost:5000](http://localhost:5000) by default.

### Running Tests
```sh
npm test
```

### Using Docker
Build and run the Docker container:
```sh
docker build -t ci-cd-tutorial .
docker run -p 5001:5001 ci-cd-tutorial
```

## CI/CD
- **CI**: On pull requests to `staging` or `main`, tests and (optionally) builds the app ([ci-pipeline.yml](.github/workflows/ci-pipeline.yml)).
- **CD**: On pushes to `staging` or releases, builds and deploys the Docker image to Google Cloud Run ([cd-pipeline.yml](.github/workflows/cd-pipeline.yml)).

## Project Structure
```
.
├── app.js
├── index.js
├── package.json
├── Dockerfile
├── jsconfig.json
├── __tests__/
│   └── index.test.js
└── .github/
    └── workflows/
        ├── ci-pipeline.yml
        └── cd-pipeline.yml
```

## License

ISC
```
