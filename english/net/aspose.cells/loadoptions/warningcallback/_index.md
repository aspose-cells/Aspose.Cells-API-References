---
title: LoadOptions.WarningCallback
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets or sets warning callback
type: docs
url: /net/aspose.cells/loadoptions/warningcallback/
---
## LoadOptions.WarningCallback property

Gets or sets warning callback.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Examples

```csharp
// Called: options.WarningCallback = new WarningCallback();
[Test]
        public void Property_WarningCallback()
        {
            LoadOptions options = new LoadOptions();
            options.WarningCallback = new WarningCallback();
            Workbook book = new Workbook(Constants.sourcePath + "CELLSJAVA42150.xlsx", options);

            book.Save(Constants.destPath + "CELLSJAVA42150.xlsx");
        }
```

### See Also

* interface [IWarningCallback](../../iwarningcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


