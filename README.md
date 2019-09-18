# Jiamin Zhu's Blog

Based on Mark Otto's Hyde Jekyll Template and forked from Chris Schuld's Blog repo

## Local Development - Building
    export JEKYLL_VERSION=3.7
    docker run --env=DEBUG=true --rm --volume="/var/www/jiamin.io:/srv/jekyll" -it jekyll/jekyll:$JEKYLL_VERSION jekyll build

## Local Development - Execution
    export JEKYLL_VERSION=3.7
    docker run --name jiamin.io --env=DEBUG=true --rm --volume="/private/var/www/jiamin.io/:/srv/jekyll" -p 3000:4000 -it jekyll/jekyll:$JEKYLL_VERSION jekyll serve --watch --drafts

## License

Open sourced under the [MIT license](LICENSE.md).

<3
