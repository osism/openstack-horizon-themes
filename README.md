# openstack-themes

https://docs.openstack.org/horizon/latest/configuration/themes.html

All themes in this repository are pre-installed in our OSISM Horizon
image.

To use a specific theme, it must be explicitly made known via the
``custom_local_settings`` file.

For example, to offer the ``default`` and ``regiocloud`` themes in one
environment, the following is added to the configuration repository in
``environments/kolla/files/overlays/custom_local_settings``.

```
AVAILABLE_THEMES = [
    ('default', 'Default', 'themes/default'),
    ('regiocloud', 'REGIO.cloud', 'themes/regiocloud'),
]
```

We are happy to include any themes you like. For each theme a single
contact person must be defined. The theme providers are responsible for
its functionality. Especially in case of updates from the Horizon image.

There are no backports, rebuilds or similar from the Horizon image in
case of errors or updates in the themes.

Each provider of a theme is fully responsible and liable for the content
in their theme.

We reserve the right to remove themes in the future.

## Sample screenshots

### regiocloud

![Horizon login](screenshots/regiocloud.png?raw=true "Horizon login")
