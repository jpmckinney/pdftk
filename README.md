To switch from GCJ binaries to `javac`, `javah`, `jar`:

* Switch double-dash with single-dash and remove equals sign in all command-line options.
* Use periods not slashes in arguments to `javah`.
* Replace `-Wall` with `-Xlint`.
* Replace `-fsource=1.3` with `-source 1.3`.
* Remove `-O2`, which optimizes object code.
* Remove `-C`, which tells gcj to generate bytecode (.class files) rather than object code (.o files).
* Update paths to binaries, `dylib` files, and `libgcj.jar` in `Makefile.OSX-10.6`.
