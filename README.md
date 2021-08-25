# Drupal-Settings
Kint-debug-settings

Improve the kint debug time and depth.

    // Include Kint class.
    include_once(DRUPAL_ROOT . '/modules/contrib/devel/kint/kint/Kint.class.php');

    // If debugging is very slow or leads to WSOD reduce the number
    // of levels of information shown by Kint.
    // Change Kint maxLevels setting:
    if (class_exists('Kint')){
      // Set the maxlevels to prevent out-of-memory. Currently there doesn't seem to be a cleaner way to set this:
      Kint::$maxLevels = 4;
    }
-----------------------------------------------------------------------------------------------------------------------------

template suggestion for theming in Drupal 8. 

    In project/path/to/sits/default/serivces.yml   
    debug: True
    cache: false
-----------------------------------------------------------------------------------------------------------------------------

