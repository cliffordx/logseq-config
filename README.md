## Description
NOTE: This is a fork repo from @cldwalker
You can find my global config under `config` folder.

This project contains my [Logseq](https://logseq.com/) configuration including
plugins. I use this configuration across all my graphs with the [global
configuration feature](https://docs.logseq.com/#/page/Global%20configuration).

## Setup

To try my configuration:
```
# If you have an existing logseq config directory, back it up
$ mv ~/.logseq/config ~/.logseq/config.bak

# Clone this configuration
$ git clone https://github.com/cldwalker/logseq-config .

# Copy over my config
$ cp -R config ~.logseq/config
```

Alternatively, you can copy over files for more granular usage.

## Plugins

To see the plugins I use, see [config/plugins.edn](config/plugins.edn).

TODO: Explain how to use my plugins once https://github.com/logseq/logseq/pull/6911 lands.

## Convert your local graph config to a global one

If you would like to convert your existing Logseq config to a global config and
possibly share with others via git:

1. In a shell: `cd ~/.logseq && git init`.
2. Copy this repository's .gitignore into `~/.logseq`.
3. Copy the `logseq/config.edn` from your most active graph to
   `~/.logseq/config/config.edn`. Be sure to only keep config options you want
   applied across all graphs. Remove the global config options from your local
   config files.
4. Save your config: `git add . && git commit -m "Initial commit"`


## Dev

Be sure to have [babashka](https://github.com/babashka/babashka) installed.

Run `bb tasks` to see available tasks. Currently there are tasks for listing plugins
and writing a `plugins.edn`.

## License
See LICENSE.md

## Additional Links
* https://cs.github.com/?scopeName=All+repos&scope=&q=logseq+path%3Alogseq%2Fconfig.edn - Github search for additional logseq configurations
