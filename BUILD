licenses(['notice'])

config_setting(
  name = 'darwin',
  values = {
    'cpu': 'darwin',
  }
)

cc_library(
  name = 'gflags',
  visibility = ['//visibility:public'],
  deps = [
    '//external:pthread',
  ],
  srcs = [
    'src/gflags.cc',
    'src/gflags_completions.cc',
    'src/gflags_reporting.cc',
  ],
  includes = select({
    ':darwin': ['__build__/darwin/include'],
    '//conditions:default': ['__build__/linux/include'],
  }),
  copts = select({
    ':darwin': ['-iquotegflags/__build__/darwin/include/gflags'],
    '//conditions:default': ['-iquotegflags/__build__/linux/include/gflags'],
  }),
)
