# Change Log

All notable changes to this project will be documented in this file.

[Unreleased]
- Added new integration for Travis CI.
- Added settings option to control maximum file upload size.
- Added support for running Zulip development environment in Docker.
- Recent private message threads are now displayed like recent topics.
- Made it possible to set LDAP and EMAIL_HOST passwords in
  /etc/zulip/secrets.conf.
- Improved the styling for the Administration page.
- Substantially improved loading performance on slow networks by enabling
  GZIP compression on more assets.
- Changed the page title in narrowed views to include the current narrow.
- Fixed bugs where draft compose content might be lost when reloading site.
- Fixed support for disabling the "zulip" notifications stream.
- Fixed missing step in postfix_localmail installation instructions.
- Substantially cleaned up console logging from run-dev.py.

[1.3.9] - 2015-11-16
- Fixed buggy #! lines in upgrade scripts.

[1.3.8] - 2015-11-15
- Added options to the Python api for working with untrusted server certificates.
- Added a lot of documentation on the development environment and testing.
- Added partial support for translating the Zulip UI.
- Migrated installing Node dependencies to use npm.
- Fixed LDAP integration breaking autocomplete of @-mentions.
- Fixed admin panel reactivation/deactivation of bots.
- Fixed inaccurate documentation for downloading the desktop apps.
- Fixed various minor bugs in production installation process.
- Fixed security issue where recent history on private streams might
  be visible to new users (to the Zulip team) who were invited with that
  private stream as one of their initial streams
  (https://github.com/zulip/zulip/issues/230).
- Major preliminary progress towards supporting Python 3.

[1.3.7] - 2015-10-19
- Turn off desktop and audible notifications for streams by default.
- Added support for the LDAP authentication integration creating new users.
- Added new endpoint to support Google auth on mobile.
- Fixed desktop notifications in modern Firefox.
- Fixed several installation issues for both production and development environments.
- Improved documentation for outgoing SMTP and the email mirror integration.
