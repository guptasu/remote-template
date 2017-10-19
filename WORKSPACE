workspace(name = "com_github_guptasu_report")

git_repository(
    name = "io_bazel_rules_go",
    commit = "9cf23e2aab101f86e4f51d8c5e0f14c012c2161c",  # Aug 1, 2017 (gazelle fixes)
    remote = "https://github.com/bazelbuild/rules_go.git",
)

load("@io_bazel_rules_go//go:def.bzl", "go_rules_dependencies", "go_register_toolchains")
go_rules_dependencies()
go_register_toolchains(go_version="1.8.3")

load("@io_bazel_rules_go//proto:def.bzl", "proto_register_toolchains")
proto_register_toolchains()

load("@io_bazel_rules_go//go:def.bzl", "go_repository")

go_repository(
    name = "com_github_istio_mixer",
    commit = "0abf3496329789992df39f752a5af8e76686f2c7",
    importpath = "istio.io/mixer",
)

load("@com_github_istio_mixer//:adapter_author_deps.bzl", "mixer_adapter_repositories")

load("@com_github_istio_mixer//:istio_api.bzl", "go_istio_api_repositories")

load("@com_github_istio_mixer//:googleapis.bzl", "go_googleapis_repositories")

mixer_adapter_repositories()

go_istio_api_repositories()

go_googleapis_repositories()

go_repository(
    name = "com_github_spf13_cobra",
    commit = "35136c09d8da66b901337c6e86fd8e88a1a255bd",  # Jan 30, 2017 (no releases)
    importpath = "github.com/spf13/cobra",
)

go_repository(
    name = "com_github_spf13_pflag",
    commit = "9ff6c6923cfffbcd502984b8e0c80539a94968b7",  # Jan 30, 2017 (no releases)
    importpath = "github.com/spf13/pflag",
)

go_repository(
    name = "com_github_hashicorp_go_multierror",
    commit = "ed905158d87462226a13fe39ddf685ea65f1c11f",  # Dec 16, 2016 (no releases)
    importpath = "github.com/hashicorp/go-multierror",
)

go_repository(
    name = "com_github_hashicorp_errwrap",
    commit = "7554cd9344cec97297fa6649b055a8c98c2a1e55",  # Oct 27, 2014 (no releases)
    importpath = "github.com/hashicorp/errwrap",
)

go_repository(
    name = "org_golang_google_genproto",
    commit = "aa2eb687b4d3e17154372564ad8d6bf11c3cf21f",  # June 1, 2017 (no releases)
    importpath = "google.golang.org/genproto",
)
