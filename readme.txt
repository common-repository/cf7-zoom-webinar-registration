# Contact Form 7 Zoom Webinar Registration

Contributors: usamealgan
Donate link: https://paypal.me/ualgan
Tags: zoom webinars, registration, api integration
Requires at least: 4.9
Tested up to: 5.4
Stable tag: 1.0.6
License: GPLv3
License URI: https://www.gnu.org/licenses/gpl-3.0

Allow registrations for your Zoom Webinar through Wordpress Contact Form 7

## Requirements

- Zoom Account that can create webinars
- [JWT Application](https://marketplace.zoom.us/develop/create) for your Zoom Account

## Installation

1. Download the [latest release](https://github.com/usame-algan/cf7-zoom-webinar-registration/releases/latest)
2. Upload the file to your wordpress installation
3. Activate the plugin

## Setup

1. After plugin activation you can save your `API Key` and `API Secret` in the Settings Page
2. The plugin looks for field names prefixed with `cf7zwr-`. The rest of the field name should be according to the [Zoom API reference](https://marketplace.zoom.us/docs/api-reference/zoom-api/webinars/webinarregistrantcreate). For example if you want to save the first name of a registrant the field should be named `cf7zwr-first_name`
3. The webinar ID can be saved within the form settings inside the `Zoom` panel

## Additional Settings

To register users optionally add a checkbox element named `cf7zwr-confirm` to your form e.g.
`[checkbox cf7zwr-confirm "Register for this webinar"]`

## License

This plugin is licensed under the GPL v3. See `license.txt` for more information.

## Bugs

If you find any Bugs please feel free to [open an issue here](https://github.com/usame-algan/cf7-zoom-webinar-registration/issues)!

## Changelog

#### [1.0.6] - 2020-10-18
- Skips Zoom API Call if there is no webinar id present
- Checks for a field `cf7zwr-confirm` to register users optionally

#### [1.0.5] - 2020-08-07
- Fixes a bug that caused guessed fields to overwrite prefixed fields

#### [1.0.4] - 2020-08-05
- Show a notice box for missing required fields

#### [1.0.3] - 2020-06-28
- Now displays selected questions from Zoom once the webinar id has been set

#### [1.0.2] - 2020-06-28
- Added custom field for the webinar id

## Credits

This plugin was inspired by [Gravity Forms Zoom Webinar Registration](https://github.com/michaelbourne/gravity-forms-zoom-webinar-registration)