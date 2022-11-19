# gcs_translations
Translations of the GCS interface text into other languages

### Organization

Translations for each release are kept in their own sub-folder named for that release. You can attempt to use translations made for a GCS release other than the one you are currently using. The worst that will happen is that some text will not be translated and will instead show up as American English again.

### How do I use these translations?

The language files are named using the language code and the `.i18n` extension. For example, a German translation would reside in a file named `de.i18n`, since `de` is the language code used for German.

Copy the appropriate language file into the GCS translations directory and relaunch GCS. For GCS v5+, the exact path can be found in the help on the command line: `gcs --help`. For versions of GCS prior to v5, this was typically a directory named `i18n` alongside the executable. GCS only reads the contents of these files once, at startup, so any changes made to them will not be noticed until you quit and re-launch.

GCS determines which language to use by looking at environment variables. It first looks at `LC_ALL`. If that isn't set or is empty, it then looks at `LANG`. If that isn't set or is empty, it then falls back to using `en_US.UTF-8` as the language choice. In addition, if the language specified isn't available (i.e. no translation file is present, or a missing key in the translation file), then the languages listed in the `LANGUAGE` environment variable (separated by `:`) are used as fallbacks, in the order listed.

### How do I create my own translations?

If you'd like to provide a translation for a language you are fluent in, copy the `language.i18n` file found on the release page on github for the version you're interested in and name it for your language (e.g. `de.i18n` for German), then edit its contents, updating the `v:` values to have the translation for the `k:` values. The file itself has more details about how to edit it. If you have questions, feel free to contact me about this.
