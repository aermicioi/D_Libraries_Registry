# D language libraries

I want to build a comprehensive list of D language libraries to be used as a reference.

This collection has the intent to help developers find a suitable library for the work and decrease the amount of effort in writing new software.

For any question or contribution, reache me via github pull requests and issues.

## New libraries and corrections

Submissions of new libraries: I accept submissions (as issues or as pull requests). Please
note that description and last update is optional because a script updates it once a day.

Corrections: if information for a library above is wrong, please send a correction as an
issue, pull request, or email. 

## Quality

This list aims to collect libraries of high qualities. Unfortunately I don't have time to test all of them exhaustively.

**If any library does not meet expected requirements (bugs, no tests, no documentation, outdated) open an issue**

Once a library is removed the name will be moved to [removed.md](removed.md) with the hope that they will be corrected by original manteiners or forks.


### Other lists

Also you might be interested in other related, but different lists:

- [Awesome D](https://github.com/zhaopuming/awesome-d): A curated list of awesome D frameworks, libraries and software. Inspired by awesome-python. 

### Categories:

  - Generic libraries 
    - [multi-purpose libraries](#multi-purpose libraries)
  - general purpose
    - [data structures](#data-structures)
    - [string processing](#strings)
    - [scripting](#scripting)
    - [hashing](#hashing)
    - [concurrency](#concurrency)
    - [events](#events)
    - [databases](#databases)
    - [IO](#IO)
  - mathematics
    - [vector math](#vectors)
    - [geometry math](#geometry-math)
    - [general math](#math)
  - parsing
    - [JSON](#json)
    - [other serialization](#serialization)
    - [argv argument processing](#argv)
    - [other parsing](#parsing)
  - graphics
    - [textmode](#graphics-text)
    - [graphics](#graphics-3d)
    - [3D geometry file processing](#geometry-file)
    - [image loading, saving, & processing](#images)
  - audio/video/data compression
    - [compression](#compression)
    - [audio processing & files](#audio)
    - [video](#video)
  - operating system features
    - [files and filenames](#files--filenames)
    - [networking](#network)
    - [hardware interfacing](#hardware)
  - debugging, profiling, testing
    - [debugging](#debugging)
    - [profiling](#profiling)
    - [unit testing etc.](#tests)
  - other
    - [AI](#ai)
    - [cryptography](#crypto)
    - [randomization](#randomization)
    - [user interface](#user-interface)
    - [miscellaneous](#miscellaneous)

# Multi-purpose
| library                                                               | license              | gc |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [ae](https://github.com/CyberShadow/ae)                               | MPL 2                | Yes || 
| [Dlib](https://github.com/gecko0307/dlib)                             | Boost                | No  || 
| [iz](https://github.com/BBasile/iz)                                   | Boost                | No  || 
| [fast](https://github.com/mleise/fast)                                | GPLv3                | No  || 
| [jive](https://github.com/krox/jive)                                  | Public Domain        | No  || 
| [kiss](https://github.com/huntlabs/kiss)                              | Apache 2             | No  || 
| [Ocean](https://github.com/sociomantic-tsunami/ocean)                 | BSD                  | No  || 
| [phobos](https://github.com/dlang/phobos)                             | Boost                | Yes || 
| [Tango-D2](https://github.com/SiegeLord/Tango-D2)                     | BSD                  | Yes || 
| [tango-rt](https://github.com/sociomantic-tsunami/tangort)            | BSD                  | No  || 
| [Tanya](https://github.com/caraus-ecms/tanya)                         | MPL 2                | No  || 
| [Thrift-d](https://github.com/dhasenan/thrift-d)                      | Apache 2             | Yes || 

# AI
| library                                                               | license              | gc |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [dnnet](https://github.com/henrygouk/dnnet)                           | Mit                  | Yes || 
| [doll](https://github.com/putyy/doll)                                 | Proprietary          | Yes || 
| [vectorflow](https://github.com/Netflix/vectorflow)                   | Apache 2          | Yes || 

# argv
| library                                                               | license              | gc |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [argsd](https://github.com/burner/argsd)                              | MIT                  | Yes || 
| [argon](https://github.com/markuslaker/Argon)                         | ISC                  | Yes || 
| [commander.d](https://github.com/yamadapc/commander.d)                | MIT                  | Yes || 
| [commando](https://github.com/SirTony/commando/)                      | MIT                  | Yes || 
| [darg](https://github.com/jasonwhite/darg)                            | Mit                  | Yes || 
| [parseopts](https://github.com/mitchgrout/parseopts)                  | Unknown              | Yes || 

# audio
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [Ddsp](https://github.com/abaga129/Ddsp)                              | MIT                  | Yes || 
| [Dplug](https://github.com/AuburnSounds/Dplug)                        | Various              | Yes || 
| [dlang-jack](https://github.com/martinez/dlang-jack)                  | BSL 1                | Yes || 
| [DerelictFmod](https://github.com/Extrawurst/DerelictFmod)            | MIT                | Yes || 
| [djack](https://github.com/cosenmarco/djack)                          | GPLv3                | Yes || 
| [DerelectBass](https://github.com/p0nce/DerelictBASS)                 | Boost                | Yes || 
| [wasapi](https://github.com/buggins/wasapi)                           | Boost                | Yes || 

# compression
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [archive](https://github.com/rcythr/archive)                          | BSL 1                | Yes || 
| [dcompress](https://github.com/byebye/dcompress)                      | Unknown              | No  || 
| [lz77text](https://github.com/Superstar64/lz77text)                   | Boost                | Yes || 

# concurrency
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [jin.go](https://github.com/nin-jin/go.d)                             | Public Domain        | Yes || 
| [workermanager](https://github.com/alphaKAI/workermanager)            | Unknown              | Yes || 

# crypto
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [botan](https://github.com/etcimon/botan)                             | Unknown/Closed       | Yes || 

# data structures
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [aammm](https://github.com/arexeu/aammm)                              | BSL 1                | No  || 
| [ArrayList](https://github.com/0xEAB/arraylist)                       | Public Domain        | Yes || 
| [containers](https://github.com/economicmodeling/containers)          | MIT                  | No  || 
| [darray](https://github.com/burner/darray)                            | LGPL 3               | Yes || 
| [Dgraph](https://github.com/WebDrake/Dgraph)                          | GPLv3                | Yes  || 
| [dhtnode](https://github.com/sociomantic-tsunami/dhtnode)             | MIT                  | No  || 
| [hash](https://github.com/Mihail-K/hash)                              | MIT                  | Yes || 
| [JudyD](https://github.com/rfarr/JudyD)                               | ISC                  | No  || 
| [memutils](https://github.com/etcimon/memutils)                       | MIT                  | No  || 
| [mir-algorithm](https://github.com/libmir/mir-algorithm)              | BSL 1                | No  || 
| [std.rcstring](https://github.com/burner/std.rcstring)                | Boost                | No  || 
| [vebtree](https://bitbucket.org/Sandman8/vebtree)                     | MIT                  | Yes | 2016-Oct-28 |A library for van Emde Boas tree 

# databases
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# debugging
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# events
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# files & filenames
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# geometry file
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# geometry math
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# graphics (text)
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# graphics
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# hardware
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# hashing
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# images
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# IO
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# math
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [botan-math](https://github.com/etcimon/botan-math)                  | BSD 2                | Yes || 
| [scid](https://github.com/DlangScience/scid)                          | Boost                | Yes || 

# network
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# serialization
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------7
| [msgpack-ll](https://github.com/jpf91/msgpack-ll)                     | BSL 1                | No  || 

# json
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# parsing
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# profiling
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# randomization
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# scripting
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# strings
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# tests
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [unit-threaded](https://github.com/atilaneves/unit-threaded)          | BSD                  | Yes || 

# user interface
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# vectors
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# video
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# miscellaneous
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------



## Thanks

Thanks to [nothings](https://github.com/nothings/single_file_libs) for inspiration.
