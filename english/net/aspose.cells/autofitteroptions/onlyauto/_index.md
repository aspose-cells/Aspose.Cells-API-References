---
title: AutoFitterOptions.OnlyAuto
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Indicates whether only fit the rows which height are not customed
type: docs
url: /net/aspose.cells/autofitteroptions/onlyauto/
---
## AutoFitterOptions.OnlyAuto property

Indicates whether only fit the rows which height are not customed.

```csharp
public bool OnlyAuto { get; set; }
```

### Examples

```csharp
// Called: loadOptions.AutoFitterOptions.OnlyAuto = true;
public void AutoFitterOptions_Property_OnlyAuto()
{
    LoadOptions loadOptions = new LoadOptions();
    loadOptions.AutoFitterOptions = new AutoFitterOptions();
    loadOptions.AutoFitterOptions.OnlyAuto = true;
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xml", loadOptions);
    Assert.AreEqual(workbook.Worksheets[1].Cells.GetColumnWidthPixel(13), 71);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(workbook.Worksheets[0].Cells["I4"].GetStyle().VerticalAlignment, TextAlignmentType.Center);
}
```

### See Also

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


