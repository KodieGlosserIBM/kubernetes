package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = [
        "autoscale_test.go",
        "clusterrolebinding_test.go",
        "configmap_test.go",
        "delete_test.go",
        "deployment_test.go",
        "env_file_test.go",
        "generate_test.go",
        "history_test.go",
        "namespace_test.go",
        "pdb_test.go",
        "priorityclass_test.go",
        "quota_test.go",
        "rolebinding_test.go",
        "rollback_test.go",
        "rolling_updater_test.go",
        "rollout_status_test.go",
        "run_test.go",
        "scale_test.go",
        "secret_for_docker_registry_test.go",
        "secret_for_tls_test.go",
        "secret_test.go",
        "service_basic_test.go",
        "service_test.go",
        "serviceaccount_test.go",
        "sorter_test.go",
    ],
    embed = [":go_default_library"],
    deps = [
        "//pkg/api/legacyscheme:go_default_library",
        "//pkg/api/testapi:go_default_library",
        "//pkg/api/testing:go_default_library",
        "//pkg/apis/batch:go_default_library",
        "//pkg/apis/core:go_default_library",
        "//pkg/apis/extensions:go_default_library",
        "//pkg/client/clientset_generated/internalclientset:go_default_library",
        "//pkg/client/clientset_generated/internalclientset/fake:go_default_library",
        "//pkg/client/clientset_generated/internalclientset/typed/core/internalversion:go_default_library",
        "//pkg/kubectl/util:go_default_library",
        "//pkg/util/pointer:go_default_library",
        "//vendor/github.com/spf13/cobra:go_default_library",
        "//vendor/k8s.io/api/apps/v1:go_default_library",
        "//vendor/k8s.io/api/apps/v1beta1:go_default_library",
        "//vendor/k8s.io/api/autoscaling/v1:go_default_library",
        "//vendor/k8s.io/api/batch/v1:go_default_library",
        "//vendor/k8s.io/api/batch/v1beta1:go_default_library",
        "//vendor/k8s.io/api/batch/v2alpha1:go_default_library",
        "//vendor/k8s.io/api/core/v1:go_default_library",
        "//vendor/k8s.io/api/extensions/v1beta1:go_default_library",
        "//vendor/k8s.io/api/policy/v1beta1:go_default_library",
        "//vendor/k8s.io/api/rbac/v1:go_default_library",
        "//vendor/k8s.io/api/rbac/v1beta1:go_default_library",
        "//vendor/k8s.io/api/scheduling/v1alpha1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/equality:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/resource:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1/unstructured:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/intstr:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/uuid:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/watch:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes/fake:go_default_library",
        "//vendor/k8s.io/client-go/rest:go_default_library",
        "//vendor/k8s.io/client-go/rest/fake:go_default_library",
        "//vendor/k8s.io/client-go/scale:go_default_library",
        "//vendor/k8s.io/client-go/scale/fake:go_default_library",
        "//vendor/k8s.io/client-go/testing:go_default_library",
        "//vendor/k8s.io/client-go/util/testing:go_default_library",
    ],
)

go_library(
    name = "go_default_library",
    srcs = [
        "apply.go",
        "autoscale.go",
        "bash_comp_utils.go",
        "clusterrolebinding.go",
        "conditions.go",
        "configmap.go",
        "delete.go",
        "deployment.go",
        "doc.go",
        "env_file.go",
        "generate.go",
        "history.go",
        "interfaces.go",
        "namespace.go",
        "pdb.go",
        "priorityclass.go",
        "quota.go",
        "rolebinding.go",
        "rollback.go",
        "rolling_updater.go",
        "rollout_status.go",
        "run.go",
        "scale.go",
        "secret.go",
        "secret_for_docker_registry.go",
        "secret_for_tls.go",
        "service.go",
        "service_basic.go",
        "serviceaccount.go",
        "sorter.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/kubectl",
    deps = [
        "//pkg/api/legacyscheme:go_default_library",
        "//pkg/api/pod:go_default_library",
        "//pkg/api/v1/pod:go_default_library",
        "//pkg/apis/apps:go_default_library",
        "//pkg/apis/batch:go_default_library",
        "//pkg/apis/core:go_default_library",
        "//pkg/apis/core/v1:go_default_library",
        "//pkg/apis/extensions:go_default_library",
        "//pkg/client/clientset_generated/internalclientset:go_default_library",
        "//pkg/client/clientset_generated/internalclientset/typed/apps/internalversion:go_default_library",
        "//pkg/client/clientset_generated/internalclientset/typed/batch/internalversion:go_default_library",
        "//pkg/client/clientset_generated/internalclientset/typed/core/internalversion:go_default_library",
        "//pkg/client/clientset_generated/internalclientset/typed/extensions/internalversion:go_default_library",
        "//pkg/controller/deployment/util:go_default_library",
        "//pkg/credentialprovider:go_default_library",
        "//pkg/kubectl/apps:go_default_library",
        "//pkg/kubectl/cmd/scalejob:go_default_library",
        "//pkg/kubectl/resource:go_default_library",
        "//pkg/kubectl/util:go_default_library",
        "//pkg/kubectl/util/hash:go_default_library",
        "//pkg/kubectl/util/slice:go_default_library",
        "//pkg/printers:go_default_library",
        "//pkg/printers/internalversion:go_default_library",
        "//vendor/github.com/golang/glog:go_default_library",
        "//vendor/github.com/spf13/cobra:go_default_library",
        "//vendor/github.com/spf13/pflag:go_default_library",
        "//vendor/k8s.io/api/apps/v1:go_default_library",
        "//vendor/k8s.io/api/apps/v1beta1:go_default_library",
        "//vendor/k8s.io/api/autoscaling/v1:go_default_library",
        "//vendor/k8s.io/api/batch/v1:go_default_library",
        "//vendor/k8s.io/api/batch/v1beta1:go_default_library",
        "//vendor/k8s.io/api/batch/v2alpha1:go_default_library",
        "//vendor/k8s.io/api/core/v1:go_default_library",
        "//vendor/k8s.io/api/extensions/v1beta1:go_default_library",
        "//vendor/k8s.io/api/policy/v1beta1:go_default_library",
        "//vendor/k8s.io/api/rbac/v1:go_default_library",
        "//vendor/k8s.io/api/rbac/v1beta1:go_default_library",
        "//vendor/k8s.io/api/scheduling/v1alpha1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/meta:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/resource:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1/unstructured:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/intstr:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/json:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/strategicpatch:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/uuid:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/validation:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/wait:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/watch:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes/typed/apps/v1:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes/typed/apps/v1beta1:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes/typed/extensions/v1beta1:go_default_library",
        "//vendor/k8s.io/client-go/rest:go_default_library",
        "//vendor/k8s.io/client-go/scale:go_default_library",
        "//vendor/k8s.io/client-go/util/integer:go_default_library",
        "//vendor/k8s.io/client-go/util/jsonpath:go_default_library",
        "//vendor/k8s.io/client-go/util/retry:go_default_library",
        "//vendor/vbom.ml/util/sortorder:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//pkg/kubectl/apply:all-srcs",
        "//pkg/kubectl/apps:all-srcs",
        "//pkg/kubectl/cmd:all-srcs",
        "//pkg/kubectl/explain:all-srcs",
        "//pkg/kubectl/genericclioptions:all-srcs",
        "//pkg/kubectl/metricsutil:all-srcs",
        "//pkg/kubectl/plugins:all-srcs",
        "//pkg/kubectl/proxy:all-srcs",
        "//pkg/kubectl/resource:all-srcs",
        "//pkg/kubectl/scheme:all-srcs",
        "//pkg/kubectl/util:all-srcs",
        "//pkg/kubectl/validation:all-srcs",
    ],
    tags = ["automanaged"],
)
