# elastic-stack-playground

To start navigate to folder 'elastic-compose' and execute the command:

docker-compose up -d

In order to use a custom .env file (for example with local environment) create a file, say .env.local, in the folder 'elastic-compose', set the necessary environment variables or provide custom values and execute the command:

docker-compose --env-file .env.local up -d

In order to check the configuration before to start execute:

docker-compose --env-file .env.local config

To check debug output into console of the running logstash container execute:

docker logs -f logstash
