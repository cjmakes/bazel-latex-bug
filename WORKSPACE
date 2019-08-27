load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive", "http_file")

# Latex
commit = "aa33f92fc7a0c93f7d19e2bae89123f30bdf3611"
http_archive(
    name = "bazel_latex",
    strip_prefix = "bazel-latex-%s" % commit,
    urls = ["https://github.com/ProdriveTechnologies/bazel-latex/archive/%s.tar.gz" % commit],
    sha256 = "abd798e02301f30ac3f031ba70757fabc343936a5e17f6cedd0e3666a72ac8e8",
)

load("@bazel_latex//:repositories.bzl", "latex_repositories")

latex_repositories()

