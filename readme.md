### DPC SDP - TIDE

To install use:

> composer create-project drupal/recommended-project:9.5.9 my_site_name_dir

Copy the composer.json on top of the one inside my_site_name_dir

> drush site-install tide --db-url=mysql://user:pass@localhost/dpc_sdp --account-name=admin --account-pass=pass

This will normally be fine but can run into installation issues, related to wysiwyg_template.

Use the browser install method instead and when it runs into an error with the aforementioned module run:

> drush pm:enable wysigyg_template

The version of simple_sitemap is not supported properly and will return an error but the profile should install just fine.
