# blockbuild-modules
## How To Install Modules
Use `blockb install <module> [version]` to install modules. Use `blockb` for more information on this command.
## Contributing
Add a directory to `/modules` and it can be installed with `blockb install <foldername>`. The directory must contain a `manifest.json` that looks something like this:
```json
{
    "author": "Your Name",
    "latest": "1.0.0"
}
```
As well as a `.zip` file for each version of the module. The archives must contain atleast one filter or an API extension (or both), and a `blockbuild-module-manifest.json` file. The archives should not contain any other files. The module can also include a `README.md` and `LICENSE`.