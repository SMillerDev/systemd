# SPDX-License-Identifier: LGPL-2.1-or-later

fundamental_path = meson.current_source_dir()

fundamental_headers = files(
        'bootspec-fundamental.h',
        'efivars-fundamental.h',
        'macro-fundamental.h',
        'sha256.h',
        'string-util-fundamental.h',
        'types-fundamental.h')

sources = '''
        bootspec-fundamental.c
        efivars-fundamental.c
        string-util-fundamental.c
        sha256.c
'''.split()

# for sd-boot
fundamental_source_paths = []
foreach source : sources
        fundamental_source_paths += meson.current_source_dir() / source
endforeach

# for libbasic
fundamental_sources = files(sources) + fundamental_headers
