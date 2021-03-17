# RecentChangesWebhooks

This is an extension that, very simply, allows adding webhooks to recent changes.

## Installation

From the root directory of your wiki, run the following commands:
```
cd extensions
git clone https://github.com/Kenny2github/RecentChangesWebhooks.git
```
Then add the following line to your LocalSettings.php:
```php
wfLoadExtension( 'RecentChangesWebhooks' );
```

## Configuration
`$wgRCWHookUrls` - an array containing the URLs of the web hooks to be triggered when a change has been made
`$wgRCWHookType` - either `realtime` or `job` to determine whether the webhook should be run synchronously with page edits or in a job