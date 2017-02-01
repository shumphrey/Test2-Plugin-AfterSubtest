Test2::Plugin::AfterSubtest
===========================

Exports a single function for executing a callback after a subtest has completed.

```perl
use Test2::Bundle::More;
use Test2::Plugin::AfterSubtest;

after_subtest(sub {
    diag "subtest has finished";
});

subtest test => sub {
    ok('subtest is running');
};
```
