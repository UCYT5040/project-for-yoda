# Project For Yoda

How I think a `manifest.yml` file for a Discord bot "plugin" should work.

## Large File

```yml
name: My Plugin
version: 4.2.0
website: https://github.com/UCYT5040/project-for-yoda # Only for the plugin's site, should not be used for a maintainer's site. Optional.
description: A short description.
readme: A url to a MD file or the content of a MD file. # Optional
maintainers:
    - name: UCYT5040
      website: https://github.com/UCYT5040 # Only for the maintainer's site, should not be used for the plugin's site. Optional.
      # Instead of website, you may use websites and a list.
      # websites:
      # - https://github.com/UCYT5040
      # - https://google.com/search?q=UCYT5040
    - name: Yoda # Maintainers don't need a website, so in this example Yoda does not have one.
permissions: # optional if only default perms are needed
    - read # read a file
    - write # write to a file
    - file # read and write bundled together
    - Mos # os module (import os)
    - Mre # re module (import re)
dependencies: # optional if there are no dependencies
    - Your Plugin # name of a plugin
    # you can be more specific like this:
    - name: Your Plugin
      version: 6.9
      website: https://github.com/imposter/your_plugin
help: # if not specified, use default (whatever that might be)
    command: command_function_name # (ctx is provided)
    # For classes:
    # command: ClassName.command_function_name
```

## Minimal File

```yml
name: My Plugin
version: 4.2.0
description: A short description.
maintainers:
    - name: UCYT5040
```
