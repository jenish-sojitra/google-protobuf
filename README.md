# Build instructions

Build by running `./build.sh` — it downloads the specified version of `@grpc/grpc-js`, patches it,
and puts it into `./package`.

`./package` is a build artifact and is present in the repo just for convenience/visibility.

## Warning

Generated `_pb.js` files need patching!

See [fix_pb.sh](./fix_pb.sh) file for replacements in `*_pb.js` files.

Usage: `./fix_pb.sh path-to-pbs/*_pb.js`.
