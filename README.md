## Attention!

Because I was lucky enough to be able to dump php completely this repository is no longer under development!
If you want to take over as maintainer, just drop me a line.

SugarCRM Client PHP Library
===========================

This library intends to provide a simpler interface for the rest api
of [sugarcrm](http://www.sugarcrm.com).

The development of the library was sponsored by the following companies:

* [Supremesurf](http://www.supremesurf.de)
* [Telematika GmbH](http://www.telematika.de)

The source of this library is released under the BSD license (see COPYING for details).

Requirements
------------

* PHP 5.3
* curl (php-curl)

Usage
-----

Just include the needed php files and initialize the sugarcrm connection object.

    <?php
    require_once('sugarcrmclient.php');
    $sugar = new \SugarCRM\Connection("http://crm.example.com", "user", "password");
    $p = $sugar->load_bean('Contacts', '6efc52c4-3c6a-8787-3284-4fabee55b834');
