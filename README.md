Really simple templating
========================

This is a very simple templating utility based on picking random
values for variables of certain types from a value list.

Assuming that the file values.lua contains the following content:

	{
		noun={"dialectic", "enlightenment", "revolution", "reduction"},
		verb={"provides", "improves", "is"}
	}

A possible input to `alois values.lua` could be:

	The [x:noun] of [y:noun] [v:verb] the [y:noun] of [x:noun].

and the output would be something like:

	The dialectic of revolution is the revolution of dialectic.

More complex inputs are of course possible.

The name of the utility has no meaning.

Requirements
------------

This utility needs the programming language lua, and furthermore requires
the simple unix utilities mkdir, cp, rm and chmod.

Installation
------------

	make install

should install alois to /usr/local.

License
=======

MIT license, more details in [LICENSE](./LICENSE).
