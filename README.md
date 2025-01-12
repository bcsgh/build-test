<!-- Generated with Stardoc: http://skydoc.bazel.build -->

# A Bazel test rule that tests if another rule builds.

A basic test that always passes, as long as everythin in `targets` builds.
This is usefull, for example, with a genrule.

NOTE consider using:
https://github.com/bazelbuild/bazel-skylib/blob/main/docs/build_test_doc.md

## `MODULE.bazel`

```
bazel_dep(
    name = "com_github_bcsgh_build_test",
    version = ...,
)
```

<a id="build_test"></a>

## build_test

<pre>
load("@com_github_bcsgh_build_test//build_test:build.bzl", "build_test")

build_test(<a href="#build_test-name">name</a>, <a href="#build_test-targets">targets</a>)
</pre>

A test that depends on arbitary targets.

**ATTRIBUTES**


| Name  | Description | Type | Mandatory | Default |
| :------------- | :------------- | :------------- | :------------- | :------------- |
| <a id="build_test-name"></a>name |  A unique name for this target.   | <a href="https://bazel.build/concepts/labels#target-names">Name</a> | required |  |
| <a id="build_test-targets"></a>targets |  Targets to check.   | <a href="https://bazel.build/concepts/labels">List of labels</a> | required |  |


## Setup (for development)
To configure the git hooks, run `./.git_hooks/setup.sh`
