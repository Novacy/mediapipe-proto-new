package(default_visibility = ["//visibility:public"])

licenses(["notice"])

cc_library(
    name = "detections_to_rects",
    srcs = ["detections_to_rects.cc"],
    hdrs = ["detections_to_rects.h"],
    deps = [
        "//mediapipe/calculators/util:alignment_points_to_rects_calculator",
        "//mediapipe/calculators/util:detections_to_rects_calculator",
        "//mediapipe/calculators/util:detections_to_rects_calculator_cc_proto",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/formats:detection_cc_proto",
        "//mediapipe/framework/formats:rect_cc_proto",
    ],
)

cc_test(
    name = "detections_to_rects_test",
    srcs = ["detections_to_rects_test.cc"],
    deps = [
        ":detections_to_rects",
        "//mediapipe/framework:calculator_framework",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/formats:detection_cc_proto",
        "//mediapipe/framework/formats:rect_cc_proto",
        "//mediapipe/framework/port:gtest",
        "//mediapipe/framework/port:gtest_main",
        "//mediapipe/framework/port:parse_text_proto",
        "//mediapipe/framework/port:status_matchers",
    ],
)

cc_library(
    name = "landmarks_to_detection",
    srcs = ["landmarks_to_detection.cc"],
    hdrs = ["landmarks_to_detection.h"],
    deps = [
        "//mediapipe/calculators/util:landmarks_to_detection_calculator",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/formats:detection_cc_proto",
        "//mediapipe/framework/formats:landmark_cc_proto",
    ],
)

cc_test(
    name = "landmarks_to_detection_test",
    srcs = ["landmarks_to_detection_test.cc"],
    deps = [
        ":landmarks_to_detection",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/formats:detection_cc_proto",
        "//mediapipe/framework/formats:landmark_cc_proto",
        "//mediapipe/framework/port:gtest",
        "//mediapipe/framework/port:gtest_main",
        "//mediapipe/framework/port:parse_text_proto",
        "//mediapipe/framework/port:status",
        "//mediapipe/framework/port:status_matchers",
    ],
)

cc_library(
    name = "landmarks_projection",
    srcs = ["landmarks_projection.cc"],
    hdrs = ["landmarks_projection.h"],
    deps = [
        "//mediapipe/calculators/util:landmark_projection_calculator",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/formats:landmark_cc_proto",
    ],
)

cc_test(
    name = "landmarks_projection_test",
    srcs = ["landmarks_projection_test.cc"],
    deps = [
        ":landmarks_projection",
        "//mediapipe/framework:calculator_framework",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/formats:landmark_cc_proto",
        "//mediapipe/framework/port:gtest",
        "//mediapipe/framework/port:gtest_main",
        "//mediapipe/framework/port:parse_text_proto",
        "//mediapipe/framework/port:status",
        "//mediapipe/framework/port:status_matchers",
    ],
)

cc_library(
    name = "loopback",
    hdrs = ["loopback.h"],
    deps = [
        "//mediapipe/calculators/core:previous_loopback_calculator",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/api2:port",
    ],
)

cc_test(
    name = "loopback_test",
    srcs = ["loopback_test.cc"],
    deps = [
        ":loopback",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/api2:node",
        "//mediapipe/framework/api2:port",
        "//mediapipe/framework/port:gtest",
        "//mediapipe/framework/port:gtest_main",
        "//mediapipe/framework/port:parse_text_proto",
        "//mediapipe/framework/port:status_matchers",
    ],
)

cc_library(
    name = "image_size",
    hdrs = ["image_size.h"],
    deps = [
        "//mediapipe/calculators/image:image_properties_calculator",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/api2:port",
        "//mediapipe/framework/formats:image",
        "//mediapipe/framework/formats:image_frame",
        "//mediapipe/gpu:gpu_buffer",
    ],
)

cc_test(
    name = "image_size_test",
    srcs = ["image_size_test.cc"],
    deps = [
        ":image_size",
        "//mediapipe/framework:calculator_framework",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/formats:image",
        "//mediapipe/framework/formats:image_frame",
        "//mediapipe/framework/port:gtest",
        "//mediapipe/framework/port:gtest_main",
        "//mediapipe/framework/port:parse_text_proto",
        "//mediapipe/framework/port:status_matchers",
        "//mediapipe/gpu:gpu_buffer",
    ],
)

cc_library(
    name = "rect_transformation",
    srcs = ["rect_transformation.cc"],
    hdrs = ["rect_transformation.h"],
    deps = [
        "//mediapipe/calculators/util:rect_transformation_calculator",
        "//mediapipe/calculators/util:rect_transformation_calculator_cc_proto",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/formats:rect_cc_proto",
        "@com_google_absl//absl/types:optional",
    ],
)

cc_test(
    name = "rect_transformation_test",
    srcs = ["rect_transformation_test.cc"],
    deps = [
        ":rect_transformation",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/formats:rect_cc_proto",
        "//mediapipe/framework/port:gtest",
        "//mediapipe/framework/port:gtest_main",
        "//mediapipe/framework/port:parse_text_proto",
    ],
)

cc_library(
    name = "threshold",
    srcs = ["threshold.cc"],
    hdrs = ["threshold.h"],
    deps = [
        "//mediapipe/calculators/util:thresholding_calculator",
        "//mediapipe/calculators/util:thresholding_calculator_cc_proto",
        "//mediapipe/framework/api2:builder",
    ],
)

cc_test(
    name = "threshold_test",
    srcs = ["threshold_test.cc"],
    deps = [
        ":threshold",
        "//mediapipe/framework:calculator_framework",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/port:gtest",
        "//mediapipe/framework/port:gtest_main",
        "//mediapipe/framework/port:parse_text_proto",
        "//mediapipe/framework/port:status_matchers",
    ],
)

cc_library(
    name = "split",
    hdrs = ["split.h"],
    deps = [
        "//mediapipe/calculators/core:split_proto_list_calculator",
        "//mediapipe/calculators/core:split_vector_calculator",
        "//mediapipe/calculators/core:split_vector_calculator_cc_proto",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/api2:port",
        "//mediapipe/framework/formats:body_rig_cc_proto",
        "//mediapipe/framework/formats:classification_cc_proto",
        "//mediapipe/framework/formats:detection_cc_proto",
        "//mediapipe/framework/formats:landmark_cc_proto",
        "//mediapipe/framework/formats:matrix",
        "//mediapipe/framework/formats:rect_cc_proto",
        "//mediapipe/framework/formats:tensor",
        "@org_tensorflow//tensorflow/lite/c:common",
    ],
)

cc_test(
    name = "split_test",
    srcs = ["split_test.cc"],
    deps = [
        ":split",
        "//mediapipe/framework:calculator_framework",
        "//mediapipe/framework/api2:builder",
        "//mediapipe/framework/formats:landmark_cc_proto",
        "//mediapipe/framework/formats:rect_cc_proto",
        "//mediapipe/framework/formats:tensor",
        "//mediapipe/framework/port:gtest",
        "//mediapipe/framework/port:gtest_main",
        "//mediapipe/framework/port:parse_text_proto",
        "//mediapipe/framework/port:status_matchers",
    ],
)
