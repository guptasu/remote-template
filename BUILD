package(default_visibility = ["//visibility:public"])

load("@com_github_istio_mixer//tools/codegen:generate.bzl", "mixer_proto_library")

load("@io_bazel_rules_go//go:def.bzl", "go_prefix")

go_prefix("github.com/guptasu/remoteRpt")

mixer_proto_library(
    name = "go_default_library",
    protos = ["ReportTesterTemplate.proto"],
    #verbose = 10,
)
