UPGRADE 3.x
===========

UPGRADE FROM 3.13 to 3.14
=========================

### SonataEasyExtends is deprecated

Registering `SonataEasyExtendsBundle` bundle is deprecated, it SHOULD NOT be registered.
Register `SonataDoctrineBundle` bundle instead.

UPGRADE FROM 3.1 to 3.2
=======================

- Doctrine MongoDb metadata `comments_count` has been changed to `commentsCount`. In case of having problems, please update your collections.

UPGRADE FROM 3.0 to 3.1
=======================

### Tests

All files under the ``Tests`` directory are now correctly handled as internal test classes.
You can't extend them anymore, because they are only loaded when running internal tests.
More information can be found in the [composer docs](https://getcomposer.org/doc/04-schema.md#autoload-dev).
