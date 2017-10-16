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

This list aims to collect libraries of high quality. Unfortunately I don't have time to test all of them exhaustively.

**If any library does not meet expected requirements (bugs, no tests, no documentation, outdated) open an issue**

Once a library is removed the name will be moved to [removed.md](removed.md) with the hope that they will be corrected by original manteiners or forks.


### Other lists

Also you might be interested in other related, but different lists:

- [Awesome D](https://github.com/zhaopuming/awesome-d): A curated list of awesome D frameworks, libraries and software. Inspired by awesome-python. 

### Categories:

  - [Multi purpose libraries](#multi-purpose)
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
| [ae](https://github.com/CyberShadow/ae)                               | MPL 2                | Yes |2017-10-14|D2 library for games, network applications etc.
| [Dlib](https://github.com/gecko0307/dlib)                             | Boost                | No  |2017-10-09|Math, XML, I/O streams, image and audio processing for D
| [iz](https://github.com/BBasile/iz)                                   | Boost                | No  |2017-10-11|my D user library
| [fast](https://github.com/mleise/fast)                                | GPLv3                | No  |2017-08-11|A library for D that aims to provide the fastest possible implementation of some every day routines.
| [jive](https://github.com/krox/jive)                                  | Public Domain        | No  |2017-09-19|Collections library for D with STL-like value-semantics.
| [kiss](https://github.com/huntlabs/kiss)                              | Apache 2             | No  |2017-10-09|A refined core library for D programming language. include aio / timer etc.
| [Ocean](https://github.com/sociomantic-tsunami/ocean)                 | BSD                  | No  |2017-10-13|General purpose, platform-dependant, high-performance library for D
| [phobos](https://github.com/dlang/phobos)                             | Boost                | Yes |2017-10-15|The standard library of the D programming language
| [Tango-D2](https://github.com/SiegeLord/Tango-D2)                     | BSD                  | Yes |2016-04-01|A port of the Tango library to D2
| [tango-rt](https://github.com/sociomantic-tsunami/tangort)            | BSD                  | No  |2017-09-27|Tango D1 runtime library
| [Tanya](https://github.com/caraus-ecms/tanya)                         | MPL 2                | No  |2017-10-14|GC-free, high-performance D library: Containers, networking, metaprogramming, memory management, utilities
| [Thrift-d](https://github.com/dhasenan/thrift-d)                      | Apache 2             | Yes |2017-09-17|Thrift library for the D programming language

# AI
| library                                                               | license              | gc |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [dnnet](https://github.com/henrygouk/dnnet)                           | Mit                  | Yes |2016-07-01|An artificial neural networks library.
| [doll](https://github.com/putyy/doll)                                 | Proprietary          | Yes |2017-10-14|D Optimization Library for Learning
| [vectorflow](https://github.com/Netflix/vectorflow)                   | Apache 2          | Yes |2017-09-26|Vectorflow is a minimalist neural network library optimized for sparse data and single machine environments.

# argv
| library                                                               | license              | gc |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [argsd](https://github.com/burner/argsd)                              | MIT                  | Yes |2017-09-13|A command line and config file parser for DLang
| [argon](https://github.com/markuslaker/Argon)                         | ISC                  | Yes |2017-02-20|A processor for command-line arguments, an alternative to Getopt, written in D
| [commander.d](https://github.com/yamadapc/commander.d)                | MIT                  | Yes |2016-04-11|Command-line interfaces in D made easy. Easy command-line parsing based in commander.js.
| [commando](https://github.com/SirTony/commando/)                      | MIT                  | Yes |2017-01-04|A more robust command line argument parser for D.
| [darg](https://github.com/jasonwhite/darg)                            | Mit                  | Yes |2017-03-21|Robust command line argument parsing for D.
| [parseopts](https://github.com/mitchgrout/parseopts)                  | Unknown              | Yes |2017-02-15|Basic command-line options parser written in D

# audio
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [Ddsp](https://github.com/abaga129/Ddsp)                              | MIT                  | Yes |2017-10-15|A library for Digital Signal Processing in D with a focus on audio
| [Dplug](https://github.com/AuburnSounds/Dplug)                        | Various              | Yes |2017-10-15|Dplug is a library for creating native audio plugins (VST / AU) as simply as possible.
| [dlang-jack](https://github.com/martinez/dlang-jack)                  | BSL 1                | Yes |2016-08-11|Idiomatic D API binding for the JACK Audio Connection Kit
| [DerelictFmod](https://github.com/Extrawurst/DerelictFmod)            | MIT                | Yes |2017-09-20|Dynamic bindings of the fmod sound library in the D programming language
| [djack](https://github.com/cosenmarco/djack)                          | GPLv3                | Yes |2014-07-13|D interface for JACK audio server
| [DerelectBass](https://github.com/p0nce/DerelictBASS)                 | Boost                | Yes |2017-06-08|DerelictBASS is a dynamic binding to the audio library BASS.
| [wasapi](https://github.com/buggins/wasapi)                           | Boost                | Yes |2017-02-10|D bindings of Windows Core Audio interfaces: Core Audio interfaces: MMDevice, WASAPI, EndpointVolume API

# compression
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [archive](https://github.com/rcythr/archive)                          | BSL 1                | Yes |2017-05-06|An archive library that supports zip, tar, and targz written entirely in D (with underlying gz implementation from zlib).
| [dcompress](https://github.com/byebye/dcompress)                      | Unknown              | No  |2017-06-02|A compression library for D programming language.
| [lz77text](https://github.com/Superstar64/lz77text)                   | Boost                | Yes |2016-08-01|implementation of the lz77 compression algorithm with text headers

# concurrency
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [jin.go](https://github.com/nin-jin/go.d)                             | Public Domain        | Yes |2017-01-07|Wait free thread communication
| [workermanager](https://github.com/alphaKAI/workermanager)            | Unknown              | Yes |2017-03-31|Multi-thread based asynchronized worker manager

# crypto
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [botan](https://github.com/etcimon/botan)                             | Unknown/Closed       | Yes |2017-07-12|Block & stream ciphers, public key crypto, hashing, KDF, MAC, PKCS, TLS, ASN.1, BER/DER, etc.

# data structures
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [aammm](https://github.com/arexeu/aammm)                              | BSL 1                | No  |2015-10-11|Associative arrays with manual memory management
| [ArrayList](https://github.com/0xEAB/arraylist)                       | Public Domain        | Yes |2017-07-27|A simple array-backed list, written in D.
| [containers](https://github.com/economicmodeling/containers)          | MIT                  | No  |2017-10-03|Containers backed by std.experimental.allocator
| [darray](https://github.com/burner/darray)                            | LGPL 3               | Yes |2017-09-20|A double ended array for the D Programming Language
| [Dgraph](https://github.com/WebDrake/Dgraph)                          | GPLv3                | Yes  |2017-03-24|Graph library written in D.
| [dhtnode](https://github.com/sociomantic-tsunami/dhtnode)             | MIT                  | No  |2017-10-13|Distributed hash-table node
| [hash](https://github.com/Mihail-K/hash)                              | MIT                  | Yes |2016-06-07|A Hash datatype for key => value pairs.
| [JudyD](https://github.com/rfarr/JudyD)                               | ISC                  | No  |2016-07-27|D language bindings for Judy Arrays
| [memutils](https://github.com/etcimon/memutils)                       | MIT                  | No  |2017-02-13|Overhead allocators, allocator-aware containers and lifetime management for D objects
| [mir-algorithm](https://github.com/libmir/mir-algorithm)              | BSL 1                | No  |2017-10-15|Dlang core library for math, finance and a home for Dlang multidimensional array package - ndslice
| [std.rcstring](https://github.com/burner/std.rcstring)                | Boost                | No  |2016-09-29|A reference counted string implementation for D's build in string construct.
| [vebtree](https://bitbucket.org/Sandman8/vebtree)                     | MIT                  | Yes | 2016-Oct-28 |A library for van Emde Boas tree 

# databases
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [basil](https://github.com/senselogic/BASIL)                          | GPLv3                | Yes || 
| [d2sqlite2](https://github.com/biozic/d2sqlite3)                      | BSL 1                | Yes || 
| [database](https://github.com/huntlabs/database)                      | Apache 2             | Yes || 
| [db](https://github.com/viile/db)                                     | Apache 2             | Yes || 
| [dbal](https://github.com/huntlabs/dbal)                              | Apache 2             | Yes || 
| [entity](https://github.com/huntlabs/entity)                          | Apache 2             | Yes || 
| [mondo](https://github.com/2night/mondo)                              | MIT                  | Yes || 
| [MongoSchemaD](https://github.com/WebFreak001/MongoSchemaD)           | MIT                  | Yes || 
| [postgres-native](https://github.com/Burgos/postgres-native)          | MIT                  | Yes || 
| [pgator](https://github.com/DSoftOut/pgator)                          | MIT                  | Yes || 
| [sqlite3-d](https://github.com/sasq64/sqlite3-d)                      | MIT                  | Yes || 
| [tiny-redis](https://github.com/adilbaig/Tiny-Redis)                  | ISC                  | Yes || 
| [vibe.d.db.postgresql](https://github.com/denizzzka/vibe.d.db.postgresql)| MIT                  | No || 
| [UnofficialDerelictSQLite3](https://github.com/workhorsy/UnofficialDerelictSQLite3) | BSL 1                | Yes || 

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
| [ArithEval](https://github.com/Dechcaudron/ArithEval)                 | GPLv3                | No  ||
| [botan-math](https://github.com/etcimon/botan-math)                   | BSD 2                | Yes |2016-08-23|Matrix Math for Botan Crypto
| [checkedint](https://github.com/tsbockman/checkedint)                 | BSL 1                | Yes ||
| [desmath](https://github.com/dexset/desmath)                          | MIT                  | Yes ||
| [gl3n](https://github.com/Dav1dde/gl3n)                               | MIT                  | Yes ||
| [numd](https://github.com/Rob-Rau/numd)                               | MIT                  | No  ||
| [scid](https://github.com/DlangScience/scid)                          | Boost                | Yes |2017-07-27|Scientific library for the D programming language

# network
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# serialization
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [msgpack-ll](https://github.com/jpf91/msgpack-ll)                     | BSL 1                | No  |2017-04-18|A low level @nogc, nothrow, @safe, pure and betterC compatible msgpack.org[D] library

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
| [unit-threaded](https://github.com/atilaneves/unit-threaded)          | BSD                  | Yes |2017-09-24|Advanced unit test framework for D (includes unittest blocks)

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
| [ip2location](https://github.com/ip2location/ip2location-d)           | LGPL 3               | Yes || 


## Thanks

Thanks to [nothings](https://github.com/nothings/single_file_libs) for inspiration.
