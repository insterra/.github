# InsTerra

`insterra` is a play on words. Has reference to the italian word which means "in the earth" and also plays on `instellar`. It's often used to describe planting of the seed, the beginning of something. The Insterra service in OpsMaru platform is the engine that assists users in bootstrapping and 'seeding' their own platform.

This organization serves as a collection of repositories that serve as learning data for `upmaru/insterra` project. Insterra learns and indexes, labels the contents of these repositories to build a library of `block` and `presets` that can be utilized by users of `upmaru/instellar`. It is recommended that each repository contains the maximum possibilities of the modules available to be learned by the algorithm.

## Types

There are 2 possible types of catalogs `blueprint` and `builder`. They both serve a different purpose.

- `blueprint` - Used for cataloging all the components required to generate infrastructure code (hcl)
- `builder` - Used for cataloging all the components required to `build` applications (yml)

## Blueprint Format

The configuration format should be `tf.json` for terraform related blocks and modules since they're going to be read by the machine. For application build packs please use `.json` to ensure consistency.

## Builder Format

The configuration format should be in `yml`. The catalog processor will read the yaml configuration and essentially index the `template` type of the packs first, then execute on the `extension` pack type.
