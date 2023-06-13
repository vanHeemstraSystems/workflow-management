[![Quarto Publish](https://github.com/vanHeemstraSystems/map-management/actions/workflows/publish.yml/badge.svg)](https://github.com/vanHeemstraSystems/map-management/actions/workflows/publish.yml)

map-management
# Map Management

Can be read as "Map Management" at https://app.gitbook.com/s/Rs3XPuVclvoj92Exb9AA/

Can be browsed as "Map Management" at https://vanheemstrasystems.github.io/map-management/

Documentation of this repository is automatically done with Quarto using GitHub Actions as described at https://github.com/vanHeemstraSystems/quarto-to-github-pages/blob/main/300/300/README.md

Based on "How to Run PostgreSQL and pgAdmin Using Docker" at https://towardsdatascience.com/how-to-run-postgresql-and-pgadmin-using-docker-3a6a8ae918b5

Based on "JointJS - React Example App With TypeScript And SCSS Using Create-React-App" at https://resources.jointjs.com/tutorial/react-ts

Create yarn.lock file as follows:

```
$ cd containers/app/main
$ yarn install
```

Run as follows:

```
$ cd containers/app
$ docker-compose --file docker-compose.dev.yml --project-name map-management-dev up --build -d
```

**NOTE**: When you try to login to PostgreSQL database via **Adminer**, use the following credentials:

- System: PostgreSQL
- Server: = IP address and exposed postgresql port (e.g. :5432) of the Docker host =
- Username: Postgres
- Password: = can be set or found in your environment variables file .env =
- Database: = leave this blank =

If you tick the "Permanent login" box, next time you visit the login page, your previous shortcut will be shown.
