load("@rules_python//python:defs.bzl", "py_test")

test_srcs = glob(["**/*.py"])

py_test(
    name = "serve_failure_smoke_test",
    size = "medium",
    srcs = test_srcs,
    env = {
        "RAY_UNIT_TEST": "1",
    },
    main = "serve_failure.py",
    tags = [
        "exclusive",
        "team:serve",
    ],
    deps = [
        "//:ray_lib",
        "//python/ray/serve:serve_lib",
    ],
)

py_test(
    name = "autoscaling_single_deployment_smoke_test",
    size = "medium",
    srcs = test_srcs,
    env = {
        "IS_SMOKE_TEST": "1",
    },
    main = "autoscaling_single_deployment.py",
    tags = [
        "exclusive",
        "team:serve",
    ],
    deps = [
        "//:ray_lib",
        "//python/ray/serve:serve_lib",
    ],
)

py_test(
    name = "autoscaling_multi_deployment_smoke_test",
    size = "medium",
    srcs = test_srcs,
    env = {
        "IS_SMOKE_TEST": "1",
    },
    main = "autoscaling_multi_deployment.py",
    tags = [
        "exclusive",
        "team:serve",
    ],
    deps = [
        "//:ray_lib",
        "//python/ray/serve:serve_lib",
    ],
)

py_test(
    name = "test_alerts",
    tags = ["team:ml", "release_unit"],
    size = "small",
    srcs = ["ray_release/tests/test_alerts.py"]
)

py_test(
    name = "test_buildkite",
    tags = ["team:ml", "release_unit"],
    size = "small",
    srcs = ["ray_release/tests/test_buildkite.py"]
)

py_test(
    name = "test_cluster_manager",
    tags = ["team:ml", "release_unit"],
    size = "small",
    srcs = ["ray_release/tests/test_cluster_manager.py"]
)

py_test(
    name = "test_glue",
    tags = ["team:ml", "release_unit"],
    size = "small",
    srcs = ["ray_release/tests/test_glue.py"]
)

py_test(
    name = "test_repeat",
    tags = ["team:ml", "release_unit"],
    size = "small",
    srcs = ["ray_release/tests/test_repeat.py"]
)

py_test(
    name = "test_wheels",
    tags = ["team:ml", "release_unit"],
    size = "small",
    srcs = ["ray_release/tests/test_wheels.py"]
)
