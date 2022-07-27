package(default_visibility = ["//visibility:public"])

objc_library(
    name = "GTMSessionFetcher",
    module_name = "GTMSessionFetcher",
    deps = [
        ":Core",
        ":Full",
        ":LogView",
    ],
)

objc_library(
    name = "Core",
    srcs = glob([
        "Sources/Core/**/*.h",
        "Sources/Core/**/*.m",
    ]),
    hdrs = glob([
        "Sources/Core/Public/GTMSessionFetcher/*.h",
    ]),
    includes = [
        "Sources/Core/Public",
    ],
    module_name = "Core",
    sdk_frameworks = [
        "Security",
    ],
)

objc_library(
    name = "Full",
    srcs = glob([
        "Sources/Full/**/*.h",
        "Sources/Full/**/*.m",
    ]),
    hdrs = glob([
        "Sources/Full/Public/GTMSessionFetcher/*.h",
    ]),
    includes = [
        "Sources/Full/Public",
    ],
    module_name = "Full",
    deps = [
        ":Core",
    ],
)

objc_library(
    name = "LogView",
    srcs = glob([
        "Sources/LogView/**/*.h",
        "Sources/LogView/**/*.m",
    ]),
    hdrs = glob([
        "Sources/LogView/Public/GTMSessionFetcher/*.h",
    ]),
    includes = [
        "Sources/LogView/Public",
    ],
    module_name = "LogView",
    deps = [
        ":Core",
    ],
)
