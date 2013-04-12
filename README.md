# MVP

MVP (Most Valuable apP), generates a ranked list of currently installed
iOS app on your devices based on their release or purchase date. The idea is
that the older an app is and still installed on your device, the higher its
value for you as it's assumed you still use it (built-in apps from Apple are
obviously excluded as can't be purchased, luckily).

# Usage

Download and run the script:

    $ ./mvp --help

# Caveats

* You need to have a iOS device backup available locally
* You need to have all purchased apps downloaded
* Some apps are listed by their latest update's "purchase" date instead of
  original purchase date

# How it works

A device backup contains a list of all currently installed app. All downloaded
apps contain their release & purchase date. The script joins the list of
installed apps with the release & purchase dates and sorts it.

To my knowledge there is currently no other way (e.g. API) to retrieve a list
of purchased and installed apps on an iOS device.

# Privacy

The script is open-source and requires no internet connection. No credentials
are exposed.

# LICENSE

MIT License.
