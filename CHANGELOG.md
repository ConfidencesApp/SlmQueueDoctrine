# 1.0.0

- Identical to 0.7.0

# 0.7.0

- [BC] Synchronize with SlmQueue release 0.7.0 which adds the ability to store binary data in job content

# 0.6.1

- Fixes an issue with timezones
- Adds support for microtimes

# 0.6.0

- [BC] Synchronize with SlmQueue release 0.6.0 which adds compatibility with PHP7, zend-servicemanager 3 and zend-eventmanager 3

# 0.5.0

- [BC] Minimum dependency has been raised to PHP 5.5
- Project has been migrated to PSR-4

# 0.4.0

- First stable release in 0.4.x branch

# 0.4.0-beta3

* [BC] Due to changes in SlmQueue ([changelog](https://github.com/juriansluiman/SlmQueue/blob/master/CHANGELOG.md)) existing jobs won't be able to be executed correctly.

# 0.4.0-beta1

* [BC] SlmQueueDoctrine has been upgraded to SlmQueue 0.4. This feature includes a new, flexible and modular event system.

# 0.3.0

* Initial release for 0.3.* branch

# 0.3.0-beta1

First release of SlmQueueDoctrine which bring it on par with its parent SlmQueue 0.3.0-beta1

Comes with unittests, bug fixes and general happiness but please be aware of the following, if you are upgrading from an earlier version...

- Existing jobs are not compatible (Job content is now serialized). Make sure you empty the queue before upgrading.
- It is suggested that you recreate the table from data/queue_default.sql as the schema changed in minor ways.
- The ability to configure the queue defaults has been removed. Any queue specific configuration now goes into the queues configuration of slm_queue.local.php

	
	

