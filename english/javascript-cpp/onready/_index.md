---
title: onReady
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Provides an initialization function to load licenses, fonts, and other configurations.
type: docs
url: /javascript-cpp/onready/
---

## onReady function
Initializes Aspose.Cells WebAssembly module with the given options and returns a Promise that resolves when the module is ready.

```javascript
onReady(options?: Object): Promise<void>;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | Object | Configuration options for initializing the module. Contains licenses, fonts, etc. |

**Example**

The following example demonstrates how to configure license, font list and use Aspose.Cells in a browser.
```javascript
<script src="aspose.cells.js.min.js"></script>
<script>
    const { Workbook } = AsposeCells;
    AsposeCells.onReady({
        license: "/lic/aspose.cells.enc",
        fontPath: "/fonts/",
        fontList: [
            "arial.ttf",
            "NotoSansSC-Regular.ttf"
        ]
    }).then(() => {
        var workbook = new Workbook();
    });
</script>
```

**Example**

Aspose.Cells can also be used directly in a browser.
```javascript
<script src="aspose.cells.js.min.js"></script>
<script>
    const { Workbook } = AsposeCells;
    var workbook = new Workbook();
</script>
```

**Example**

The following example demonstrates how to use Aspose.Cells in Node.js.
```javascript
const { AsposeCells } = require("aspose.cells.js");
const { Workbook } = AsposeCells;

AsposeCells.onReady({
        license: "./files/aspose.cells.enc"
    }).then(() => {
    var workbook = new Workbook();
});
```

**Example**

How to use Aspose.Cells in Node.js without any options.
```javascript
const { AsposeCells } = require("aspose.cells.js");
const { Workbook } = AsposeCells;

AsposeCells.onReady().then(() => {
    var workbook = new Workbook();
});
```
