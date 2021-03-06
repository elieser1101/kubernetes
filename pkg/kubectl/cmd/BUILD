load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = [
        "alpha.go",
        "cmd.go",
        "profiling.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/kubectl/cmd",
    visibility = [
        "//build/visible_to:pkg_kubectl_cmd_CONSUMERS",
    ],
    deps = [
        "//pkg/kubectl/cmd/annotate:go_default_library",
        "//pkg/kubectl/cmd/apiresources:go_default_library",
        "//pkg/kubectl/cmd/apply:go_default_library",
        "//pkg/kubectl/cmd/attach:go_default_library",
        "//pkg/kubectl/cmd/auth:go_default_library",
        "//pkg/kubectl/cmd/autoscale:go_default_library",
        "//pkg/kubectl/cmd/certificates:go_default_library",
        "//pkg/kubectl/cmd/clusterinfo:go_default_library",
        "//pkg/kubectl/cmd/completion:go_default_library",
        "//pkg/kubectl/cmd/config:go_default_library",
        "//pkg/kubectl/cmd/convert:go_default_library",
        "//pkg/kubectl/cmd/cp:go_default_library",
        "//pkg/kubectl/cmd/create:go_default_library",
        "//pkg/kubectl/cmd/delete:go_default_library",
        "//pkg/kubectl/cmd/describe:go_default_library",
        "//pkg/kubectl/cmd/diff:go_default_library",
        "//pkg/kubectl/cmd/drain:go_default_library",
        "//pkg/kubectl/cmd/edit:go_default_library",
        "//pkg/kubectl/cmd/exec:go_default_library",
        "//pkg/kubectl/cmd/explain:go_default_library",
        "//pkg/kubectl/cmd/expose:go_default_library",
        "//pkg/kubectl/cmd/get:go_default_library",
        "//pkg/kubectl/cmd/kustomize:go_default_library",
        "//pkg/kubectl/cmd/label:go_default_library",
        "//pkg/kubectl/cmd/logs:go_default_library",
        "//pkg/kubectl/cmd/options:go_default_library",
        "//pkg/kubectl/cmd/patch:go_default_library",
        "//pkg/kubectl/cmd/plugin:go_default_library",
        "//pkg/kubectl/cmd/portforward:go_default_library",
        "//pkg/kubectl/cmd/proxy:go_default_library",
        "//pkg/kubectl/cmd/replace:go_default_library",
        "//pkg/kubectl/cmd/rollingupdate:go_default_library",
        "//pkg/kubectl/cmd/rollout:go_default_library",
        "//pkg/kubectl/cmd/run:go_default_library",
        "//pkg/kubectl/cmd/scale:go_default_library",
        "//pkg/kubectl/cmd/set:go_default_library",
        "//pkg/kubectl/cmd/taint:go_default_library",
        "//pkg/kubectl/cmd/top:go_default_library",
        "//pkg/kubectl/cmd/util:go_default_library",
        "//pkg/kubectl/cmd/version:go_default_library",
        "//pkg/kubectl/cmd/wait:go_default_library",
        "//pkg/kubectl/util/i18n:go_default_library",
        "//pkg/kubectl/util/templates:go_default_library",
        "//staging/src/k8s.io/apiserver/pkg/util/flag:go_default_library",
        "//staging/src/k8s.io/cli-runtime/pkg/genericclioptions:go_default_library",
        "//staging/src/k8s.io/client-go/tools/clientcmd:go_default_library",
        "//vendor/github.com/spf13/cobra:go_default_library",
        "//vendor/github.com/spf13/pflag:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["cmd_test.go"],
    data = [
        "//api/openapi-spec",
        "//pkg/kubectl/cmd/plugin:testdata",
        "//test/e2e/testing-manifests:all-srcs",
        "//test/fixtures",
    ],
    embed = [":go_default_library"],
    deps = [
        "//pkg/kubectl/cmd/util:go_default_library",
        "//staging/src/k8s.io/cli-runtime/pkg/genericclioptions:go_default_library",
        "//vendor/github.com/spf13/cobra:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//pkg/kubectl/cmd/annotate:all-srcs",
        "//pkg/kubectl/cmd/apiresources:all-srcs",
        "//pkg/kubectl/cmd/apply:all-srcs",
        "//pkg/kubectl/cmd/attach:all-srcs",
        "//pkg/kubectl/cmd/auth:all-srcs",
        "//pkg/kubectl/cmd/autoscale:all-srcs",
        "//pkg/kubectl/cmd/certificates:all-srcs",
        "//pkg/kubectl/cmd/clusterinfo:all-srcs",
        "//pkg/kubectl/cmd/completion:all-srcs",
        "//pkg/kubectl/cmd/config:all-srcs",
        "//pkg/kubectl/cmd/convert:all-srcs",
        "//pkg/kubectl/cmd/cp:all-srcs",
        "//pkg/kubectl/cmd/create:all-srcs",
        "//pkg/kubectl/cmd/delete:all-srcs",
        "//pkg/kubectl/cmd/describe:all-srcs",
        "//pkg/kubectl/cmd/diff:all-srcs",
        "//pkg/kubectl/cmd/drain:all-srcs",
        "//pkg/kubectl/cmd/edit:all-srcs",
        "//pkg/kubectl/cmd/exec:all-srcs",
        "//pkg/kubectl/cmd/explain:all-srcs",
        "//pkg/kubectl/cmd/expose:all-srcs",
        "//pkg/kubectl/cmd/get:all-srcs",
        "//pkg/kubectl/cmd/help:all-srcs",
        "//pkg/kubectl/cmd/kustomize:all-srcs",
        "//pkg/kubectl/cmd/label:all-srcs",
        "//pkg/kubectl/cmd/logs:all-srcs",
        "//pkg/kubectl/cmd/options:all-srcs",
        "//pkg/kubectl/cmd/patch:all-srcs",
        "//pkg/kubectl/cmd/plugin:all-srcs",
        "//pkg/kubectl/cmd/portforward:all-srcs",
        "//pkg/kubectl/cmd/proxy:all-srcs",
        "//pkg/kubectl/cmd/replace:all-srcs",
        "//pkg/kubectl/cmd/rollingupdate:all-srcs",
        "//pkg/kubectl/cmd/rollout:all-srcs",
        "//pkg/kubectl/cmd/run:all-srcs",
        "//pkg/kubectl/cmd/scale:all-srcs",
        "//pkg/kubectl/cmd/set:all-srcs",
        "//pkg/kubectl/cmd/taint:all-srcs",
        "//pkg/kubectl/cmd/testing:all-srcs",
        "//pkg/kubectl/cmd/top:all-srcs",
        "//pkg/kubectl/cmd/util:all-srcs",
        "//pkg/kubectl/cmd/version:all-srcs",
        "//pkg/kubectl/cmd/wait:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = [
        "//build/visible_to:pkg_kubectl_cmd_CONSUMERS",
    ],
)
