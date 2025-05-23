---
title: LoadOptions.AutoFilter
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Indicates whether auto filtering the data when loading the files
type: docs
url: /net/aspose.cells/loadoptions/autofilter/
---
## LoadOptions.AutoFilter property

Indicates whether auto filtering the data when loading the files.

```csharp
public bool AutoFilter { get; set; }
```

### Remarks

Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

### Examples

```csharp
// Called: options.AutoFilter = true;
public void LoadOptions_Property_AutoFilter()
{
    LoadOptions options = new LoadOptions();
    options.AutoFilter = true;
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xml", options);
    Assert.IsTrue(workbook.Worksheets[0].Cells.IsRowHidden(6));
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);//.Save(Constants.destPath + @"example.xlsx");
}
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


