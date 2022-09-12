load("@rules_rust//rust:defs.bzl", "rust_doc", "rust_library")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "freebsd-errno",
    srcs = ["freebsd-errno.rs"],
    crate_features = ["posix-traits"],
    target_compatible_with = [
        "@platforms//os:freebsd",
    ],
    deps = [
        "@rust_posix_errno//posix-errno",
    ],
)

rust_doc(
    name = "freebsd-errno_doc",
    crate = ":freebsd-errno",
)
