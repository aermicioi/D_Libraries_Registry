# D language libraries

I want to build a comprehensive list of D language libraries to be used as a reference.

This collection has the intent to help developers find a suitable library for the work and decrease the amount of effort in writing new software.

For any question or contribution, reache me via github pull requests and issues.



### Other lists

Also you might be interested in other related, but different lists:

- [Awesome D](https://github.com/zhaopuming/awesome-d): A curated list of awesome D frameworks, libraries and software. Inspired by awesome-python. 

### Categories:

  - [multi-purpose libraries](#multi-purpose libraries)
  - general purpose
    - [data structures](#data-structures)
    - [string processing](#strings)
    - [scripting](#scripting)
    - [hashing](#hashing)
    - [concurrency](#concurrency)
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
| [phobos](https://github.com/dlang/phobos)                             | Boost                | Yes || 
| [Tango-D2](https://github.com/SiegeLord/Tango-D2)                     | BSD                  | Yes || 
| [Tanya](https://github.com/caraus-ecms/tanya)                         | MPL 2                | No  || 
| [Dlib](https://github.com/gecko0307/dlib)                             | Boost                | No  || 
| [Ocean](https://github.com/sociomantic-tsunami/ocean)                 | BSD                  | No  || 
| [ae](https://github.com/CyberShadow/ae)                               | MPL 2                | Yes || 
| [iz](https://github.com/BBasile/iz)                                   | Boost                | No  || 
| [kiss](https://github.com/huntlabs/kiss)                              | Apache 2             | No  || 
| [tango-rt](https://github.com/sociomantic-tsunami/tangort)            | BSD                  | No  || 
| [jive](https://github.com/krox/jive)                                  | Public Domain        | No  || 
| [Thrift-d](https://github.com/dhasenan/thrift-d)                      | Apache 2             | Yes || 
| [fast](https://github.com/mleise/fast)                                | GPLv3                | No  || 

# AI
| library                                                               | license              | gc |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [dnnet](https://github.com/henrygouk/dnnet)                           | Mit                  | Yes || 
| [doll](https://github.com/putyy/doll)                                 | Proprietary          | Yes || 
| [vectorflow](https://github.com/Netflix/vectorflow)                   | Apache 2          | Yes || 

# argv
| library                                                               | license              | gc |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [darg](https://github.com/jasonwhite/darg)                            | Mit                  | Yes || 
| [commander.d](https://github.com/yamadapc/commander.d)                | MIT                  | Yes || 
| [commando](https://github.com/SirTony/commando/)                      | MIT                  | Yes || 
| [argsd](https://github.com/burner/argsd)                              | MIT                  | Yes || 
| [argon](https://github.com/markuslaker/Argon)                         | ISC                  | Yes || 
| [parseopts](https://github.com/mitchgrout/parseopts)                  | Unknown              | Yes || 

# audio
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [Dplug](https://github.com/AuburnSounds/Dplug)                        | Various              | Yes || 
| [Ddsp](https://github.com/abaga129/Ddsp)                              | MIT                  | Yes || 
| [DerelectBass](https://github.com/p0nce/DerelictBASS)                 | Boost                | Yes || 
| [dlang-jack](https://github.com/martinez/dlang-jack)                  | BSL 1                | Yes || 
| [djack](https://github.com/cosenmarco/djack)                          | GPLv3                | Yes || 
| [wasapi](https://github.com/buggins/wasapi)                           | Boost                | Yes || 
| [DerelictFmod](https://github.com/Extrawurst/DerelictFmod)            | MIT                | Yes || 

# compression
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [dcompress](https://github.com/byebye/dcompress)                      | Unknown              | No  || 
| [lz77text](https://github.com/Superstar64/lz77text)                   | Boost                | Yes || 
| [archive](https://github.com/rcythr/archive)                          | BSL 1                | Yes || 

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

# debugging
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

# math
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [scid](https://github.com/DlangScience/scid)                          | Boost                | Yes || 
| [botan-math](https://github.com/etcimon/botan-math)                  | BSD 2                | Yes || 

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


## New libraries and corrections

Submissions of new libraries: I accept submissions (as issues or as pull requests). Please
note that descriptio and last update is optional because a script updates it once a day.

Corrections: if information for a library above is wrong, please send a correction as an
issue, pull request, or email. 

## Thanks

Thanks to [nothings](https://github.com/nothings/single_file_libs) for inspiration.
