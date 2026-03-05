[![CI-workflow](https://github.com/juhahinkula/ci-testing-demo/actions/workflows/ci.yml/badge.svg)](https://github.com/juhahinkula/ci-testing-demo/actions/workflows/ci.yml)

## Node.js Application for CI Training

This repository is training on creating a CI pipeline using GitHub Actions.

### Instructions
1. Fork this repository, clone it to your local machine, and install the required dependencies.
2. Create a `./github/workflows/ci_workflow.yaml` file.
3. Define a workflow to:
 - build the application
 - run tests
 - perform linting
5. Fix any errors encountered during the process.

### Running, Building, and Linting the Project

To manage the project, use the following npm commands:

- **Install the application**:
  ```bash
  npm ci
  ```

- **Run the application**:
  ```bash
  npm start
  ```

- **Test the application**:
  ```bash
  npm test
  ```

- **Build the application**:
  ```bash
  npm run build
  ```

- **Lint the code**:
  ```bash
  npm run lint
  ```

## Docker

Build the Docker image:

```bash
docker build -t ci-trainings:latest .
```

Run the container (map port 3000):

```bash
docker run --rm -p 3000:3000 ci-trainings:latest
```

You can set a custom port with `-e PORT=1234`.
