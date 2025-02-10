# Kobo-Essentials
Tools I consider essentials to get the most out of your Kobo eReader

# Line than needs to be added to Kobo eReader.conf
```
[FeatureSettings]
ExcludeSyncFolders=(\\.(?!kobo|adobe).+|([^.][^/]*/)+\\..+)
```

# Content of my custom NickelMenu "Menu" should be a good start
```
experimental :menu_main_15505_icon :/mnt/onboard/.adds/nm/.icon.png
experimental: menu_main_15505_label : +NM+

menu_item    : main                  : KOReader+            : cmd_spawn        :quiet       :exec /mnt/onboard/.adds/koreader/koreader.sh
menu_item    : main                  : Dark Mode            : nickel_setting   : toggle     : dark_mode
menu_item    : main                  : Screenshots          : nickel_setting   : toggle     : screenshots
menu_item    : main                  : Import books         : nickel_misc      : rescan_books_full
menu_item    : main                  : Reboot               : power            : reboot
menu_item    : main                  : Shutdown             : power            : shutdown
menu_item    : main                  : WiFi On/Off          : nickel_setting   : toggle     : force_wifi
                                       chain_success        : nickel_wifi      : toggle
menu_item    : main                  : USB Connect          : nickel_misc      : force_usb_connection
# ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- #
menu_item    : reader                : Dark Mode            : nickel_setting   : toggle     : dark_mode
menu_item    : reader                : Screenshots          : nickel_setting   : toggle     : screenshots
menu_item    : reader                : Goodreads            : nickel_browser   : https://www.goodreads.com/book
menu_item    : reader                : USB Connect          : nickel_misc      : force_usb_connection
# ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- #
menu_item    : library               : Dark Mode            : nickel_setting   : toggle     : dark_mode
menu_item    : library               : Screenshots          : nickel_setting   : toggle     : screenshots
menu_item    : library               : Import books         : nickel_misc      : rescan_books_full
menu_item    : library               : Reboot               : power            : reboot
menu_item    : library               : Shutdown             : power            : shutdown
menu_item    : library               : WiFi On/Off          : nickel_setting   : toggle     : force_wifi
                                       chain_success        : nickel_wifi      : toggle
menu_item    : library               : USB Connect          : nickel_misc      : force_usb_connection
```