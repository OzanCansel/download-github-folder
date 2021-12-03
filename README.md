# dgf - Download Github Folder
Allows to download a sub-folder in a github repo.

It is a bash script.

#### Depends On
- curl
- echo
- grep
- mkdir

Tested only on Linux.

## Usage

General Usage
```sh
./dgf.sh <repo_url> <auth_token>
```

Download [a repo](https://github.com/OzanCansel/fsconfig) without personal access token
```sh
./dgf.sh https://github.com/OzanCansel/fsconfig/tree/master
```

Download [a repo](https://github.com/OzanCansel/fsconfig) with your personal access token.

Note : Replace the token with yours, this token is fake.
```sh
./dgf.sh https://github.com/OzanCansel/fsconfig/tree/master ghp_N0PwoHr4yvYy21Cu5gscSdjImcGGtrauQcuy
```

```
fsconfig/.gitignore
fsconfig/CMakeLists.txt
fsconfig/LICENSE
fsconfig/README.md
fsconfig/cmake/fsconfig-config.cmake.in
fsconfig/example/CMakeLists.txt
fsconfig/example/app-settings-example.cpp
fsconfig/include/fsconfig/fsconfig.hpp
fsconfig/test/CMakeLists.txt
fsconfig/test/car/engine/capacity
fsconfig/test/car/engine/hp
fsconfig/test/car/engine/type
fsconfig/test/car/name
fsconfig/test/car/owner
fsconfig/test/catch.hpp
fsconfig/test/constructor-test.cpp
fsconfig/test/is_set-test.cpp
fsconfig/test/set-test.cpp
fsconfig/test/sub-test.cpp
fsconfig/test/subscript-operator-test.cpp
fsconfig/test/value-test.cpp
```

Download [a folder](https://github.com/OzanCansel/fsconfig/tree/master/test) in [a repo](https://github.com/OzanCansel/fsconfig)
```sh
./dgf.sh https://github.com/OzanCansel/fsconfig/tree/master/test
```

```
fsconfig/test/CMakeLists.txt
fsconfig/test/car/engine/capacity
fsconfig/test/car/engine/hp
fsconfig/test/car/engine/type
fsconfig/test/car/name
fsconfig/test/car/owner
fsconfig/test/catch.hpp
fsconfig/test/constructor-test.cpp
fsconfig/test/is_set-test.cpp
fsconfig/test/set-test.cpp
fsconfig/test/sub-test.cpp
fsconfig/test/subscript-operator-test.cpp
fsconfig/test/value-test.cpp
```

Download [the sh documentation folder](https://github.com/torvalds/linux/tree/v5.15/Documentation/sh) in [linux repo v5.15](https://github.com/torvalds/linux/tree/v5.15)
```sh
./dgf.sh https://github.com/torvalds/linux/tree/v5.15/Documentation/sh 
```
```
linux/Documentation/sh/booting.rst
linux/Documentation/sh/features.rst
linux/Documentation/sh/index.rst
linux/Documentation/sh/new-machine.rst
linux/Documentation/sh/register-banks.rst
```
## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
[MIT](https://raw.githubusercontent.com/OzanCansel/download-github-folder/master/LICENSE)
