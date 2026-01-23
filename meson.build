project(
    'vubar',
    ['c'],
    default_options: ['c_std=c99'],
    version: '1.0',
    license: 'GPL-2.0',
)

c_args = [
    '-Wall',
    '-Wextra',
    '-O2',
    '-D_GNU_SOURCE',
]

# libraries

app_deps = [
    dependency('gtk+-3.0'),
    dependency('libpulse-simple'),
]

app_sources = [
    'gui.c',
    'vu.c',
]

executable(
    meson.project_name(),
    c_args: c_args,
    dependencies: app_deps,
    sources: app_sources,
    install: true,
)


