#    CVE-Search Changelog

##   What's new in CVE-Search v2.1?

 * Plug-in manager bugfixes and features
 * Use datetime objects in the database
 * password change option in web interface
 * code revision
 
The upgrade from CVE-Search v1.x or v2 to v2.1 requires a database refill. Run the `./sbin/db_updater` script with the `-f` option to do this and keep the user data.

**Note:** The above comand might influence the database dates. If you wish to keep the dates as-is, read the steps [here](v2_to_v2.1/db_actions.md)

##   What's new in CVE-Search v2?

 * Plug-in manager
   * Seen, Bookmarks and MISP have been moved to plug-ins. See [our plug-in repo](https://github.com/cve-search/Plugins)
 * Bugfixes
 * Master pages
 * Working towards Windows compatibility
 * Internal working restructuring
   * Database abstraction
   * Database searching
   * Function streamlining
 * CWE browser
 * User requests
   * Posibility to view last update log in web interface
   * Minimal update (only CVE and CPE)

The update from CVE-Search v1.x to v2 will require database modifications if you wish to keep user data. The database does not have to be re-imported, but collections have to be moved around. [You can find the steps here](v1_to_v2/db_actions.md)
