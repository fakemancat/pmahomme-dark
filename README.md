# pmahomme-dark

[Русская версия](README.ru.md)

A dark graphite theme for phpMyAdmin, based on the default `pmahomme` theme.

![pmahomme-dark preview](screen.png)

## About

`pmahomme-dark` gives phpMyAdmin a consistent dark interface while preserving the familiar layout of the default theme. It includes dark styles for navigation, tables, forms, dialogs, alerts, the SQL editor, the console, Designer, and other common interface elements.

## Compatibility

- phpMyAdmin 5.0, 5.1, and 5.2
- Theme version: 1.0
- LTR and RTL layouts

## Installation

1. Download this repository using **Code → Download ZIP**, or clone it with Git.
2. Make sure the extracted directory is named `pmahomme-dark`.
3. Copy the entire directory into the `themes` directory of your phpMyAdmin installation:

   ```text
   phpMyAdmin/
   └── themes/
       └── pmahomme-dark/
           ├── css/
           ├── img/
           ├── jquery/
           ├── scss/
           └── theme.json
   ```

4. Open phpMyAdmin and select **pmahomme-dark** from the **Theme** selector on the home page.

Do not replace or remove the original `pmahomme` directory. The new theme must be installed alongside it.

### Make it the default theme

Add the following setting to `config.inc.php`:

```php
$cfg['ThemeDefault'] = 'pmahomme-dark';
```

If the theme selector is not visible, make sure the theme manager is enabled:

```php
$cfg['ThemeManager'] = true;
```

For more details, see the [official phpMyAdmin custom themes documentation](https://docs.phpmyadmin.net/en/release_5_2_0/themes.html).

## Updating

Replace the existing `themes/pmahomme-dark` directory with the files from the new version, then refresh phpMyAdmin. If old styles remain, clear your browser cache.

## Uninstalling

Switch to another theme first, then remove the `themes/pmahomme-dark` directory. Also remove or change the `ThemeDefault` setting if you added it.
