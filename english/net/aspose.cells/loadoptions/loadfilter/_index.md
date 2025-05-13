---
title: LoadOptions.LoadFilter
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. The filter to denote how to load data
type: docs
url: /net/aspose.cells/loadoptions/loadfilter/
---
## LoadOptions.LoadFilter property

The filter to denote how to load data.

```csharp
public LoadFilter LoadFilter { get; set; }
```

### Examples

```csharp
// Called: options.LoadFilter = new LoadFilter40889();
public void LoadOptions_Property_LoadFilter()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets.Add();
    workbook.Worksheets[0].IsVisible = false;
    workbook.Worksheets[0].Cells["A1"].PutValue("sdfsdf");
    workbook.Save(Constants.destPath + "example.xlsx");
    LoadOptions options = new LoadOptions();
    options.LoadFilter = new LoadFilter40889();
    workbook.Dispose();
    workbook = new Workbook(Constants.destPath + "example.xlsx", options);
    Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].StringValue, "");
    workbook.Dispose();
}
```

### See Also

* class [LoadFilter](../../loadfilter/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


