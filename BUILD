load("@rules_go//go:def.bzl", "go_test")
load("@gazelle//:def.bzl", "gazelle")

gazelle(name = "gazelle")

go_test(
    name = "a_test",
    srcs = ["main_test.go"],
    data = ["//liba"],
    x_defs = {
        "libAPath": "$(rlocationpath //liba)",
    },
)
