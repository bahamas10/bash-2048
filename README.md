bash 2048
=========

My take at http://gabrielecirulli.github.io/2048/ in pure bash

![screenshot][screenshot.png]

Usage
-----

**note:** try `-a` for awesome animations

    $ ./2048 -h
    Usage: 2048 [-a] [-b] [-h] [-g <goal>] [-s <size>]

    Options
      -a          enable animations, note they are slow and weird
      -b          disable color output, b for boring!
      -g <goal>   the goal piece, defaults to 2048
      -h          print this message and exit
      -s <size>   the size of the board, defaults to 4

External Utilities
------------------

`tput` is the only external command used in this bash script to figure out the proper
codes to print for colorized output.  If your system lacks `tput`, it will still work
without color support.

Issues
------

- Performance is lacking... the algorithm could probably be optimized
- Animations with `-a` are slow and wonky

License
-------

MIT License
