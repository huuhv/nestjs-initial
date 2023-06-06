# Install without Docker

## Prerequisites

- Node `v18.15.0` with npm
- Mysql version `^8.0`
- Redis version `^7.0`

## Installation

- First, you need clone source code:

  ```shell
  git clone git@github.com:framgia/jmb-app-be.git
  ```

- Then, create the `.env` file from example and update its content:

  ```shell
  cp .env.example .env
  ```

- Finally, install all node dependencies:

  ```shell
  npm install
  ```
