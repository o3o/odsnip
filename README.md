# odnsnip - my  UltiSnips snippets for D

odsnips is a collection of [UltiSnips](https://github.com/SirVer/ultisnips) snippets for the D programming language based on work of
[Ferdinand Majerech](https://github.com/kiith-sa/DSnips)

## Getting Started
* Install [UltiSnips](https://github.com/SirVer/ultisnips#quick-start)
* Get odsnip: `git clone https://github.com/o3o/odsnip.git``
* Copy the ``d.snippets`` file to UltiSnips user snippets directory. On Linux this
  should be ``~/.vim/UltiSnips``.
## References
### Language
|          |                               |
| ---      | -----                         |
| `al`     | alias                         |
| `auto`   | auto /*variable*/ = /*value*/ |
| `cast`   | cast(/type*/)                 |
| `con`    | const *variable* = *value*    |
| `const`  | const()                       |
| `format` | format(/*values*/)            |
| `len`    | length                        |
| `mixin`  | mixin                         |
| `module` | module                        |
| `new`    | new                           |
| `over`   | override                      |
| `priv`   | private                       |
| `pub`    | public                        |
| `publ`   | public: /*memeber*/           |
| `pubb`   | public {/*memeber*/}          |
| `ret`    | return                        |
| `rett`   | return /value to return*/     |
| `scope`  | scope (exit)                  |
| `super`  | super(/*args*/)               |
| `vd`     | void                          |
| `with`   | with ()                       |

### Vibe.d log
|         |               |
| ---     | -----         |
| `logd`  | logDebug      |
| `logdi` | logDiagnostic |
| `logi`  | logInfo       |
| `logw`  | logWarn       |
| `loge`  | logError      |

### Import
|         |                                              |
| ---     | -----                                        |
| `imp`   | import list                                  |
| `impa`  | import std.array                             |
| `impc`  | import std.conv;                             |
| `impe`  | import std.signals                           |
| `impex` | import std.exception                         |
| `impf`  | import std.file                              |
| `impi`  | import std.stdio                             |
| `impo`  | import /*module*/                            |
| `imps`  | import std.string                            |
| `impu`  | import unit_threaded                         |
| `impuv` | `version(unittest) { import unit_threaded }` |
| `pimp`  | public import /*module*/                     |

### Unit threaded
|        |                           |
| ---    | -----                     |
| `seq`  | shouldEqual               |
| `saeq` | shouldApproxEqual(/*to*/) |
| `sinc` | shouldInclude(/*item*/)   |
| `sneq` | shouldNotEqual(/*to*/)    |
| `st`   | shouldBeTrue              |
| `sf`   | shouldBeFalse             |
| `sn`   | shouldBeNull              |
| `sgt`  | shouldBeGreaterThan       |
| `sst`  | shouldBeSmallerThan       |
| `ssj`  | shouldBeSameJsonAs        |
| `snn`  | shouldNotBeNull           |
| `sth`  | shouldThrow!Exception     |
| `snth` | shouldNotThrow!Exception  |
| `ht`   | @HiddenTest(message)      |
| `ut`   | @UnitTest                 |

### Phobos
|         |                                 |
| ---     | -----                           |
| `imm`   | immutable()                     |
| `siz`   | size_t /*variable*/ = /*value*/ |
| `wr`    | writeln()                       |
| `wr`    | writeln()                       |
| `wrf`   | writefln()                      |

### Conversion
|        |                        |
| ---    | -----                  |
| `to`   | to!/*type*/(/*arg*/)   |
| `top`  | to!(/*type*/)(/*arg*/) |
| `tos`  | to!string()            |
| `tosa` | to!string(/*arg*/)     |

### Branches
|        |                                     |
| ---    | -----                               |
| `if`   | if (/*condition*/)                  |
| `ifnn` | if (/*condition*/ !is null)         |
| `ife`  | if (/*condition*/) else             |
| `el`   | else {                              |
| `elif` | else if (/*condition*/)             |
| `sif`  | static if ()                        |
| `sw`   | switch (/*var*/) .. case            |
| `fsw`  | final switch (/*var*/)              |
| `case` | case /*value*/:  break              |
| `?:`   | /*condition*/ ? /*then*/ : /*else*/ |

### Loops
|           |                                                 |
| ---       | -----                                           |
| `do`      | do while                                        |
| `wh`      | while (/*condition*/)                           |
| `for`     | for (size_t i = 0; i < count; ++i)              |
| `fori`    | for (int i = 0; i < count; ++i)                 |
| `forever` | for (;;)                                        |
| `fore`    | foreach (/*elem*/; /*range*/)                   |
| `forif`   | foreach (/*elem*/; /*range*/) if(/*condition*/) |

### Contracts
|        |                                                |
| ---    | -----                                          |
| `req`  | assert(var !is null) and assign                |
| `reqn` | assert(var !is null)                           |
| `in`   | in                                             |
| `out`  | out                                            |
| `body` | body                                           |
| `inv`  | invariant()                                    |
| `enf`  | enforce(/*condition*/)                         |
| `enfe` | enforce(/*condition*/,new Exception(/*args*/)) |
| `enfa` | enforce(/*condition*/)  ans assegnation        |

### Functions
|           |                                                        |
| ---       | -----                                                  |
| `fun`     | /*ret*/ /*function name*/(/*args*/) @safe pure nothrow |
| `func`    | void /*function name*/(/*args*/) @safe pure nothrow    |
| `this`    | this(/*args*/)                                         |
| `get`     | *getter property*                                      |
| `set`     | *setter property*                                      |
| `getset`  | *getter setter property*                               |
| `getp`    | *getter property pure*                                 |
| `setp`    | *setter property pure*                                 |
| `getsetp` | *getter setter property pure*                          |
| `prop`    | @property                                              |
| `main`    | void main(string[] args)                               |
| `maini`   | int main(string[] args)                                |

### Signal
|          |                                   |
| ---      | -----                             |
| `signal` | mixin Signal!(/*args*/) /*name*/; |
| `emit`   | emit(/*arg*/);                    |

### Exception handling
|         |                         |
| ---     | -----                   |
| `try`   | try , catch             |
| `tryf`  | try , catch and finally |
| `catch` | catch (Exception e)     |
| `thr`   | throw new Exception("") |
| `exc` | Exception class declaration |

### Type definitions
|          |           |
| ---      | -----     |
| `struct` | struct    |
| `union`  | union     |
| `class`  | class     |
| `inter`  | interface |
| `enum`   | enum      |

### Conditional compilation
|             |                             |
| ---         | -----                       |
| `version`   | version ()                  |
| `versioni`  | version (/*name*/) /*code*/ |
| `versionl`  | version (linux)             |
| `versionw`  | version (Windows)           |
| `versionil` | version (linux) /*code*/    |
| `versioniw` | version (Windows) /*code*/  |
| `debug`     | debug                       |

### Template
|        |                             |
| ---    | -----                       |
| `temp` | template /*name*/(/*args*/) |

### Assert
|       |                                        |
| ---   | -----                                  |
| `as`  | assert(false)                          |
| `asm` | assert(/*condition*/, "error message") |
| `sas` | static assert(false)                   |
|

### DDoc and comments
|           |                           |
| ---       | -----                     |
| `fix`     | // FIX:                   |
| `todo`    | // TODO:                  |
| `sdc`     | Short sdoc  block         |
| `doc`     | Generic sdoc  block       |
| `fdoc`    | Function ddoc block       |
| `fsdoc`   | Short function ddoc block |
| `Pars`    | Params ddoc block         |
| `Par`     | Params inline             |
| `Ret`     | Returns                   |
| `Thr`     | Throws                    |
| `Example` | Examples                  |

### License
|         |               |
| ---     | -----         |
| `gpl`   | GPL License   |
| `boost` | Boost License |
