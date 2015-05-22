Pip 7 and Travis caching
========================

This is a throwaway repository to demonstrate how much faster you can make your
Travis builds by caching Python dependencies using the [automatic wheel
builder][pip7] functionality introduced by pip version 7.

The repository doesn't do anything useful, it just installs some Python packages
that are traditionally slow to build.

See `.travis.yml` for an example of how to make your builds faster.

- [**First build**: 2m28s](https://travis-ci.org/nickstenning/travis-pip-cache/builds/63622073)
- [**Second build**: 16s](https://travis-ci.org/nickstenning/travis-pip-cache/builds/63622544)
