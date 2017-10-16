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
    - [math](#math)
  - parsing
  	- [regex](#regex)
    - [JSON](#json)
    - [other serialization](#serialization)
    - [argv argument processing](#argv)
    - [configuration files](#configuration files)
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
    - [unit testing](#tests)
  - other
    - [AI](#ai)
    - [cryptography](#crypto)
    - [randomization](#randomization)
    - [user interface](#user-interface)
    - [miscellaneous](#miscellaneous)
    - [logging](#logging)

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
| [dcv](https://github.com/libmir/dcv)                                  | BSL 1                | Yes |2017-08-11|Computer Vision Library for D Programming Language
| [vectorflow](https://github.com/Netflix/vectorflow)                   | Apache 2             | Yes |2017-09-26|Vectorflow is a minimalist neural network library optimized for sparse data and single machine environments.

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

# configuration files
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [aedi-property-reader](https://github.com/aermicioi/aedi-property-reader)     | BSL 1        | Yes |2017-08-22|Aedi extension, that loads data from multiple sources (environment, xml, json, etc.)
| [configd](https://github.com/LightBender/configd)                     | BSL 1                | Yes |2016-12-08|Key/Value Configuration Library for D
| [libconfig-d](https://github.com/rtbo/libconfig-d)                    | BSD 3                | Yes |2016-10-16|Port of libconfig to the D programming language
| [onyx-config](https://github.com/nykytenko/onyx-config)               | MIT                  | Yes |2017-08-31|Working with configuration data in run-time (D lang)
| [runtimer](https://github.com/chrishalebarnes/runtimer)               | MIT                  | Yes |2016-04-23|Application runtime configuration for applications built in the D programming language.
| [yamkeys](https://github.com/carlor/yamkeys)                          | MIT                  | Yes |2016-04-09|A runtime configuration management utility.

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
| [StringBuffer](https://github.com/burner/StringBuffer)                | LGPL 3               | Yes |2017-05-19|A stack based string buffer that grows into the heap if needed.
| [vebtree](https://bitbucket.org/Sandman8/vebtree)                     | MIT                  | Yes | 2016-Oct-28 |A library for van Emde Boas tree 

# databases
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [basil](https://github.com/senselogic/BASIL)                          | GPLv3                | Yes |2017-10-07|Textual database builder.
| [d2sqlite2](https://github.com/biozic/d2sqlite3)                      | BSL 1                | Yes |2017-07-10|A small wrapper around SQLite for the D programming language
| [database](https://github.com/huntlabs/database)                      | Apache 2             | Yes |2017-10-13|Database abstraction layer for D programing language, support PostgreSQL / MySQL / SQLite.
| [db](https://github.com/viile/db)                                     | Apache 2             | Yes |2017-09-18|Database abstraction layer for D programing language, support PostgreSQL / MySQL / SQLite.
| [dbal](https://github.com/huntlabs/dbal)                              | Apache 2             | Yes |2017-10-10|Database Abstraction Layer for dlang, can construct SQL statements.
| [entity](https://github.com/huntlabs/entity)                          | Apache 2             | Yes |2017-10-12|An object-relational mapping (ORM) framework for dlang's database,  support PostgreSQL / MySQL / SQLite.
| [mondo](https://github.com/2night/mondo)                              | MIT                  | Yes |2017-10-05|D library for MongoDb (over mongo-c-library)
| [MongoSchemaD](https://github.com/WebFreak001/MongoSchemaD)           | MIT                  | Yes |2017-10-04|Support for more structured MongoDB databases
| [postgres-native](https://github.com/Burgos/postgres-native)          | MIT                  | Yes |2017-02-01|Native D postgres client library
| [pgator](https://github.com/DSoftOut/pgator)                          | MIT                  | Yes |2017-10-03|Application server that transforms JSON-RPC and Web REST calls into SQL queries for PostgreSQL
| [sqlite3-d](https://github.com/sasq64/sqlite3-d)                      | MIT                  | Yes |2017-06-14|SQLite3 interface for D
| [sqld](https://github.com/Mihail-K/sqld)                              | MIT                  | Yes |2017-05-04|SQL query construction and relational algebra.
| [tiny-redis](https://github.com/adilbaig/Tiny-Redis)                  | ISC                  | Yes |2017-09-07|Redis driver for D
| [vibe.d.db.postgresql](https://github.com/denizzzka/vibe.d.db.postgresql)| MIT                  | No |2017-10-06|PostgreSQL support for Vibe.d
| [UnofficialDerelictSQLite3](https://github.com/workhorsy/UnofficialDerelictSQLite3) | BSL 1                | Yes |2017-10-15|Dynamic bindings to the SQLite library for the D Programming Language.

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

# logging
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [DLayerLogger](https://github.com/MayurovGeorge/DLayerLogger)         | GPLv3                | Yes |2017-08-06|Layer logger written in D
| [dlogg](https://github.com/NCrashed/dlogg)                            | MIT                  | Yes |2017-03-08|Logging utilities that aimed to be used in highly loaded applications
| [gelf](https://github.com/kaleidicpublic/gelf)                        | BSL 1                | Yes |2017-04-21|The Graylog Extended Log Format (GELF) written in D
| [gelf-d](https://github.com/adilbaig/gelfd)                           | MIT                  | Yes |2017-08-21|Native GELF (Graylog Extended Log Format) protocol for D
| [log](https://github.com/linkrope/log)                                | BSL 1                | Yes |2017-06-20|Simple Logging for D
| [logDefer-D](https://github.com/rfarr/LogDefer-D)                     | ISC                  | Yes |2016-10-19|Log defer inspired logging in D
| [onyx-log](https://github.com/nykytenko/onyx-log)                     | MIT                  | Yes |2017-09-27|The simple, fast, multithreading logging library for D.

# math
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [ArithEval](https://github.com/Dechcaudron/ArithEval)                 | GPLv3                | No  |2016-06-27|A minimal arithmetic expression evaluation library for D
| [botan-math](https://github.com/etcimon/botan-math)                   | BSD 2                | Yes |2016-08-23|Matrix Math for Botan Crypto
| [cblas](https://github.com/DlangScience/cblas)                        | BSL 1                | Yes  |2017-07-06|D BLAS header. Works with OpenBLAS.
| [checkedint](https://github.com/tsbockman/checkedint)                 | BSL 1                | Yes |2017-04-21|D module that provides safer integer math operations and types
| [desmath](https://github.com/dexset/desmath)                          | MIT                  | Yes |2016-01-07|math
| [dstats](https://github.com/DlangScience/dstats)                      | Various              | Yes |2017-08-31|A statistics library for D.
| [gl3n](https://github.com/Dav1dde/gl3n)                               | MIT                  | Yes |2017-08-15|OpenGL Maths for D (not glm for D).
| [linalg](https://github.com/vsn4ik/linalg)                            | MIT                  | Yes  |2017-09-02|Linear algebra for D programming language.
| [lubeck](https://github.com/kaleidicassociates/lubeck)                | BSL 1                | Yes  |2017-06-11|High level linear algebra library for Dlang
| [mir-vectorflow](https://github.com/libmir/vectorflow)                | Apache 2             | Yes |2017-09-26|Mir implementation: Vectorflow is a minimalist neural network library optimized for sparse data and single machine environments.
| [numd](https://github.com/Rob-Rau/numd)                               | MIT                  | No  |2017-09-16|A simple @nogc matrix math library for the D Programming language.
| [numir](https://github.com/libmir/numir)                              | BSL 1                | Yes  |2017-09-29|numpy-like API wrappers of mir
| [mir-glas](https://github.com/libmir/mir-glas)                        | BSL 1                | No   |2017-09-18|[Experimental] LLVM-accelerated Generic Linear Algebra Subprograms
| [scid](https://github.com/DlangScience/scid)                          | Boost                | Yes |2017-07-27|Scientific library for the D programming language
| [vecd](https://github.com/nucular/vecd)                               | GPLv3                | Yes  |2015-09-05|Vector module expanding the vector extensions of D

# network
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# regex
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
|[pattern](https://github.com/Mihail-K/pattern)                         | MIT                  | Yes ||

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
| [dunit](https://github.com/nomad-software/dunit)                      | MIT                  | Yes |2016-10-20|Advanced unit testing toolkit for the D programming language

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
| [mir-cpuid](https://github.com/libmir/mir-cpuid)                      | BSL 1                | Yes |2017-06-24|CPU Identification Routines
| [ip2location](https://github.com/ip2location/ip2location-d)           | LGPL 3               | Yes |2017-01-05|Use IP2Location geolocation database to lookup for accurate visitor location with D Library. It enables the user to find the country, region, city, coordinates, zip code, time zone, ISP, domain name, connection type, area code, weather, MCC, MNC, mobile brand name, elevation and usage type that any IP address or hostname originates from. 
|[miao.string](https://github.com/qqiangwu/miao.string)                 | Boost                | Yes ||
|[natcmp](https://github.com/Herringway/natcmp)                         | BSL 1                | Yes ||
|[stringex-d](https://github.com/katafrakt/stringex-d)                  | MIT                  | Yes ||


## Thanks

Thanks to [nothings](https://github.com/nothings/single_file_libs) for inspiration.
