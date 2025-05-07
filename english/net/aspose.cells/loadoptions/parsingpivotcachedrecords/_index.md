---
title: LoadOptions.ParsingPivotCachedRecords
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Indicates whether parsing pivot cached records when loading the file. The default value is false
type: docs
url: /net/aspose.cells/loadoptions/parsingpivotcachedrecords/
---
## LoadOptions.ParsingPivotCachedRecords property

Indicates whether parsing pivot cached records when loading the file. The default value is false.

```csharp
public bool ParsingPivotCachedRecords { get; set; }
```

### Remarks

Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

### Examples

```csharp
// Called: loadOptions.ParsingPivotCachedRecords = true;
[Test]
        public void Property_ParsingPivotCachedRecords()
        {
            LoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
            loadOptions.ParsingPivotCachedRecords = true;
            Workbook workbook1 = new Workbook(Constants.PivotTableSourcePath + "CellsNet54902.csv", loadOptions);
            workbook1.Worksheets[0].Name = "Cas";
            CreatePivotTable(workbook1);
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


