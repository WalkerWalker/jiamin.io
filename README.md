# Jiamin Zhu's Blog

Based on Mark Otto's Hyde Jekyll Template and forked from Chris Schuld's Blog repo

## Local Development - Building
    export JEKYLL_VERSION=3.7
    docker run --env=DEBUG=true --rm --volume="/var/www/chrisschuld.com:/srv/jekyll" -it jekyll/jekyll:$JEKYLL_VERSION jekyll build

## Local Development - Execution
    export JEKYLL_VERSION=3.7
    docker run --name chrisschuld.com --env=DEBUG=true --rm --volume="/private/var/www/chrisschuld.com/:/srv/jekyll" -p 3000:4000 -it jekyll/jekyll:$JEKYLL_VERSION jekyll serve --watch --drafts

## Author

**Jiamin Zhu**
- <https://github.com/walkerwalker>
- <https://twitter.com/cbschuld>


## License

Open sourced under the [MIT license](LICENSE.md).

<3
