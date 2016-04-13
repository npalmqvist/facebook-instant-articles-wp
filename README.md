# Instant Articles for WP

Enable [Instant Articles for Facebook](https://developers.facebook.com/docs/instant-articles) on your WordPress site.

## Description

This plugin adds support for Instant Articles for Facebook, which is a new way for publishers to distribute fast, interactive stories on Facebook. Instant Articles are preloaded in the Facebook mobile app so they load instantly.

With the plugin active, a new menu will be available for you to connect to your Facebook Page and start publishing your Instant Articles. You'll also see the status of each Instant Articles submission on the edit page of your posts.

## Feed submission to Facebook

Facebook has a review process where they verify that all Instant Articles are properly formatted, have content consistency with their mobile web counterparts, and adhere to their community standards and content policies. You will not be able to publish Instant Articles in Facebook until your feed has been approved.

It's important to note that if you use meta fields to add extra text, images or videos to your Posts, Facebook will expect you to add these to your Instant Articles output too. This plugin includes hooks to help you do that.

[See Facebook's documentation for full details of the submission process.](https://developers.facebook.com/docs/instant-articles)

Facebook requires a minimum number of articles in your feed before they will review it. Once your feed has been approved, new posts will automatically be taken live on Instant Articles, and existing posts will be taken live once you update them.

## Installation

1. Run `composer install` on the root of the plugin folder. Make sure you have [Composer](https://github.com/composer/composer) installed.
2. Upload the folder to the `/wp-content/plugins/` directory
3. Activate the plugin through the 'Plugins' menu in WordPress

## Frequently Asked Questions

**How do I customize the output for my site?**

There are a number of filters available in the plugin for modifying the output.

**How do I post articles to Instant Articles after plugin is installed?**

You can re-publish existing articles (simply edit + save) or post new articles in order to submit them to Instant Articles. After you have 50 articles added, you will be able to submit them for review.

**How do I change the feed slug/URL if I'm using the RSS integration?**

To change the feed slug, set the constant INSTANT_ARTICLES_SLUG to whatever you like. If you do, remember to flush the rewrite rules afterwards.
By default it is set to `instant-articles` which usually will give you a feed URL set to `/feed/instant-articles`

**How do I flush the rewrite rules after changing the feed slug?**

Usually simply visiting the permalinks settings page in the WordPress dashboard will do the trick (/wp-admin/options-permalink.php)
