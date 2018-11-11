# Project name and programming language
project('com.github.jaywooTM.MyAppAgain', 'vala', 'c')

# Create a new executable
executable(
    meson.project_name(),
    'src/Application.vala',
    depencies: [
        depency('gtk+-3.0')
    ],
    install: true
)

# Install the .desktop for the Application Menu
install_data(
    join_paths('data', meson.project_name() + '.desktop'),
    install_dir: join_paths(get_option('datadir'), 'applications')
)

# Install .appdata.xml for AppCenter
install_data(
    join_paths('data', meson.project_name() + '.appdata.xml'),
    install_dir: join_paths(get_option('datadir'), 'metainfo')
)
