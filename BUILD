licenses(['notice'])

cc_library(
  name = 'gflags',
  visibility = ['//visibility:public'],
  hdrs = [
    '__build__/linux/include/gflags/gflags.h',
    '__build__/linux/include/gflags/gflags_completions.h',
    '__build__/linux/include/gflags/gflags_declare.h',
    '__build__/linux/include/gflags/gflags_gflags.h',
  ],
  srcs = [
    'src/gflags.cc',
    'src/gflags_completions.cc',
    'src/gflags_reporting.cc',
  ],
  includes = [
    '__build__/linux/include',
    '__build__/linux/include/gflags',
  ],
  linkopts = [
    '-pthread',
  ],
)
