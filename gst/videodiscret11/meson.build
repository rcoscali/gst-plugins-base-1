videodiscret11_sources = [
  'gstvideodiscret11.c',
]

gstvideodiscret11 = library('gstvideodiscret11',
  videodiscret11_sources,
  c_args : gst_plugins_base_args,
  include_directories: [configinc, libsinc],
  dependencies : glib_deps + [video_dep, gst_dep, gst_base_dep],
  install : true,
  install_dir : plugins_install_dir,
)
pkgconfig.generate(gstvideodiscret11, install_dir : plugins_pkgconfig_install_dir)
plugins += [gstvideodiscret11]
