add_library(littlefs
  lfs.c
  lfs_util.c
  )

target_compile_options(littlefs PUBLIC
  $<$<COMPILE_LANGUAGE:C>:${BUILD_FLAGS_FOR_C}>
)

target_include_directories(littlefs PUBLIC .)
