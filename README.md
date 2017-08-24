# NgBootstrapAoT

To reproduce webpack build errors:

```
cd NgBootstrapAoT
npm install
webpack --config webpack.config.vendor.js --env.prod
webpack --env.prod
```

Expected output:

```
$ webpack --env.prod
Hash: b72fad9933e3fdfcd9795b2ec44ae44a4f2c21e1
Version: webpack 2.5.1
Child
    Hash: b72fad9933e3fdfcd979
    Time: 15657ms
             Asset    Size  Chunks                    Chunk Names
    main-client.js  600 kB       0  [emitted]  [big]  main-client

    ERROR in ./$$_gendir/~/@ng-bootstrap/ng-bootstrap/alert/alert.ngfactory.ts
    Module parse failed: D:\Projects\NgBootstrapAoT\NgBootstrapAoT\$$_gendir\node_modules\@ng-bootstrap\ng-bootstrap\alert\alert.ngfactory.ts Unexpected token (13:21)
    You may need an appropriate loader to handle this file type.
    | import * as i2 from '@ng-bootstrap/ng-bootstrap/alert/alert';
    | import * as i3 from '@ng-bootstrap/ng-bootstrap/alert/alert-config';
    | const styles_NgbAlert:any[] = ([] as any[]);
    | export const RenderType_NgbAlert:i0.RendererType2 = i0.ɵcrt({encapsulation:2,styles:styles_NgbAlert,
    |     data:{}});
     @ ./$$_gendir/ClientApp/app/app.module.browser.ngfactory.ts 10:0-103
     @ ./ClientApp/boot.browser.ts

    ERROR in ./$$_gendir/~/@ng-bootstrap/ng-bootstrap/tooltip/tooltip.ngfactory.ts
    Module parse failed: D:\Projects\NgBootstrapAoT\NgBootstrapAoT\$$_gendir\node_modules\@ng-bootstrap\ng-bootstrap\tooltip\tooltip.ngfactory.ts Unexpected token (11:29)
    You may need an appropriate loader to handle this file type.
    | import * as i0 from '@angular/core';
    | import * as i1 from '@ng-bootstrap/ng-bootstrap/tooltip/tooltip';
    | const styles_NgbTooltipWindow:any[] = ['.bs-tooltip-top[_nghost-%COMP%]   .arrow[_ngcontent-%COMP%], .bs-tooltip-bottom[_nghost-%COMP%]   .arrow[_ngcontent-%COMP%] {\n      left: 50%;\n    }\n\n    .bs-tooltip-left[_nghost-%COMP%]   .arrow[_ngcontent-%COMP%], .bs-tooltip-right[_nghost-%COMP%]   .arrow[_ngcontent-%COMP%] {\n      top: 50%;\n    }'];
    | export const RenderType_NgbTooltipWindow:i0.RendererType2 = i0.ɵcrt({encapsulation:0,
    |     styles:styles_NgbTooltipWindow,data:{}});
     @ ./$$_gendir/ClientApp/app/app.module.browser.ngfactory.ts 11:0-107
     @ ./ClientApp/boot.browser.ts
 
 etc.
 ```
 
