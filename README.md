# import-size Vscode Extension

This extension will display inline in the editor the size of the imported package.
The extension utilizes webpack with UglifyJSPlugin in order to detect the imported size.
![Example Image](https://file-gwpnofjfte.now.sh/Screen%20Shot%202017-07-15%20at%202.13.55%20PM.png)

## Features

- Default importing: `import Func from 'utils';`
- Entire content importing: `import * as Utils from 'utils';`
- Selective importing: `import {Func} from 'utils';`
- Selective importing with alias: `import {orig as alias} from 'utils';`
- Submodule importing: `import Func from 'utils/Func';`
- Require: `const Func = require('utils').Func;`
- Supports both `Javascript` and `Typescript`

## Known Issues

Naive detection of local imports by searching for imports that start with the char `.`

### 1.0.0

Initial release