# gcs_translations
Translations of the GCS interface text into other languages

### Organization

Translations for each release are kept in their own sub-folder named for that release. You can attempt to use translations made for a GCS release other than the one you are currently using. The worst that will happen is that some text will not be translated and will instead show up as American English again.

### How do I use these translations?

The language files are named using the language code and the **.i18n** extension. For example, a German translation would reside in a file named **de.i18n**, since **de* is the language code used for German.

Copy the appropriate language file into the GCS **i18n** directory found in the GCS release package and re-launch GCS. GCS only reads the contents of these files once, at startup, so any changes made to them will not be noticed until you quit and re-launch.

### How do I create my own translations?

If you'd like to provide a translation for a language you are fluent in, copy the **template.i18n** file in the **i18n** directory and name it for your language (e.g. **de.i18n** for German), then edit its contents, updating the **v:** values to have the translation for the **k:** values. The file itself has more details about how to edit it. If you have questions, feel free to contact me about this.
