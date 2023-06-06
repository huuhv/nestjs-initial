# Install with Docker

## Prerequisites

- Docker. Tested with `v23.0.2`.
- Docker Compose. Tested with `v2.15.1`.

## Installation

- First, you need clone source code:

  ```shell
  git clone git@github.com:framgia/jmb-app-be.git
  ```

- Then, create the `.env` file from example and update its content:

  ```shell
  cp .env.example .env
  ```

- Finally, build the stack using `main` command:

  ```shell
  ./main build
  ```

  To see the `main` command usage, call it without any parameters:

  ```shell
  ./main
  ```
