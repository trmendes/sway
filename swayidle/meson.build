threads = dependency('threads')

executable(
	'swayidle', [
		'main.c',
	],
	include_directories: [sway_inc],
	dependencies: [
		client_protos,
		pixman,
		wayland_client,
		wayland_server,
		wlroots,
		swayidle_deps,
	],
	link_with: [lib_sway_common, lib_sway_client],
	install_rpath : rpathdir,
	install: true
)
