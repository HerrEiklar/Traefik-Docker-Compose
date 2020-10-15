# This is a Traefik docker-compose project

## Basic description

I'm happy that you found my project!

So, this whole thing is optimized to run on a single server,
but I am working on deploying this to docker swarms.

I'm not sure when I'll be done with it, as I have to look into
docker swarms.

## The project structure

The project has a simple structure, and it is as follows:

* configs -> folder for service configuration files (there shouldn't be any private data, passwords or api-tokens in there)
* env_files -> config files for each service, instead of defining in the docker-compose file
* secrets -> in there are all secrets, like api tokens and such
* volumes -> data created by the services, each service has it's own folder, and the file structure is the same as in the service
* .env.sample -> rename this to .env and change the the value of "TRAEFIK_LABEL_HOST" to your domain/needs
* stack.yml -> this is not yet available to public as I am still figuring things out with this one, but just so you know!

## Passwords and secret data

In this project there're secrets used, meaning,
all passwords are in a seperate folder,
and will NOT be pushed, as they are listed in the .gitignore file.

There might be some sample values, just open the project in Visual Studio Code,
or any editor of your choice and search for the term "SAMPLE_VALUE", and replace it
with a value that makes sense.

Generate some digests [here](https://websistent.com/tools/htdigest-generator-tool)

## Standards

I'm trying to be as close to the standards as possible.
Here is what I am using.

[Conventional Commits 1.0.0](https://www.conventionalcommits.org/en/v1.0.0/)
[Semantic Versioning 2.0.0](https://semver.org/lang/de/)
