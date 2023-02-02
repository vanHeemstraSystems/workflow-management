[![Quarto Publish](https://github.com/vanHeemstraSystems/financial-management/actions/workflows/publish.yml/badge.svg)](https://github.com/vanHeemstraSystems/financial-management/actions/workflows/publish.yml)

financial-management
# Financial Management

Based on "Actual" at https://github.com/actualbudget/actual

Based on "Actual Server" at https://hub.docker.com/r/jlongster/actual-server

Based on "Actual - Documentation" at https://actualbudget.github.io/docs/

Create yarn.lock file as follows:

```
$ cd containers/app/main
$ yarn install
```

Run as follows:

```
$ cd containers/app
$ docker-compose --file docker-compose.dev.yml --project-name financial-management-dev up --build -d
```

## Accessing Actual
You should now be able to access http://localhost:5006 in your browser and you will see Actual.

When first accessing Actual, you may be prompted to provide a URL for the server. In this case (when installing locally), you can input http://localhost:5006 or click the “use this domain” button below the text field (which will do the same thing).
