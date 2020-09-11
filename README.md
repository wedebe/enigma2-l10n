# enigma2-l10n
Aggregation of popular e2 image language files into a simple, (almost-)visual format.

- [openATV](https://github.com/openatv/enigma2/tree/6.4/po)
- [OpenHDF](https://github.com/openhdf/enigma2/tree/master/po)
- [OpenPLi](https://github.com/openpli/enigma2/tree/develop/po)
- [OpenViX](https://github.com/openvix/enigma2/tree/master/po)

Currently, each po folder needs to be saved manually to 
`enigma2-l10n/po/reference/[IMAGE_NAME]`

[IMAGE_NAME] will be used as the header.

Generated output will be saved to 
`enigma2-l10n/aggregated/[POFILE_NAME].csv` (eg. `en.po.csv`)

An example...
en.po.csv (with made up data)

||openatv|openhdf|openpli|openvix|*[IMAGE_NAME]*|
|---|---|---|---|---|---|
*msgid*|*msgstr*|*msgstr*|*msgstr*|*msgstr*||
ffwd|Fast Forward|FFWD|Fast Forward|FAST FWD||
play|PLAY||Play|''||

`Blank` entries don't feature that particular `msgid` in that image's translation (po file)

`''` entries feature, but haven't been translated

So far, translations are only read into each individual language's csv file. 
The intention is to enable simpler bulk modifying/saving of po translation files 
from an aggregated csv file.
