ExternalProject_Add(
  ext_frei0r
  DOWNLOAD_DIR ${EXT_DOWNLOAD_DIR}
  GIT_REPOSITORY https://github.com/dyne/frei0r.git

  CMAKE_ARGS ${CMAKE_GLOBAL_PROFILE} -DWITHOUT_OPENCV:BOOL=ON
  DEPENDS ext_ffmpeg
)
