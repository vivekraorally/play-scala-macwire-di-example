rules_play_routes_version = "cba8a4383d81e6519730ba2b0203f74fd2c9b765"

http_archive(
  name = "io_bazel_rules_play_routes",
  url = "https://github.com/lucidsoftware/rules_play_routes/archive/%s.zip"%rules_play_routes_version,
  type = "zip",
  strip_prefix= "rules_play_routes-%s" % rules_play_routes_version
)

maven_jar(
    name = "scala_test_maven",
    artifact = "org.scalatestplus.play:scalatestplus-play_2.12:3.1.2",
)

maven_jar(
    name = "macwire",
    artifact = "com.softwaremill.macwire:macros_2.12:2.3.1",
)

bind(
  name = "scala_test",
  actual = "@scala_test_maven//jar"
)