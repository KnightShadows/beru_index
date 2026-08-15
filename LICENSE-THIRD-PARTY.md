# Third-Party Licenses

The `beru_index` repository contains package management metadata, build instructions (recipes), and URLs referencing third-party open-source software. 

**Disclaimer:** This repository does **not** host, distribute, or bundle the source code or binaries of the third-party libraries listed below. When you use the Beru CLI to build these packages, the Beru orchestrator downloads the source code directly from the original authors' repositories. You are solely responsible for complying with the licensing terms of any third-party software you compile and link into your applications.

Below is a non-exhaustive summary of the primary third-party libraries referenced in this index and their typical open-source licenses:

## Boost Software License 1.0 (BSL-1.0)
* **Boost** (`boostorg/boost`)
* **Asio** (`chriskohlhoff/asio`)
* **Beast** (`boostorg/beast`)
* **Outcome** (`ned14/outcome`)

## MIT License
* **fmt** (`fmtlib/fmt`)
* **spdlog** (`gabime/spdlog`)
* **nlohmann-json** (`nlohmann/json`)
* **CLI11** (`CLIUtils/CLI11`)
* **cxxopts** (`jarro2783/cxxopts`)
* **entt** (`skypjack/entt`)
* **magic_enum** (`Neargye/magic_enum`)
* **pugixml** (`zeux/pugixml`)
* **tabulate** (`p-ranav/tabulate`)
* **simdjson** (`simdjson/simdjson`)
* **cereal** (`USCiLab/cereal`)
* **sol2** (`ThePhD/sol2`)
* **stduuid** (`mariusbancila/stduuid`)
* **nameof** (`Neargye/nameof`)
* **rapidjson** (`Tencent/rapidjson`)
* **yyjson** (`ibireme/yyjson`)

## Apache License 2.0
* **Abseil** (`abseil/abseil-cpp`)
* **Folly** (`facebook/folly`)
* **gRPC** (`grpc/grpc`)
* **RocksDB** (`facebook/rocksdb`)
* **Poco** (`pocoproject/poco`) - *Note: POCO uses the Boost Software License 1.0*
* **s2n-tls** (`aws/s2n-tls`)
* **SOCI** (`SOCI/soci`)
* **Arrow** (`apache/arrow`)

## BSD 3-Clause License
* **GoogleTest** (`google/googletest`)
* **Google Benchmark** (`google/benchmark`)
* **glog** (`google/glog`)
* **gflags** (`gflags/gflags`)
* **Protobuf** (`protocolbuffers/protobuf`)
* **FlatBuffers** (`google/flatbuffers`)
* **pybind11** (`pybind/pybind11`)
* **Snappy** (`google/snappy`)
* **zstd** (`facebook/zstd`)
* **LevelDB** (`google/leveldb`)
* **CMake** (`Kitware/CMake`)

## BSD 2-Clause License
* **lz4** (`lz4/lz4`)
* **websocketpp** (`zaphoyd/websocketpp`)

## Zlib License
* **zlib** (`madler/zlib`)
* **miniz** (`richgel999/miniz`)
* **SDL** (`libsdl-org/SDL`)
* **SFML** (`SFML/SFML`)
* **GLFW** (`glfw/glfw`)
* **libpng** (`glennrp/libpng`)
* **tinyxml2** (`leethomason/tinyxml2`)

## GNU General Public License (GPL) / Lesser GPL (LGPL)
* **GMP** (`gmp-math/gmp`) - *LGPL/GPL*
* **MPFR** (`mpfr-math/mpfr`) - *LGPL*
* **ZeroMQ** (`zeromq/libzmq`) - *LGPL with static linking exception*
* **FFmpeg** (`FFmpeg/FFmpeg`) - *LGPL/GPL depending on configuration*
* **GnuTLS** (`gnutls/gnutls`) - *LGPL*

## SQLite License (Public Domain)
* **SQLite3** (`sqlite/sqlite`)

---

*Note: The licenses listed above are provided for informational purposes only. Licenses can change between package versions. Always verify the `LICENSE` file within the downloaded source code of the specific version you are using.*
