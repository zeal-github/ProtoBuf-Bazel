# ProtoBuf-Bazel
Minimum example to using protocal buffer in bazel c++ project.

This project is tested in:
1. bazel 5.2.0

The example is copy from [protocal buffer c++ tutorials](https://developers.google.com/protocol-buffers/docs/cpptutorial)

# Resources
1. [protocal buffer c++ tutorials](https://developers.google.com/protocol-buffers/docs/cpptutorial)
2. [bazel proto tutorials](https://bazel.build/reference/be/c-cpp#cc_proto_library)
3. [bazel cc_proto_rules](https://github.com/bazelbuild/rules_proto/tree/4.0.0-3.20.0)

# Usage
```bash
git clone this project
cd /path/to/this_project

bazel build //:all
# the protoc generated file will be located in ./bazel-bin/addressbook.pb.h && ./bazel-bin/addressbook.pb.cc
./bazel-bin/write_message addressbook.db # create and add new address to database

./bazel-bin/list_addressbook addressbook.db # list address book
```