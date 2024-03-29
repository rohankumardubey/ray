# --------------------------------------------------------------------
# Tests from the doc directory.
# Please keep these sorted alphabetically, but start with the
# root directory.
# --------------------------------------------------------------------

# Support for Dask has been dropped in 3.6.
py_test(
    name = "dask_xgboost",
    size = "medium",
    main = "test_myst_doc.py",
    srcs = ["test_myst_doc.py"],
    tags = ["exclusive", "team:ml", "py37"],
    data = ["//doc/source/ray-core/examples:core_examples"],
    args = ["--path", "doc/source/ray-core/examples/dask_xgboost/dask_xgboost.ipynb",
            "--smoke-test", "--address ''", "--num-actors 4", "--cpus-per-actor 1", "--num-actors-inference 4",
            "--cpus-per-actor-inference 1"]
)

# Support for Modin has been dropped in 3.6.
py_test(
    name = "modin_xgboost",
    size = "medium",
    main = "test_myst_doc.py",
    srcs = ["test_myst_doc.py"],
    tags = ["exclusive", "team:ml", "py37"],
    data = ["//doc/source/ray-core/examples:core_examples"],
    args = ["--path", "doc/source/ray-core/examples/modin_xgboost/modin_xgboost.ipynb",
            "--smoke-test", "--address ''", "--num-actors 4",
            "--cpus-per-actor 1", "--num-actors-inference 4",
            "--cpus-per-actor-inference 1"]
)

### Ray Data
py_test(
    name = "quick_start",
    size = "small",
    srcs = ["source/data/doc_code/quick_start.py"],
    tags = ["exclusive", "team:ml"]
)

py_test(
    name = "big_data_ingestion",
    size = "small",
    main = "test_myst_doc.py",
    srcs = ["test_myst_doc.py"],
    args = ["--path", "doc/source/data/examples/big_data_ingestion.ipynb"],
    data = ["//doc/source/data/examples:data_examples"],
    tags = ["exclusive", "team:core", "py37"]
)

py_test(
    name = "datasets_train",
    size = "medium",
    srcs = ["source/ray-core/_examples/datasets_train/datasets_train.py"],
    tags = ["exclusive", "team:ml", "py37", "datasets_train"],
    args = ["--smoke-test", "--num-workers=2", "--use-gpu"]
)

py_test(
    name = "plot_hyperparameter",
    size = "small",
    main = "test_myst_doc.py",
    srcs = ["test_myst_doc.py"],
    args = ["--path", "doc/source/ray-core/examples/plot_hyperparameter.ipynb"],
    data = ["//doc/source/ray-core/examples:core_examples"],
    tags = ["exclusive", "team:ml"]
)

py_test(
    name = "plot_parameter_server",
    size = "medium",
    main = "test_myst_doc.py",
    srcs = ["test_myst_doc.py"],
    args = ["--path", "doc/source/ray-core/examples/plot_parameter_server.ipynb"],
    data = ["//doc/source/ray-core/examples:core_examples"],
    tags = ["exclusive", "team:ml"]
)

py_test(
    name = "plot_pong_example",
    size = "large",
    main = "test_myst_doc.py",
    srcs = ["test_myst_doc.py"],
    args = ["--path", "doc/source/ray-core/examples/plot_pong_example.ipynb"],
    data = ["//doc/source/ray-core/examples:core_examples"],
    tags = ["exclusive", "team:ml"]
)

py_test(
    name = "progress_bar",
    main = "test_myst_doc.py",
    srcs = ["test_myst_doc.py"],
    size = "small",
    args = ["--path", "doc/source/ray-core/examples/progress_bar.ipynb"],
    data = ["//doc/source/ray-core/examples:core_examples"],
    tags = ["exclusive", "team:ml"]
)


# Directory: source/ray-core/doc_code
py_test(
    name = "doc_code_tf_example",
    size = "small",
    main = "source/ray-core/doc_code/tf_example.py",
    srcs = ["source/ray-core/doc_code/tf_example.py"],
    tags = ["exclusive", "tf", "team:ml"]
)

py_test(
    name = "doc_code_torch_example",
    size = "small",
    main = "source/ray-core/doc_code/torch_example.py",
    srcs = ["source/ray-core/doc_code/torch_example.py"],
    tags = ["exclusive", "pytorch", "team:ml"]
)

py_test(
    name = "doc_code_metrics_example",
    size = "small",
    main = "source/ray-core/doc_code/metrics_example.py",
    srcs = ["source/ray-core/doc_code/metrics_example.py"],
    tags = ["exclusive", "team:serve"]
)

py_test(
    name = "doc_code_runtime_env_example",
    size = "small",
    main = "source/ray-core/doc_code/runtime_env_example.py",
    srcs = ["source/ray-core/doc_code/runtime_env_example.py"],
    tags = ["exclusive", "post_wheel_build", "team:serve"]
)

# --------------------------------------------------------------------
# Tests from the doc/source/tune/tutorials directory.
# Please keep these sorted alphabetically.
# --------------------------------------------------------------------

py_test(
    name = "tune_sklearn",
    size = "medium",
    main = "test_myst_doc.py",
    srcs = ["test_myst_doc.py"],
    args = ["--path", "doc/source/tune/tutorials/tune-sklearn.ipynb"],
    data = ["//doc/source/tune/tutorials:tune_tutorials"],
    tags = ["exclusive", "team:ml"],
)

py_test(
    name = "tune_serve_integration_mnist",
    size = "medium",
    main = "test_myst_doc.py",
    srcs = ["test_myst_doc.py"],
    args = ["--path", "doc/source/tune/tutorials/tune-serve-integration-mnist.ipynb", "--smoke-test", "--from_scratch", "--day 0"],
    data = ["//doc/source/tune/tutorials:tune_tutorials"],
    tags = ["exclusive", "team:ml"],
)

py_test(
    name = "hyperopt_example",
    size = "small",
    main = "test_myst_doc.py",
    srcs = ["test_myst_doc.py"],
    args = ["--path", "doc/source/tune/examples/hyperopt_example.ipynb"],
    data = ["//doc/source/tune/examples:tune_examples"],
    tags = ["exclusive", "team:ml"],
)
