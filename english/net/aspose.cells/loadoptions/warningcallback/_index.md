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
// Called: options.WarningCallback = warningCallback;
public void LoadOptions_Property_WarningCallback()
{
    DefaultWarningCallback warningCallback = new DefaultWarningCallback();
    LoadOptions options = new LoadOptions();
    options.IgnoreUselessShapes = true;
    options.WarningCallback = warningCallback;
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx", options);
    wb.Save(Constants.destPath + "example.xlsx");
    Assert.AreEqual("APRIL2", wb.Worksheets["REGULAR"].Cells["D1"].StringValue);

}
```

### See Also

* interface [IWarningCallback](../../iwarningcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


