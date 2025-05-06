---
title: Workbook.FileFormat
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets and sets the file format
type: docs
url: /net/aspose.cells/workbook/fileformat/
---
## Workbook.FileFormat property

Gets and sets the file format.

```csharp
public FileFormatType FileFormat { get; set; }
```

### Examples

```csharp
// Called: template.FileFormat = FileFormatType.Xlsx;
[Test]
        public void Property_FileFormat()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET46824_&quot;;


            LoadOptions opt = new LoadOptions();
            opt.MemorySetting = MemorySetting.MemoryPreference;

            Workbook template = new Workbook(filePath + &quot;Template.xlsx&quot;);
            Workbook dataSource = new Workbook(filePath + &quot;DataSource.xlsx&quot;);

            // Copy Data
            template = CopyDataToTemplate46824(dataSource.Worksheets[0], template);


            template.FileFormat = FileFormatType.Xlsx;
            template.Save(Constants.PIVOT_CHECK_FILE_PATH + &quot;NET46824.xlsx&quot;, SaveFormat.Xlsx);
        }
```

### See Also

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


