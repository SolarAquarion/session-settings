session_data = configuration_data()
autostartdir = join_paths(get_option('sysconfdir'), 'xdg', 'autostart')

session_data.set('libexecdir', join_paths(get_option('libexecdir'))

gsd_desktop = [
    'org.gnome.SettingsDaemon.A11ySettings-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.Power-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.Clipboard-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.PrintNotifications-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.Color-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.Rfkill-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.Datetime-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.Sharing-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.Housekeeping-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.Smartcard-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.Keyboard-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.Sound-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.MediaKeys-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.Wacom-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.Mouse-pantheon.desktop.in',
    'org.gnome.SettingsDaemon.XSettings-pantheon.desktop.in'.
      ]

if get_option('patched-gsd-autostarts')
    install_subdir(
        'gsd',
        install_dir: autostartdir,
        strip_directory: true
    )
endif


if get_option('patched-ubuntu-autostarts')
    install_subdir(
        'ubuntu',
        install_dir: autostartdir,
        strip_directory: true
    )
endif

