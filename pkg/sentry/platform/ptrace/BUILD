load("//tools:defs.bzl", "go_library")

package(
    default_applicable_licenses = ["//:license"],
    licenses = ["notice"],
)

go_library(
    name = "ptrace",
    srcs = [
        "filters.go",
        "ptrace.go",
        "ptrace_amd64.go",
        "ptrace_arm64.go",
        "ptrace_arm64_unsafe.go",
        "ptrace_unsafe.go",
        "stub_amd64.s",
        "stub_arm64.s",
        "stub_unsafe.go",
        "subprocess.go",
        "subprocess_amd64.go",
        "subprocess_arm64.go",
        "subprocess_linux.go",
        "subprocess_linux_unsafe.go",
        "subprocess_unsafe.go",
    ],
    visibility = ["//:sandbox"],
    deps = [
        "//pkg/abi/linux",
        "//pkg/bpf",
        "//pkg/context",
        "//pkg/cpuid",
        "//pkg/fd",
        "//pkg/hostarch",
        "//pkg/hosttid",
        "//pkg/log",
        "//pkg/safecopy",
        "//pkg/seccomp",
        "//pkg/sentry/arch",
        "//pkg/sentry/arch/fpu",
        "//pkg/sentry/memmap",
        "//pkg/sentry/platform",
        "//pkg/sentry/platform/interrupt",
        "//pkg/sighandling",
        "//pkg/sync",
        "@org_golang_x_sys//unix:go_default_library",
    ],
)
