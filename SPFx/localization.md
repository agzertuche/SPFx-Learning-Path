Location files are in JSON format
They work similar as Resources files (XML) on VS Solution
The default language is English (en-us)
Developers can test the locale by:
Updating write-manifests.json file
{  "cdnBasePath": "<!-- PATH TO CDN -->",  "debugLocale": “es-mx"}
Or by using the “locale” command argument
gulp serve --locale=es-mx

Note: the documentation of this feature is still in progress.
