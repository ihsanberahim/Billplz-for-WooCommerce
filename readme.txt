=== Billplz for WooCommerce ===
Contributors: wanzulnet
Tags: billplz
Tested up to: 5.3
Stable tag: 3.23.2
Donate link: http://billplz.com/join/lz7pmrxa45tiihvqdydxqq/
Requires at least: 4.6
License: GPL-3.0-or-later
License URI: http://www.gnu.org/licenses/gpl-2.0.html
Requires PHP: 5.2.4

Accept payment by using Billplz.

== Description ==
Install this plugin to accept payment using Billplz.

== Upgrade Notice ==

= 3.22.0 =
* Customizing the input fields for skip bill page feature will require minor adjustment due to changes in API from Get FPX Banks to Get Payment Gateways.

== Screenshots ==
* Billplz for WooCommerce installation
* Activate plugin after installation
* Set API Secret Key, Collection ID and X Signature Key
* Enable X Signature Key at [Billplz Account Settings](https://www.billplz.com/enterprise/setting)

== Changelog ==

= 3.23.2 =
* FIXED: Issue with new PayPal account not displaying on checkout page when Bypass Billplz Page setting is on.
* NEW: Bump WooCommerce version support to 4.0.

= 3.23.1 =
* FIXED: Undefined index for clear cart key

= 3.23.0 =
* IMPROVED: Remove special character on name to avoid X Signature calculation failure.
* IMPROVED: Cart session are removed by default.
* IMPROVED: No requery will be made upon redirect and callback.
* REMOVED: Requery all order status due to performance impact.
* REMOVED: Bill notification feature is now always disabled.
* REMOVED: Auto detect mode. Now merchant need to tick on Sandbox to use sandbox mode.

= 3.22.1 =
* FIXED: Order status callback not functioning when customer name has single quote.

= 3.22.0 =
* ADDED: Added support for all available payment methods. Custom integration should refer to upgrade notice for details.
* IMPROVED: Using transient instead of normal wp option for storing payment method availability.

= 3.21.9 =
* IMPROVED: Add bfw_filter_order_data filter
* IMPROVED: Auto disable plugin when using other than MYR Currency
* IMPROVED: Webhook to have 403 forbidden status code if X Signature comparison failed
* REMOVED: Support for WooCommerce 2.x

= 3.21.8.1 =
* IMPROVED: Removed Boost e-wallet as a default title

== Installation ==

**Step 1:**

- Login to your *WordPress Dashboard*
- Navigate to **Plugins >> Add New**
- Search **Billplz for WooCommerce >> Install Now**

**Step 2:**

- Activate Plugin

**Step 3:**

- Navigate to **WooCommerce >> Settings >> Checkout >> Billplz**
- Insert your **API Secret Key**, **Collection ID** and **X Signature Key**
- Save changes

== Frequently Asked Questions ==


= Where can I get API Secret Key? =

You can the API Secret Key at your Billplz Account Settings. [Get it here](https://www.billplz.com/enterprise/setting)

= Where can I get Collection ID? =

You can the Collection ID at your Billplz >> Billing. [Get it here](https://www.billplz.com/enterprise/billing)

= Where can I get X Signature Key? =

You can the X Signature Key at your Billplz Account Settings. [Get it here](https://www.billplz.com/enterprise/setting)

= Troubleshooting =

1. If you are not getting a **Callback/Redirect** response from Billplz:

	Please make sure you have **Tick "Enable XSignature Payment Completion"** on Billplz Account Settings and make sure you have set your **X Signature Key**.

2. To immediately reduce stock on add to cart, we strongly recommend you to use [WooCommerce Cart Stock Reducer](http://bit.ly/1UDOQKi) plugin.

== Links ==
[Sign Up](https://www.billplz.com/join/lz7pmrxa45tiihvqdydxqq/) for Billplz account to accept payment using Billplz now!
