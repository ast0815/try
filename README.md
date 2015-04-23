
try - A script the keeps trying
===============================

`try` is a command wrapper for bash that solves the problem of trying the same
command over and over until it succeeds. It tries to run the supplied command
until the return code is == 0 or >128, or the maximum number of tries is
reached. Between tries it can `sleep` for a set amount of time.
