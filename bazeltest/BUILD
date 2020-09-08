load("@io_bazel_rules_scala//scala:scala.bzl", "scala_library", "scala_test")
 
scala_library(
   name = "bazeltest",
   srcs = ["src/main/scala/bazeltest/Main.scala"],
   deps = [
       "//othermodule",
       "//3rdparty/jvm/joda_time:joda_time"
   ],
   visibility = ["//:__pkg__"]
)
 
scala_test(
    name = "test-main",
    srcs = ["src/test/scala/bazeltest/MainSpec.scala"],
    deps = [":bazeltest"]
)
