# blockbuild-modules
## How To Install Modules
Use `blockb install <module> [version]` to install modules. Use `blockb` for more information on this command.
## Contributing
Add a directory to /modules and it can be installed with `blockb install <foldername>`. The directory must contain a `manifest.json` that looks something like this:
```json
{
    "author": "Your Name",
    "latest": "1.0.0"
}
```
As well as a subdirectory for each version of the module. The subdirectories must contain atleast one filter or an API extension (or both), and a `blockbuild-module-manifest.json` file. They should not contain any other files, other than a `README.md` or `LICENSE`. We highly recommend adding a `README.md` and some way to find a `LICENSE` file (maybe a `LICENSE` file in the module, or a link to one in the `README.md`), however, they are optional.