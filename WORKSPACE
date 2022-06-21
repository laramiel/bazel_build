workspace(name = "laramiel_bazel_build")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "bazel_skylib",
    urls = ["https://github.com/bazelbuild/bazel-skylib/releases/download/1.2.1/bazel-skylib-1.2.1.tar.gz"],
    sha256 = "f7be3474d42aae265405a592bb7da8e171919d74c16f082a5457840f06054728",
)

load("@bazel_skylib//:workspace.bzl", "bazel_skylib_workspace")

bazel_skylib_workspace()

http_archive(
    name = "org_libuv",
    sha256 = "d233a9c522a9f4afec47b0d12f302d93d114a9e3ea104150e65f55fd931518e6",
    strip_prefix = "libuv-1.44.1",
    urls = [
        "https://github.com/libuv/libuv/archive/v1.44.1.zip",
    ],
    build_file = Label("//third_party:org_libuv/libuv.BUILD.bazel"),
)

http_archive(
    name = "org_libevent",
    sha256 = "92e6de1be9ec176428fd2367677e61ceffc2ee1cb119035037a27d346b0403bb",
    strip_prefix = "libevent-2.1.12-stable",
    urls = [
        "https://github.com/libevent/libevent/releases/download/release-2.1.12-stable/libevent-2.1.12-stable.tar.gz",
    ],
    build_file = Label("//third_party:org_libevent/libevent.BUILD.bazel"),
)

