# Vendored Third-Party Notices

## SheetJS Community Edition

- File: `assets/vendor/xlsx.full.min.js`
- Version: 0.20.3
- Source used for vendoring: `https://cdn.sheetjs.com/xlsx-0.20.3/package/dist/xlsx.full.min.js`
- License: Apache License 2.0
- Full license text: `assets/vendor/SHEETJS-LICENSE.txt`

This dependency is vendored so the static app does not load XLSX parsing code from a CDN at runtime.

## ISO 3166 Country Code Data

- File: `assets/js/country-codes.js`
- Source: `wooorm/iso-3166`
- Source URL: `https://github.com/wooorm/iso-3166`
- Data used: assigned ISO 3166-1 alpha-2 code, alpha-3 code, and English name
- License: MIT

Runtime common display names are read from the browser `Intl.DisplayNames`
implementation when available. They are not bundled as source data. Additional
short aliases in `assets/js/country-codes.js` are hand-authored for common
customer workbook inputs.

MIT license notice for `wooorm/iso-3166`:

```text
(The MIT License)

Copyright (c) 2020 Titus Wormer <tituswormer@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## Font Awesome Free Icons

- File: inline SVG symbol subset in `index.html`
- Source: Font Awesome Free SVG icon set
- License: CC BY 4.0 for icons
- Project URL: `https://fontawesome.com/`

Only the SVG paths needed by the static UI are embedded, so the app does not load Font Awesome from a CDN at runtime.
