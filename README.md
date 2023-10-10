# dts-cleanup
Removes .d.ts and .js files in the project

Recursively traverses folder structure and deletes generated `.d.ts` and `.js` file pairs.
Only deletes files if both files exist with the same name, e.g.
will delete both `index.d.ts` and `index.js`, but won't delete lonely `config.js`.

Never traverses `node_modules`. To exclude some files or folders, use
`--exclude` option.

### Usage
```
dts-cleanup [options]

Removes .d.ts and .js files in the project

Options:
  -e, --exclude  Path patterns to omit in addition to `node_modules`     [array]
  -h, --help     Show usage                                            [boolean]
  -v, --version  Show version number                                   [boolean]
```
