Dafny for Unikraft
=============================

This is the port of Dafny as a Unikraft external library. We currently 
support only the C++ output. It depends on the following libraries 
that need to be added to `Makefile` in this order:

* `libc`, e.g. `newlib`
* `libcxx'
* `libunwind`
* `libcxxabi`
* `compiler-rt`

# Using Dafny in your projects
We the following suffix to `>.cpp`. For example:
```
APPHELLOWORLD_SRCS-y += $(APPHELLOWORLD_BASE)/test.dfy>.cpp
```

Please refer to the `README.md` as well as the documentation in the `doc/`
subdirectory of the main unikraft repository.
