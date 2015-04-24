
try - A script that keeps trying
================================

`try` is a command wrapper for bash that solves the problem of trying the same
command over and over until it succeeds. It tries to run the supplied command
until the return code is == 0 (success) or in the range 129~160 (aborted by
signal).  Between tries it can `sleep` for a set amount of time and stops
trying after the maximum number of tries is reached.

Usage
-----

    try [-n <N>] [-t <T>] <command>

Paramters
---------

*   `<N>`   :
    The maximum number of tries, before the wrapper admits defeat. Default: 10
*   `<T>`   :
    The number of seconds to wait between tries. Default: 5
