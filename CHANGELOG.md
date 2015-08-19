
# Changelog

## 2.0.0

### New features

* Add Clojurescript support.
* Remove `title-case`, it was duplicating `clojure.string/capitalize`.
* Various docstring improvements.

### Bugs fixed

* [#4](https://github.com/expez/superstring/issues/4) Inconsistency in the `pascal-case` docstring.  Examples were correct, prose was wrong.

# 1.1.0
### New features

* Add `char-at`, which wraps the native String/charAt
* Add `re-quote` which quotes a string, for use in regular expressions.

### Bugs fixed

* `mixed-case?` is now false on strings like "123" where no character has a case.
* `swap-case` on "ß" now returns "SS"
* Fix `starts-with?` throwing exception when `prefix` is longer than `s`.
