# InsTerra

`insterra` is a play on words. Has reference to the italian word which means "in the earth". It's often used to describe planting of the seed, the beginning of something. The Insterra service in OpsMaru platform is the engine that assists users in bootstrapping and 'seeding' their own platform.

This organization serves as a collection of repositories that serve as learning data for `upmaru/insterra` project. Insterra learns and indexes, labels the contents of these repositories to build a library of `block` and `presets` that can be utilized by users of `upmaru/instellar`. It is recommended that each repository contains the maximum possibilities of the modules available to be learned by the algorithm.

## Format

The configuration format should be `tf.json` for terraform related blocks and modules since they're going to be read by the machine. For application build packs please use `.json` to ensure consistency.
