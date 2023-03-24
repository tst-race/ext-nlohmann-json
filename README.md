# nlohmann-json for RACE

This repo provides scripts to custom-build the
[nlohmann-json library](https://github.com/nlohmann/json) for RACE.

## License

The nlohmann-json library is licensed under the MIT license.

Only the build scripts in this repo are licensed under Apache 2.0.

## Dependencies

nlohmann-json has no dependencies on any custom-built libraries.

## How To Build

The [ext-builder](https://github.com/tst-race/ext-builder) image is used to
build nlohmann-json.

```
git clone https://github.com/tst-race/ext-builder.git
git clone https://github.com/tst-race/ext-nlohmann-json.git
./ext-builder/build.py \
    --target linux-x86_64 \
    ./ext-nlohmann-json
```

## Platforms

nlohmann-json is built for the following platforms:

* `linux-x86_64`
* `linux-arm64-v8a`
* `android-x86_64`
* `android-arm64-v8a`

## How It Is Used

nlohmann-json is used directly by the RACE core.
