# Third-Party Notices

SHK IPTV is proprietary software (see [LICENSE](LICENSE)) that includes the
following third-party components. This file lists them and their license
terms, as required by those licenses.

## FFmpeg

SHK IPTV runs an unmodified, official FFmpeg binary as a separate process
to remux video and convert incompatible audio tracks to AAC — it is not
modified and not compiled into this application's own code.

- Project: https://ffmpeg.org
- License: GNU General Public License v3 (GPLv3) — see
  https://www.gnu.org/licenses/gpl-3.0.html
- Source code for the exact version distributed with this release: see the
  `ffmpeg -version` output bundled in the release, and the corresponding
  commit at https://github.com/FFmpeg/FFmpeg

## Electron

The application shell is built with Electron, which bundles Chromium and
Node.js. Electron's own license and the full list of bundled open-source
components (Chromium, Node.js, and their dependencies) are included with
every download as `LICENSE.electron.txt` and `LICENSES.chromium.html`,
installed alongside the application.

- Project: https://www.electronjs.org
- License: MIT

## JavaScript libraries

| Library | License | Copyright |
|---|---|---|
| React / React DOM | MIT | Facebook, Inc. and its affiliates |
| hls.js | Apache-2.0 | Dailymotion; portions Brightcove |
| lucide-react | ISC | Cole Bemis / Lucide Contributors |
| axios | MIT | Matt Zabriskie & Collaborators |
| express | MIT | TJ Holowaychuk, Roman Shtylman, Douglas Christopher Wilson |
| http-proxy-middleware | MIT | Steven Chim |
| electron-updater | MIT | Loopline Systems |

Full license texts:

### MIT (React, React DOM, axios, express, http-proxy-middleware, electron-updater)

```
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

### ISC (lucide-react)

```
Permission to use, copy, modify, and/or distribute this software for any
purpose with or without fee is hereby granted, provided that the above
copyright notice and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
```

### Apache License 2.0 (hls.js)

Licensed under the Apache License, Version 2.0. A copy of the license is
available at http://www.apache.org/licenses/LICENSE-2.0.
