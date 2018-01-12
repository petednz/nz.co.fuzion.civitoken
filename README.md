nz.co.fuzion.civitoken
======================

Fuzion Token extension for CiviCRM, that provides its users extra tokens. 

These include tokens to access membership data, like membership type, start and end dates, and status. These are particularly useful to use on your "fees due" automatic notices.

By default all tokens are enabled. If you just want some there is a setting page
(screenshot below).

*A note about country-specific address formatting*
CiviCRM has a data structure to support country-specific address formatting but
no inbuilt functionality to support this. 

The data format is that the country table has an address_format_id field. That can
be used to link to a row in civicrm_address_format which you create with
a specific format. Currently the only way to create such formats is directly
in the DB. If, however, you do create those formats, this
extension will respect them in the address blocks.


![list of tokens](docs/token_listing.png)
![list of tokens2](docs/token_listing_2.png)


Installation
-----------

Installing this extension is quite easy. You only have to:

1. Visit your `civicrm/admin/extensions` page
2. See what is your extension directory, or create one if it doesn't exist
3. Go to that directory and `git clone https://github.com/eileenmcnaughton/nz.co.fuzion.civitoken.git`
4. Change permissions and ownership of the new directory, if needed
5. Refresh the `civicrm/admin/extensions` page
6. Click on "install"
