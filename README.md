# DEMO API

## Installation

- [With Docker](./docs/install_with_docker.md)
- [Without Docker](./docs/install_without_docker.md)

## Development

| Command                     | With Docker (`main` command) | Without Docker     |
| --------------------------- | ---------------------------- | ------------------ |
| Build                       | ./main build                 | npm install        |
| Add new package             | ./main npm install ...       | npm install ...    |
| Nest CLI                    | ./main npx nest ...          | npx nest ...       |
| Running                     | N/A                          | npm run start      |
| Running in watch mode       | ./main up -d                 | npm run start:dev  |
| View app log                | ./main logs api -f           | View in watch mode |
| Stop the app                | ./main down                  | `control + C`      |
| Prisma CLI                  | ./main npx prisma            | npx prisma         |
| Test                        | ./main test                  | npm run test       |
| Custom command in container | ./main shell                 | N/A                |
| `main` command usage        | ./main                       | N/A                |

## Deployment

Updating
