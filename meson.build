
# project name and programming language
project ('com.github.mafin.gtk-hello', 'vala', 'c')

# create new executable, list the files we want to compile, list the dependencies we need, and install
executable (
    meson.project_name(),
    'src/App-update-1.vala',
    dependencies: [
        dependency('gtk+-3.0')
    ],
    install: true
)

# install .decktop file so the Application Menu will see it
install_data(
    join_paths('data', meson.project_name() + '.desktop'),
    install_dir: join_paths(get_option('datadir'), 'applications')
)

# install .appdata.xml file so AppCenter will see it
install_data(
    join_paths('data', meson.project_name() + '.appdata.xml'),
    install_dir: join_paths(get_option('datadir'), 'metainfo')
)
