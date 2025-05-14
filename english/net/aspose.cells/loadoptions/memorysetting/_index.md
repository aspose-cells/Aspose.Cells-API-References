---
title: LoadOptions.MemorySetting
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets or sets the memory usage options
type: docs
url: /net/aspose.cells/loadoptions/memorysetting/
---
## LoadOptions.MemorySetting property

Gets or sets the memory usage options.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Examples

```csharp
// Called: opt.MemorySetting = MemorySetting.MemoryPreference;
public void LoadOptions_Property_MemorySetting()
{
    string filePath = Constants.PivotTableSourcePath + @"NET46824_";


    LoadOptions opt = new LoadOptions();
    opt.MemorySetting = MemorySetting.MemoryPreference;

    Workbook template = new Workbook(filePath + "Template.xlsx");
    Workbook dataSource = new Workbook(filePath + "DataSource.xlsx");

    // Copy Data
    template = CopyDataToTemplate46824(dataSource.Worksheets[0], template);


    template.FileFormat = FileFormatType.Xlsx;
    template.Save(Constants.PIVOT_CHECK_FILE_PATH + "example.xlsx", SaveFormat.Xlsx);
}
```

### See Also

* enum [MemorySetting](../../memorysetting/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


