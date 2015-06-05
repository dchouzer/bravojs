BravoJS is an implementation of an unratified proposed draft for CommonJS Modules/2.0

The current draft this code is based on is located at http://www.page.ca/~wes/CommonJS/modules-2.0-7/

The proposal attempts to address several issues
  * Modules/1.1.1 compatibility guarantees
  * Minor Modules/1.1.1 spec bug fixes
  * Formalizing the CommonJS environment
  * Defining a wrapped module format
  * Defining a formal way to specify explicit dependencies
  * Defining a way to lazy-load modules (similar to require.async) in the base-level specification
  * Defining cross-platform hooks which can be used by future work (including transports, packages, mappings)
  * Recommendations for platform-dependent bootstrapping

**Caveat User:** This version of BravoJS is based on an early _draft_ of an _unratified_ CommonJS specification. This means that using this product as it stands today will most likely lead you to writing modules which are not compatible with any other CommonJS platform.

## Package-aware Fork ##
Christoph Dorn is working on a fork of this project which adds CommonJS package/mappings capabilities, implemented around the PINF loader. The announcement is here: http://groups.google.com/group/commonjs/browse_thread/thread/da10667d667a2a3a, along with some useful URLs.

If you are an existing BravoJS user and want to try out Christoph's changes, you can pull from https://christoph-bravojs-packages.googlecode.com/hg/ right into your existing BravoJS repository. Don't forget to <tt>hg update</tt>!