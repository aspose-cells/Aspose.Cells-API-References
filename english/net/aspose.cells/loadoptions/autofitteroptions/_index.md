---
title: LoadOptions.AutoFitterOptions
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets and sets the auto fitter options
type: docs
url: /net/aspose.cells/loadoptions/autofitteroptions/
---
## LoadOptions.AutoFitterOptions property

Gets and sets the auto fitter options

```csharp
public AutoFitterOptions AutoFitterOptions { get; set; }
```

### Remarks

Only for xlsx ,spreadsheetML file now.

### Examples

```csharp
// Called: loadOptions.AutoFitterOptions = options;
public void LoadOptions_Property_AutoFitterOptions()
{
    AutoFitterOptions options = new AutoFitterOptions();
    options.OnlyAuto = true;
    LoadOptions loadOptions = new LoadOptions();
    loadOptions.AutoFitterOptions = options;
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx", loadOptions);
    Assert.AreEqual(76.5, workbook.Worksheets[0].Cells.GetRowHeight(12));
}
```

### See Also

* class [AutoFitterOptions](../../autofitteroptions/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


