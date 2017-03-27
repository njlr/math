include_defs('//BUCKAROO_DEPS')

# TODO: Do we need to compile src/tr1? 
prebuilt_cxx_library(
  name = 'math',
  header_only = True,
  header_namespace = 'boost',
  visibility = [
    'PUBLIC',
  ],
  deps = BUCKAROO_DEPS,
  exported_deps = [
    ':boost-math-no-deps',
  ],
)

prebuilt_cxx_library(
  name = 'boost-math-no-deps',
  header_only = True,
  header_namespace = 'boost',
  exported_headers = subdir_glob([
    ('include/boost', '**/*.hpp'),
  ]),
  visibility = [
    'PUBLIC',
  ],
)
