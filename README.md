# ISX #

Welcome to the [Inno Setup installer](http://www.jrsoftware.org/isinfo.php) eXtensions collection.

This collection contains scripts which extend the functionality of the Inno Setup installer.

Head to the [download](https://bitbucket.org/fougas/isx/downloads) page to obtain the latest ISX snapshot.

The extension's generic usage procedure is as follows:

. Put the extension's _.iss_ source alongside the custom Inno Setup script.
. Add the _[Code]_ section to the custom script.
. Slurp the extension source with the _#include_ directive in the above section.
. Write the extension-specific custom hook procedure(s) below the _#include_ directive. Consult the _<extension>_example.iss_ sample script for the details.

### Path.iss ###

The extension to manipulate the PATH environment variable.

This extension allows to prepend/append the entries to either system wide or current user's path.
It also performs the path cleanup upon uninstallation.
A path entry can be added either unconditionally or when specific component or task is enabled.

Refer to _path_example.iss_ sample script for more info.

If this extension does not suit you, there is an eariler work [ModPath](http://www.legroom.net/software/modpath) worth considering.



_Happy hacking & have fun!_

Oleg A. Khlybov <fougas@mail.ru>