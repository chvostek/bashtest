You want to use bashisms without bash?  Here you go.

Note: This is a silly hack.  :-)

To install, you'll probably want to include this as a library:

    #!/bin/sh

    . /path/to/bashtest

**Note:** You need to quote or escape some things that wouldn't require
quoting or escaping in bash. For example:

    $ if [[ "foo" ~ '.*o' ]]; then echo yes; else echo no; fi
    yes

    $ if [[ 5 \> 3 ]]; then echo yes; else echo no; fi
    yes

