# Primer.style octicons for jinja templates

Each of the icons are in a macro where the macro is the same as the icon name
(dashes are replaced with an underscore).


### Usage

* Store the macro file, `icons.html`, in somewhere appropriate in your `templates`
folder; e.g. `macros/icons.html`. Simply `wget` the file from github (raw) into
your own desired folder.
* Import the macro into your template or into a base file if you have one. 
`{% import 'macros/icons.html' as icons %}`
* Import an icon as follows. `{{ icons.alert() }}`

* By default the size will be 16px. However you can scale it, e.g. if you want it
to be 32px then import it as follows. `{{ icons.alert(scale=2) }}`
* Add custom classes to the SVG: `{{ icons.alert(classes="octicon border other") }}`


