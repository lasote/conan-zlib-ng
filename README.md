[![Build Status](https://travis-ci.org/lasote/conan-zlib-ng.svg)](https://travis-ci.org/lasote/conan-zlib-ng)


# conan-zlib-ng

[Conan.io](https://conan.io) package for ZLIB library

The packages generated with this **conanfile** can be found in [conan.io](https://conan.io/source/zlib-ng/1.2.8/lasote/stable).
Sources from Dead2/zlib-ng repository: https://github.com/Dead2/zlib-ng

## Build packages

    $ pip install conan_package_tools
    $ python build.py
    
## Upload packages to server

    $ conan upload zlib-ng/1.2.8@lasote/stable --all
    
## Reuse the packages

### Basic setup

    $ conan install zlib-ng/1.2.8@lasote/stable
    
### Project setup

If you handle multiple dependencies in your project is better to add a *conanfile.txt*
    
    [requires]
    zlib-ng/1.2.8@lasote/stable

    [options]
    zlib-ng:shared=true # false
    
    [generators]
    txt
    cmake

Complete the installation of requirements for your project running:</small></span>

    conan install . 

Project setup installs the library (and all his dependencies) and generates the files *conanbuildinfo.txt* and *conanbuildinfo.cmake* with all the paths and variables that you need to link with your dependencies.
