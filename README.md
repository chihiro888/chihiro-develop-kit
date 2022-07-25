# Save The Query

## Initial Setting

### install nodeenv for mac

```bash
brew install nodeenv
```

### create nodeenv

```bash
nodeenv --node=16.16.0 nenv
```

### setup nodeenv

```bash
. nenv/bin/activate
```

### install yarn

```bash
npm install -g yarn
```

## database

```bash
cd infra
docker-compose up
```

| key           | value          |
| ------------- | -------------- |
| host          | localhost      |
| port          | 3306           |
| database      | save_the_query |
| root user     | root           |
| root password | root           |
| user          | docker         |
| password      | docker         |

## backend

- Please create the database with docker first.

```bash
cd backend
yarn install

# if local
yarn start:local

# if development
yarn start:dev

# if production
yarn start:prod
```

http://localhost:9000/api

## frontend

```bash
cd frontend
yarn install
yarn start
```

http://localhost:3000/

# License

<img src="docs/image/License.png" width="300"/>

https://themeforest.net/item/metronic-responsive-admin-dashboard-template/4021469
