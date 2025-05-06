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
// Called: options.WarningCallback = new NumbersWarningCallback();
[Test]
        public void Property_WarningCallback()
        {
            LoadOptions options = new LoadOptions();
            options.WarningCallback = new NumbersWarningCallback();
            Workbook wb = new Workbook(Constants.sourcePath + &quot;Numbers13/Acquisti.numbers&quot;, options);
            //wb.Save(Constants.destPath + @&quot;Numbers13\Acquisti.xlsx&quot;);
            wb = Util.ReSave(wb, SaveFormat.Xlsx);
        }
```

### See Also

* interface [IWarningCallback](../../iwarningcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


