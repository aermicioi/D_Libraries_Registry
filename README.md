# Note

This project was just a quick draft that I used to understand if there is interest and possibilities for a better reorganization of D libraries.
At the moment the project is abandoned while I am working on a dub-registry mirror that implements more features.

# D language libraries

I want to build a comprehensive list of D language libraries to be used as a reference.

This collection has the intent to help developers find a suitable library for the work and decrease the amount of effort in writing new software.

For any question or contribution, reache me via github pull requests and issues.

## New libraries and corrections

Submissions of new libraries: I accept submissions (as issues or as pull requests). Please
note that description and last update is optional (for libraries that are hosted on github)
because a script updates it once a day.

Corrections: if information for a library above is wrong, please send a correction as an
issue, pull request, or email. 

Categories: I am open to discussions on the current categorization method. Reach to me on github.

## Quality

This list aims to collect libraries of high quality. Unfortunately I don't have time to test all of them exhaustively.

**If any library does not meet expected requirements (bugs, no tests, no documentation, outdated) open an issue**

Once a library is removed the name will be moved to [removed.md](removed.md) with the hope that they will be corrected by original manteiners or forks.


### Other lists

Also you might be interested in other related, but different lists:

- [Awesome D](https://github.com/zhaopuming/awesome-d): A curated list of awesome D frameworks, libraries and software. Inspired by awesome-python.||
- [Dub Registry](http://code.dlang.org/): The package registry used by DUB.||

### Categories:

  - [Multi purpose libraries](#multi-purpose)
  - [Frameworks](#frameworks)
  - general purpose
    - [data structures](#data-structures)
    - [scripting](#scripting)
    - [hashing](#hashing)
    - [concurrency](#concurrency)
    - [databases](#databases)
    - [IO](#IO)
  - mathematics
    - [math](#math)
  - parsing
  	- [regex](#regex)
    - [JSON](#json)
    - [rpc and serialization](#serialization-rpc)
    - [argv argument processing](#argv)
    - [configuration files](#configuration files)
    - [other parsing](#parsing)
  - graphics
    - [graphics](#graphics)
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
  - [game engines and frameworks](#games)
  - other
    - [AI](#ai)
    - [cryptography](#crypto)
    - [randomization](#randomization)
    - [user interface](#user-interface)
    - [miscellaneous](#miscellaneous)
    - [logging](#logging)
    - [build systems](#build-systems)
    - [time and dates](#time-dates)

# Multi-purpose
| library                                                               | license              | gc |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [ae](https://github.com/CyberShadow/ae)                               | MPL 2                | Yes |2017-12-29|D2 library for games, network applications etc.
| [Dlib](https://github.com/gecko0307/dlib)                             | Boost                | No  |2018-01-04|Math, XML, I/O streams, image and audio processing for D
| [iz](https://github.com/BBasile/iz)                                   | Boost                | No  |2018-01-04|nogc: streams, containers; rtti: properties, serializer, binder; reasonable and crazy things;
| [fast](https://github.com/mleise/fast)                                | GPLv3                | No  |2017-12-31|A library for D that aims to provide the fastest possible implementation of some every day routines.
| [mach.d](https://github.com/pineapplemachine/mach.d)                  | Zlib                 | Yes |2017-10-31|Library for the D programming language.
| [jive](https://github.com/krox/jive)                                  | Public Domain        | No  |2017-09-19|Collections library for D with STL-like value-semantics.
| [kiss](https://github.com/huntlabs/kiss)                              | Apache 2             | No  |2017-12-27|A refined core library for D programming language. include aio / timer etc.
| [Ocean](https://github.com/sociomantic-tsunami/ocean)                 | BSD                  | No  |2018-01-04|General purpose, platform-dependant, high-performance library for D
| [phobos](https://github.com/dlang/phobos)                             | Boost                | Yes |2018-01-04|The standard library of the D programming language
| [Tango-D2](https://github.com/SiegeLord/Tango-D2)                     | BSD                  | Yes |2016-04-01|A port of the Tango library to D2
| [tango-rt](https://github.com/sociomantic-tsunami/tangort)            | BSD                  | No  |2018-01-04|Tango D1 runtime library
| [Tanya](https://github.com/caraus-ecms/tanya)                         | MPL 2                | No  |2018-01-04|GC-free, high-performance D library: Containers, networking, metaprogramming, memory management, utilities
| [Thrift-d](https://github.com/dhasenan/thrift-d)                      | Apache 2             | Yes |2017-09-17|Thrift library for the D programming language

# frameworks
| library                                                               | license              | gc |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [big.d](https://github.com/LLC-CERERIS/big.d)                         | MIT                  | Yes |2017-10-26|MVC Web framework for D
| [Cmsed](https://github.com/rikkimax/Cmsed)                            | MIT                  | Yes |2015-01-23|A component library for Vibe that functions as a CMS.
| [Diamond](https://github.com/DiamondMVC/Diamond)                      | MIT                  | Yes |2017-12-22|Diamond is a powerful MVC / Template Framework written in the D Programming Language, inspired by ASP.NET using vibe.d as backend.
| [hunt](https://github.com/huntlabs/hunt)                              | Apache 2             | Yes |2017-12-08|A high performance full-stack Web framework written in dlang.
| [Ocean](https://github.com/sociomantic-tsunami/swarm)                 | BSL 1                | No  |2017-12-28|Asynchronous client/node framework library
| [Orwell](https://github.com/mattremmel/Orwell)                        | proprietary          | Yes |2017-08-16|A security framework and proxy for analyzing network traffic and web applications.
| [turtle](https://github.com/sociomantic-tsunami/turtle)               | BSL                  | Yes |2017-12-28|Black box application testing library/framework
| [orm](https://github.com/viile/orm)                                   | Apache 2                  | Yes |2017-12-23|An object-relational mapping (ORM) framework for dlang's database, support PostgreSQL / MySQL / SQLite.
| [collie](https://github.com/huntlabs/collie)                          | Apache 2                  | Yes |2017-09-13|An asynchronous event-driven network framework written in D.
| [endovena](https://github.com/o3o/endovena)                           | Boost                  | Yes |2017-09-08|Simple dependency injection framework for D
| [dich](https://github.com/LLC-CERERIS/dich)                           |  MIT                  | Yes |2017-08-29|Simple dependency injection framework for D. Based on endovena similar work.
| [poodinis](https://github.com/mbierlee/poodinis)                       |  MIT                  | Yes |2018-01-04|A dependency injection framework for D with support for autowiring.
| [dchem](https://github.com/fawzi/dchem)                               |  ?                  | Yes |2017-07-25|a chemistry simulation, and electrostatic embedding framework in D
| [caraus](https://github.com/caraus-ecms/caraus)                       |  MPL 2                  | Yes |2017-01-11|Web framework for the D programming language in development
| [yu](https://github.com/dushibaiyu/yu)                                | Apache 2             | Yes |2017-08-16|Dlang‘s Toolkit

# AI
| library                                                               | license              | gc |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [dcv](https://github.com/libmir/dcv)                                  | BSL 1                | Yes |2017-12-07|Computer Vision Library for D Programming Language
| [dnnet](https://github.com/henrygouk/dnnet)                           | Mit                  | Yes |2017-11-05|An artificial neural networks library.
| [doll](https://github.com/putyy/doll)                                 | Proprietary          | Yes |2017-10-14|D Optimization Library for Learning
| [dopt](https://github.com/henrygouk/dopt)                             | BSD 3 clause         | Yes |2018-01-02|A numerical optimisation and deep learning framework for D.
| [neuralnet](https://github.com/bloodythorn/neuralNet)                 | MIT                  | Yes |2017-05-15|A neural network implemented in D using Back Propagation and Momentum.
| [vectorflow](https://github.com/Netflix/vectorflow)                   | Apache 2             | Yes |2017-11-23|Vectorflow is a minimalist neural network library optimized for sparse data and single machine environments.

# argv
| library                                                               | license              | gc |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [argsd](https://github.com/burner/argsd)                              | MIT                  | Yes |2017-12-27|A command line and config file parser for DLang
| [argon](https://github.com/markuslaker/Argon)                         | ISC                  | Yes |2017-11-10|A processor for command-line arguments, an alternative to Getopt, written in D
| [commander.d](https://github.com/yamadapc/commander.d)                | MIT                  | Yes |2016-04-11|Command-line interfaces in D made easy. Easy command-line parsing based in commander.js.
| [commando](https://github.com/SirTony/commando/)                      | MIT                  | Yes |2017-01-04|A more robust command line argument parser for D.
| [ctoptions](https://github.com/Soulsbane/ctoptions)                   | Copyright            | Yes |2018-01-03|A D Programming Language library for handling a key/value config file format at compile-time.
| [darg](https://github.com/jasonwhite/darg)                            | Mit                  | Yes |2017-03-21|Robust command line argument parsing for D.
| [parseopts](https://github.com/mitchgrout/parseopts)                  | Unknown              | Yes |2017-02-15|Basic command-line options parser written in D

# audio
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [Ddsp](https://github.com/abaga129/Ddsp)                              | MIT                  | Yes |2017-12-23|A library for Digital Signal Processing in D with a focus on audio
| [Dplug](https://github.com/AuburnSounds/Dplug)                        | Various              | Yes |2018-01-04|Dplug is a library for creating native audio plugins (VST / AU / AAX) as simply as possible.
| [dlang-jack](https://github.com/martinez/dlang-jack)                  | BSL 1                | Yes |2016-08-11|Idiomatic D API binding for the JACK Audio Connection Kit
| [DerelictFmod](https://github.com/Extrawurst/DerelictFmod)            | MIT                | Yes |2017-11-20|Dynamic bindings of the fmod sound library in the D programming language
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
| [cheetah](https://github.com/bausshf/cheetah)                        | MIT                  | Yes |2017-05-16|A high performance event-based tcp server socket library based on vibe.d
| [workermanager](https://github.com/alphaKAI/workermanager)            | Unknown              | Yes |2017-03-31|Multi-thread based asynchronized worker manager
| [eventcore](https://github.com/vibe-d/eventcore)                      | MIT                  | No  |2017-12-20|High performance proactor event loop abstraction library
| [libasync](https://github.com/etcimon/libasync)                       | MIT                  | Yes  |2017-12-13|Cross-platform event loop library of asynchronous objects
| [EventSystem](https://github.com/WebFreak001/EventSystem)             | Unlicense            | Yes  |2017-04-11|Tiny event system in D using delegates
| [eventmanager](https://github.com/AndrewSChapman/eventmanager)        | BSL 1                | Yes  |2017-06-30|Written for the "D" programming language, this library implements a variant of the pub/sub pattern, using events, an event list and event dispatchers
| [jin.go](https://github.com/nin-jin/go.d)                             | Public Domain        | Yes |2017-01-07|Wait free thread communication
| [subscribed](https://github.com/v--/subscribed)                       | BSL 1                | Yes  |2017-07-10|A minimalistic library providing eventing-related structures.

# configuration files
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [aedi-property-reader](https://github.com/aermicioi/aedi-property-reader)     | BSL 1        | Yes |2017-08-22|Aedi extension, that loads data from multiple sources (environment, xml, json, etc.)
| [configd](https://github.com/LightBender/configd)                     | BSL 1                | Yes |2016-12-08|Key/Value Configuration Library for D
| [inilike](https://github.com/FreeSlave/inilike)                       | BSL 1             | Yes |2017-10-23|D library for parsing .ini-like files used in Freedesktop systems
| [libconfig-d](https://github.com/rtbo/libconfig-d)                    | BSD 3                | Yes |2016-10-16|Port of libconfig to the D programming language
| [onyx-config](https://github.com/nykytenko/onyx-config)               | MIT                  | Yes |2017-12-19|Working with configuration data in run-time (D lang)
| [runtimer](https://github.com/chrishalebarnes/runtimer)               | MIT                  | Yes |2016-04-23|Application runtime configuration for applications built in the D programming language.
| [yamkeys](https://github.com/carlor/yamkeys)                          | MIT                  | Yes |2016-04-09|A runtime configuration management utility.

# crypto
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [botan](https://github.com/etcimon/botan)                             | Unknown/Closed       | Yes |2017-11-29|Block & stream ciphers, public key crypto, hashing, KDF, MAC, PKCS, TLS, ASN.1, BER/DER, etc.
| [cryption](https://github.com/shove70/cryption)                       | Apache 2             | Yes |2018-01-02|A D Library of encryption, decryption, encode, hash, and message digital signatures.

# data structures
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [aammm](https://github.com/arexeu/aammm)                              | BSL 1                | No  |2015-10-11|Associative arrays with manual memory management
| [ArrayList](https://github.com/0xEAB/arraylist)                       | Public Domain        | Yes |2017-07-27|A simple array-backed list, written in D.
| [containers](https://github.com/economicmodeling/containers)          | MIT                  | No  |2018-01-04|Containers backed by std.experimental.allocator
| [darray](https://github.com/burner/darray)                            | LGPL 3               | Yes |2017-09-20|A double ended array for the D Programming Language
| [Dgraph](https://github.com/WebDrake/Dgraph)                          | GPLv3                | Yes  |2017-03-24|Graph library written in D.
| [dhtnode](https://github.com/sociomantic-tsunami/dhtnode)             | MIT                  | No  |2018-01-04|Distributed hash-table node
| [hash](https://github.com/Mihail-K/hash)                              | MIT                  | Yes |2016-06-07|A Hash datatype for key => value pairs.
| [JudyD](https://github.com/rfarr/JudyD)                               | ISC                  | No  |2016-07-27|D language bindings for Judy Arrays
| [memutils](https://github.com/etcimon/memutils)                       | MIT                  | No  |2017-10-18|Overhead allocators, allocator-aware containers and lifetime management for D objects
| [mir-algorithm](https://github.com/libmir/mir-algorithm)              | BSL 1                | No  |2018-01-04|Dlang core library for math, finance and a home for Dlang multidimensional array package - ndslice
| [std.rcstring](https://github.com/burner/std.rcstring)                | Boost                | No  |2016-09-29|A reference counted string implementation for D's build in string construct.
| [StringBuffer](https://github.com/burner/StringBuffer)                | LGPL 3               | Yes |2017-05-19|A stack based string buffer that grows into the heap if needed.
| [vebtree](https://bitbucket.org/Sandman8/vebtree)                     | MIT                  | Yes ||

# databases
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [basil](https://github.com/senselogic/BASIL)                          | GPLv3                | Yes |2017-10-07|Textual database builder.
| [d2sqlite3](https://github.com/biozic/d2sqlite3)                      | BSL 1                | Yes |2017-11-25|A small wrapper around SQLite for the D programming language
| [database](https://github.com/huntlabs/database)                      | Apache 2             | Yes |2018-01-04|Database abstraction layer for D programing language, support PostgreSQL / MySQL / SQLite.
| [db](https://github.com/viile/db)                                     | Apache 2             | Yes |2017-12-23|Database abstraction layer for D programing language, support PostgreSQL / MySQL / SQLite.
| [dbal](https://github.com/huntlabs/dbal)                              | Apache 2             | Yes |2017-12-20|Database Abstraction Layer for dlang, can construct SQL statements.
| [Dvorm](https://github.com/rikkimax/Dvorm)                            | MIT                  | Yes |2016-05-12|An orm for D with Vibe support.
| [entity](https://github.com/huntlabs/entity)                          | Apache 2             | Yes |2018-01-04|An object-relational mapping (ORM) framework for dlang's database,  support PostgreSQL / MySQL / SQLite.
| [mysql-native](https://github.com/mysql-d/mysql-native)               | Boost                | Tes |2017-12-15|Native D client driver for MySQL/MariaDB, works with or without Vibe.d
| [mondo](https://github.com/2night/mondo)                              | MIT                  | Yes |2017-10-05|D library for MongoDb (over mongo-c-library)
| [MongoSchemaD](https://github.com/WebFreak001/MongoSchemaD)           | MIT                  | Yes |2017-10-04|Support for more structured MongoDB databases
| [postgres-native](https://github.com/Burgos/postgres-native)          | MIT                  | Yes |2017-02-01|Native D postgres client library
| [pgator](https://github.com/DSoftOut/pgator)                          | MIT                  | Yes |2017-12-31|Application server that transforms JSON-RPC and Web REST calls into SQL queries for PostgreSQL
| [sqlite3-d](https://github.com/sasq64/sqlite3-d)                      | MIT                  | Yes |2017-06-14|SQLite3 interface for D
| [sqld](https://github.com/Mihail-K/sqld)                              | MIT                  | Yes |2017-05-04|SQL query construction and relational algebra.
| [tiny-redis](https://github.com/adilbaig/Tiny-Redis)                  | ISC                  | Yes |2017-12-24|Redis driver for D
| [vibe.d.db.postgresql](https://github.com/denizzzka/vibe.d.db.postgresql)| MIT                  | No |2017-10-06|PostgreSQL support for Vibe.d
| [UnofficialDerelictSQLite3](https://github.com/workhorsy/UnofficialDerelictSQLite3) | BSL 1                | Yes |2017-10-15|Dynamic bindings to the SQLite library for the D Programming Language.

# debugging
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# files & filenames
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [d-glob](https://github.com/workhorsy/d-glob)                         | BSL 1                | Yes |2017-09-28|Search file systems with glob patterns using the D programming language
| [lnk](https://github.com/FreeSlave/lnk)                         | BSL 1                | Yes |2017-02-03|D library for parsing .lnk files
| [FSWatch](https://github.com/WebFreak001/FSWatch)                     | BSL 1                | Yes |2017-10-21|A cross-platform folder & file watching library using win32, inotify or std.file
| [proped](https://github.com/milofon/proped)                           | BSD                  | Yes |2017-08-25|A library for reading properties files
| [trashcan](https://github.com/FreeSlave/trashcan)                     | BSL 1                | Yes |2017-03-28|Move files to trash can in D programming language

# games
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [dagon](https://github.com/gecko0307/dagon)                           |  BSL 1               | Yes |2017-12-07|3D game engine for D
| [DAllegro](https://github.com/SiegeLord/DAllegro5)                    | Zlib                 | Yes |2016-10-02|D binding to the Allegro5 game development library
| [dash](https://github.com/Circular-Studios/Dash)                      | MIT                  | Yes |2016-02-08|A free and open 3D game engine written in D.
| [DSFML](https://github.com/Jebbs/DSFML)                               | Zlib                 | Yes |2017-10-24|DSFML is a D binding of SFML 
| [dvpe](https://github.com/kuviman/dvpe)                               |  Unknown             | Yes |2017-01-12|2D Game Engine for the D Programming Language
| [GFM](https://github.com/d-gamedev-team/gfm)                          | Unlicense            | Yes |2017-12-25|D gamedev toolkit.
| [orb](https://github.com/claudemr/orb)                                |  GPLv3               | Yes |2017-08-11|3D-voxel engine
| [RaiderEngine](https://github.com/Raiderium/RaiderEngine)             |  MIT                 | Yes |2017-12-24|A small game engine.
| [tharsis.prof](https://github.com/kiith-sa/tharsis.prof)              |  ?                   | Yes |2016-11-01|Frame profiler library for game development in D.
| [unecht](https://github.com/Extrawurst/unecht)                        |  MIT                 | Yes |2017-06-11|Game Engine Framework for the D programming language
| [voxelman](https://github.com/MrSmith33/voxelman)                     |  BSL 1               | Yes |2018-01-01|Plugin-based client-server voxel game engine written in D language

# graphics
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [DerelictGL3](https://github.com/DerelictOrg/DerelictGL3)             | Boost                | Yes |2017-12-04|A dynamic binding to OpenGL for the D Programming Language.
| [DerelictLibUI](https://github.com/Extrawurst/DerelictLibui)          | MIT                  | Yes |2016-08-01|Dynamic Binding for libui (https://github.com/andlabs/libui) in D
| [dgfxbase](https://github.com/bioglaze/dgfxbase)                      | MIT                  | Yes |2017-11-06|OpenGL 4.5 basecode using D language and Derelict
| [dgui](https://github.com/o3o/dguihub)                                | Boost                | Yes |2017-08-21|D Win32 Graphic Library
| [dlangui](https://github.com/buggins/dlangui)                         | BSL 1                | Yes |2017-12-19|Cross Platform GUI for D programming language
| [dwt](https://github.com/d-widget-toolkit/dwt)                        | EPL                  | Yes |2018-01-04|A library for creating cross-platform GUI applications.
| [dqml](https://github.com/filcuc/dqml)                                | LGPLv3               | Yes |2017-07-29|Qt Qml bindings for the D programming language
| [GtkD](https://github.com/gtkd-developers/GtkD) 	                    | LGPLv3               | Yes |2018-01-02|GtkD is a D binding and OO wrapper of GTK+
| [gtkui](https://github.com/deviator/gtkui)                            | MIT                  | Yes |2017-10-22|aux lib for using with glade ui builder
| [glamour](https://github.com/Dav1dde/glamour)                         | MIT                  | Yes |2016-10-05|OpenGL wrapper for the D programming language.
| [nice-curses](https://github.com/mpevnev/nice-curses)                 | BSL                  | Yes |2017-09-25|A ncurses wrapper and an UI library for D programming language
| [opengl-d](https://github.com/WebFreak001/opengl-d)                   | Boost                | Yes |2017-06-05|dynamic & static generated OpenGL bindings for D using ogl_gen
| [pdcurses-d](https://github.com/unleashy/pdcurses-d)                   | MIT                | Yes |2017-09-09|D bindings for pdcurses
| [poison-ui](https://github.com/PoisonEngine/poison-ui)                | MIT                  | Yes |2016-12-10|A cross-platform desktop/mobile UI engine written in D using dsfml
| [QTE5](https://github.com/MGWL/QtE5)                                  | GPLv3                | Yes |2017-12-31|It is wrapper Qt 5 for programming language D. (http://www.dlang.org)
| [Sciter-Dport](https://github.com/sciter-sdk/Sciter-Dport)            | MIT                  | Yes |2017-06-12|Port of Sciter headers for the D language
| [tkd](https://github.com/nomad-software/tkd)                          | MIT                  | Yes |2017-05-28|GUI toolkit for the D programming language based on Tcl/Tk

# hardware
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [nel-d](https://github.com/Bananattack/nel-d)                         | MIT                  | ? |2013-03-07|nel is a compiler for a low-level assembly programming language for developing on the NES hardware.

# hashing
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [sha1ct](https://github.com/WebFreak001/sha1ct)                       | Unlicense            | Yes |2017-06-14|sha1 hashing & uuid algorithm that works at compile time

# images
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [daffodil](https://github.com/BenjaminSchaaf/daffodil)                | MIT                | Yes |2017-04-22|A image processing library for D
| [img-d](https://github.com/rtbo/img-d)                                | MIT                | Yes |2017-01-13|A set of bindings to manipulate images with the D programming language.
| [imageformats](https://github.com/lgvz/imageformats)                   | Boost                | Yes |2017-10-31|Image loading/saving for D
| [rip](https://github.com/LightHouseSoftware/rip)                      | GPLv3                | Yes |2017-09-29|Raster and Image Processor

# IO
| library                                                               | license              | GC  |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [io](https://github.com/MartinNowak/io) 							    | BSL 1                | No  |2018-01-04|Core I/O functionality
| [iopipe](https://github.com/schveiguy/iopipe)					        | BSL 1                | Yes |2018-01-04|D language library for modular io

# logging
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [DLayerLogger](https://github.com/MayurovGeorge/DLayerLogger)         | GPLv3                | Yes |2017-08-06|Layer logger written in D
| [dlogg](https://github.com/NCrashed/dlogg)                            | MIT                  | Yes |2017-11-10|Logging utilities that aimed to be used in highly loaded applications
| [gelf](https://github.com/kaleidicpublic/gelf)                        | BSL 1                | Yes |2017-04-21|The Graylog Extended Log Format (GELF) written in D
| [gelf-d](https://github.com/adilbaig/gelfd)                           | MIT                  | Yes |2017-08-21|Native GELF (Graylog Extended Log Format) protocol for D
| [log](https://github.com/linkrope/log)                                | BSL 1                | Yes |2017-11-07|Simple Logging for D
| [logDefer-D](https://github.com/rfarr/LogDefer-D)                     | ISC                  | Yes |2016-10-19|Log defer inspired logging in D
| [onyx-log](https://github.com/nykytenko/onyx-log)                     | MIT                  | Yes |2017-12-19|The simple, fast, multithreading logging library for D.

# math
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [ArithEval](https://github.com/Dechcaudron/ArithEval)                 | GPLv3                | No  |2017-12-30|A minimal arithmetic expression evaluation library for D
| [botan-math](https://github.com/etcimon/botan-math)                   | BSD 2                | Yes |2017-10-18|Matrix Math for Botan Crypto
| [cblas](https://github.com/DlangScience/cblas)                        | BSL 1                | Yes  |2017-10-28|D BLAS header. Works with OpenBLAS.
| [checkedint](https://github.com/tsbockman/checkedint)                 | BSL 1                | Yes |2017-04-21|D module that provides safer integer math operations and types
| [desmath](https://github.com/dexset/desmath)                          | MIT                  | Yes |2016-01-07|math
| [dstats](https://github.com/DlangScience/dstats)                      | Various              | Yes |2017-10-28|A statistics library for D.
| [gl3n](https://github.com/Dav1dde/gl3n)                               | MIT                  | Yes |2017-11-07|OpenGL Maths for D (not glm for D).
| [linalg](https://github.com/vsn4ik/linalg)                            | MIT                  | Yes  |2017-09-02|Linear algebra for D programming language.
| [lubeck](https://github.com/kaleidicassociates/lubeck)                | BSL 1                | Yes  |2017-10-27|High level linear algebra library for Dlang
| [mir-vectorflow](https://github.com/libmir/vectorflow)                | Apache 2             | Yes |2017-09-26|Mir implementation: Vectorflow is a minimalist neural network library optimized for sparse data and single machine environments.
| [numd](https://github.com/Rob-Rau/numd)                               | MIT                  | No  |2017-09-16|A simple @nogc matrix math library for the D Programming language.
| [numir](https://github.com/libmir/numir)                              | BSL 1                | Yes  |2017-12-09|numpy-like API wrappers of mir
| [mir-glas](https://github.com/libmir/mir-glas)                        | BSL 1                | No   |2017-12-02|[Experimental] LLVM-accelerated Generic Linear Algebra Subprograms
| [scid](https://github.com/DlangScience/scid)                          | Boost                | Yes |2017-07-27|Scientific library for the D programming language
| [vecd](https://github.com/nucular/vecd)                               | GPLv3                | Yes  |2015-09-05|Vector module expanding the vector extensions of D

# network
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [dlang-requests](https://github.com/ikod/dlang-requests)              | BSL 1                | Yes |2017-12-11|dlang http client library inspired by python-requests
| [libhttp2](https://github.com/etcimon/libhttp2)                       | MIT                  | Yes |2017-10-18|HTTP/2 library in D, translated from nghttp2
| [nanomsg-wrapper](https://github.com/kaleidicassociates/nanomsg-wrapper)               | Boost                | No |2017-11-14|d-lang bindings for nanomsg
| [nbuff](https://github.com/ikod/nbuff)                                | BSL 1                | Yes |2017-10-17|network buffer
| [netkit](https://github.com/huntlabs/netkit)                        | Apache 2                | Yes |2017-08-19|This library contains tcp / http / http2 / websocket servers and clients.
| [networkD](https://github.com/Nafees10/networkD)                      | MIT                  | Yes |2017-10-28|A simple and basic networking library based on `std.socket` for D Language
| [requests](https://github.com/burner/requests)                        | GPLv3                | No |2017-07-31|A lightweight vibe.d (dlang) requestHttp wrapper to execute multiple http requests in parallel


# regex
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [pattern](https://github.com/Mihail-K/pattern)                         | MIT                  | Yes |2016-04-10|Templated types for string pattern matching and lexers.

# serialization-rpc
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [buffer](https://github.com/shove70/buffer)                          |  MIT                  | Yes |2018-01-02|protocol buffer & rpc
| [cerealed](https://github.com/atilaneves/cerealed)                    | BSD                  | Yes |2017-12-07|Powerful binary serialisation library for D
| [dproto](https://github.com/msoucy/dproto)                            | BSL 1.0              | Yes |2017-08-31|D Protocol Buffer mixins to create structures at compile time
| [hprose](https://github.com/hprose/hprose-d)                          |  MIT                 | Yes |2016-11-14|Hprose for Dlang
| [experimental.xtml](https://github.com/lodo1995/experimental.xml)      | Boost                 | No |2017-07-27|A replacement of Phobos std.xml
| [msgpack-ll](https://github.com/jpf91/msgpack-ll)                     | BSL 1                | No  |2017-04-18|A low level @nogc, nothrow, @safe, pure and betterC compatible msgpack.org[D] library
| [orange](https://github.com/jacob-carlborg/orange)                    | BSL 1                | Yes |2017-10-05|A serialization library for the D programming language.
| [kiss-rpc](https://github.com/huntlabs/kiss-rpc)                          |  Apache 2                 | Yes |2017-11-08|Ultra high performance RPC
| [viberpc-channel](https://github.com/jpf91/vibe-rpcchannel)          |  BSL 1                 | Yes |2017-04-17|A RPC TCP/Noise server and client for vibe.D
| [xmlrpcc-d](https://github.com/o3o/xmlrpcc-d)                          |  Boost                  | Yes |2017-02-23|XML-RPC client for D Programming Language

# json
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [asdf](https://github.com/tamediadigital/asdf)                        | BSL 1               | Yes |2018-01-03|worlds fastest json parser geared towards processing huge amounts of JSON
| [fastjwt](https://github.com/burner/fastjwt)                          | BSL                  | No |2017-02-24|Fast JSON Web Token Library for Dlang's vibe.d Framework
| [json.d](https://github.com/SirTony/json.d)                           | MIT                  | Yes |2017-12-21|An alternative JSON parser that's designed to be much nicer to work with than std.json
| [jsonserailized](https://github.com/forbjok/jsonserialized)           | MIT                  | Yes |2017-08-02|JSON serialization library for std_data_json. Easily serialize/deserialize structs and classes to/from a JSONValue.
| [jsonzer](https://github.com/rcorre/jsonizer)                         | MIT                  | Yes |2017-08-05|D language json serializer
| [jwt](https://github.com/zolamk/jwt)                                  |  MIT                 | Yes |2017-02-10|A Simple D Implementation of JSON Web Tokens.
| [jwtd](https://github.com/olehlong/jwtd)                              | MIT                  | Yes |2017-11-05|D implementation of JSON Web Token.
| [painlessjson](https://github.com/BlackEdder/painlessjson)            | BSL                  | Yes |2016-11-17|D library for converting any custom types to and from JSON the painless way.

# parsing
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [infiled](https://github.com/burner/inifiled)                         |  LGPL 3              | Yes |2017-07-29|a compile time ini file parser and writter generator for D
| [Slang-D](https://github.com/Abscissa/SDLang-D)                       | Zlib                 | Yes |2017-08-05|An SDLang (Simple Declarative Language) library for D
| [D-YAML](https://github.com/dlang-community/D-YAML)                   | Boost                | Yes |2017-10-27|YAML parser and emitter for the D programming language

# profiling
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# randomization
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [dxorshift](https://github.com/WebDrake/dxorshift)                    | CC0                  | Yes |2016-05-15|Random number generators from the extended Xorshift family
| [hap](https://github.com/WebDrake/hap)                                | BSL 1                | Yes |2017-01-07|An experimental next-generation random number package for D's standard library
| [mir-random](https://github.com/libmir/mir-random)                    | BSL 1                | No  |2017-12-22|Advanced Random Number Generators

# tests
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [checkit](https://github.com/LLC-CERERIS/checkit)                     | MIT                  | Yes |2017-08-01|BDD testing framework for D.
| [dunit](https://github.com/nomad-software/dunit)                      | MIT                  | Yes |2016-10-20|Advanced unit testing toolkit for the D programming language
| [unit-threaded](https://github.com/atilaneves/unit-threaded)          | BSD                  | Yes |2017-12-22|Advanced unit test framework for D (includes unittest blocks)

# video
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------

# time-dates
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| dateparser 															| BSL 1                | Yes ||

# miscellaneous
| library                                                               | license              | GC |last update| description
|---------------------------------------------------------------------- |:--------------------:|:---:|:---------:| -----------
| [mir-cpuid](https://github.com/libmir/mir-cpuid)                      | BSL 1                | No |2017-10-27|CPU Identification Routines
| [ip2location](https://github.com/ip2location/ip2location-d)           | LGPL 3               | Yes |2017-01-05|Use IP2Location geolocation database to lookup for accurate visitor location with D Library. It enables the user to find the country, region, city, coordinates, zip code, time zone, ISP, domain name, connection type, area code, weather, MCC, MNC, mobile brand name, elevation and usage type that any IP address or hostname originates from. 
| [miao.string](https://github.com/qqiangwu/miao.string)                 | Boost                | Yes |2017-03-31|String matching library for Dlang
| [modbus](https://github.com/deviator/modbus)                          | MIT                  | Yes |2017-12-17|Modbus protocol realization
| [natcmp](https://github.com/Herringway/natcmp)                         | BSL 1                | Yes |2017-11-03|Human-natural string comparison algorithm
| [kafka-d](https://github.com/tamediadigital/kafka-d)                   | MIT                  | Yes |2017-01-10|kafka-d is a D Kafka client that depends on the vibe.d framework.
| [stringex-d](https://github.com/katafrakt/stringex-d)                  | MIT                  | Yes |2017-07-24|Unicode to ASCII transcoder
| [vibe-aws](https://github.com/vibe-aws/vibe-aws)                       | MIT                  | Yes |2017-01-16| AWS client library for the D programming language, based on the vibe.d framework


## Thanks

Thanks to [nothings](https://github.com/nothings/single_file_libs) for inspiration.

## TODO

1. Automate some scraping from the DUB registry.
2. Consider adding a tooling section for utilities that are not libraries but aid the development.
