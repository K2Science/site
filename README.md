# Site of Kotlin for Data

This is the site of Kotlin for Data project.

It aggregates all the main projects we (@SPC-Code and @asm0dey) are aware of. If you know more projects - please let us know in Issues or better yet, make a PR>

## Building/Running the site

There are two ways to build the site:

1. Follow the installation procedure on the [`mkdocs-material` site](https://squidfunk.github.io/mkdocs-material/getting-started/#installation)
2. Build the attached Dockerfile

```bash
docker build -t kodata-mkdocs .
```

Running the site with docker is also just a one-liner:

```bash
docker run --rm -it -p 8000:8000 -v ${PWD}:/docs kodata-mkdocs
```

So what I usuall do is just running these command sequentially

## Contributing

Contributions are very welcome!

The main entry for you as a contributor is the `mkdocs.yml` file.

The very core of the file is the `multirepo` plugin, it allows us to include all the documentation for the respecive modules right into this site.

If you don't know want to write complex config files - that's fine, just let us know what you think and will do our best to improve the site.

Or just spread the word!