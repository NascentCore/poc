# PoC

Proof of concept of NascentCore's ML infrastructure system.

## Bazel workspace setup

This repo uses `bazel`. The setup follows [How to use Bazel](
https://docs.bazel.build/versions/master/getting-started.html#installation).

Notes:

*   `.gitignore` has an entry to ignore `bazel-*` files.

## Setup SSH connection to Github

See [Connecting to GitHub with SSH](
https://help.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh),
especially
[Generating a new SSH key and adding it to the ssh-agent](
https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

## Useful links

*   [Markdown cheatsheet](
    https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).
    Markdown is used to write documents.

### Bazel

*   [Bazel rules for Go](
    https://github.com/bazelbuild/rules_go).
*   [Bazel gazelle](https://github.com/bazelbuild/bazel-gazelle). Gazelle is
    used to manage build files for Go source code.
*   [Bazel rules for docker](https://github.com/bazelbuild/rules_docker).
    *   Registry needs to be set to `index.docker.io`
    *   To push, first `docker login -u <username> --password-stdin`
    *   Then `bazel run :<container_push_label>`

### Machine learning

*   [CIFAR-10 with TensorFlow](https://www.tensorflow.org/tutorials/images/cnn).
*   [TensorFlow with Docker](https://www.tensorflow.org/install/docker).
