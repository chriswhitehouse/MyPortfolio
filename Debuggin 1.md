### Debugging 1: Introduction to debugging; ran through simple geocoder code base with errors to debug:

* three steps:
    1) Tighten the loop (find the exact line the error is coming from)
    2) Get Visibility (use p to inspect everything to get the exact line)
    3) Once you know the one thing that is throwing the error, fix it.

* learnt how to read the stack trace (from bottom to top). Keeping an eye on the file path of each trace.
* Exceptions is the ruby name for errors, every error has a name as defined by the exceptions class: https://ruby-doc.org/core-2.5.1/Exception.html
* Sometimes errors will be in libraries rather than just source code. Can access the gem code with ~$ bundle open [name]~ (having previously run $ bundle install to include all gems)
