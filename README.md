# Storage-of-knowledge

Repository to run storage-of-knowledge application services with dependencies
from scratch.

### Installing

- Clone repository
```
git clone https://github.com/ArtyomSliusar/storage-of-knowledge.git
```

- (OPTIONAL) Configure backend service logging file `logging/logging.json` 

- (OPTIONAL) Configure nginx configuration template `nginx/nginx.conf.template`, it
will be used to automatically create `nginx.conf` with environment variables substituted

- Create .env file in project root folder (use example.env)

- Run all services
```
docker-compose up -d
```

### Configuration

Environment variables for configuration:

- FE - https://github.com/ArtyomSliusar/storage-of-knowledge-fe#configuration
- BE - https://github.com/ArtyomSliusar/storage-of-knowledge-be#configuration
- DOMAIN - application domain used by nginx configuration
- MYSQL_ROOT_PASSWORD - mandatory mysql root user password

### How to

- Stop and remove all containers (ES and MySql data will remain)
```
docker-compose down
```

### TODO:
- clear tokens cron
- aws ecs
- add site monitoring and statistics solution