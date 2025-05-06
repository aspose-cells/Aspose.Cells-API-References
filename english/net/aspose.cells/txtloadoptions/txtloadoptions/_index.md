---
title: TxtLoadOptions.TxtLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions constructor. Creates the options for loading text file
type: docs
url: /net/aspose.cells/txtloadoptions/txtloadoptions/
---
## TxtLoadOptions() {#constructor}

Creates the options for loading text file.

```csharp
public TxtLoadOptions()
```

### Remarks

The default load file type is CSV .

### Examples

```csharp
// Called: var workbook = new Workbook(datafileName, new TxtLoadOptions { Separator = &amp;apos;;&amp;apos; });
[Test]
        public void TxtLoadOptions_Constructor()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET46734_&quot;;
            string datafileName = filePath + &quot;Data.csv&quot;;

            var workbook = new Workbook(datafileName, new TxtLoadOptions { Separator = &apos;;&apos; });
            var worksheet = workbook.Worksheets[workbook.Worksheets.ActiveSheetIndex];
            var data = worksheet.Cells.ExportDataTable(0, 0, worksheet.Cells.MaxRow + 1, worksheet.Cells.MaxColumn + 1,
                new ExportTableOptions() { ExportColumnName = true });

            CreatePivotTable46734(data, filePath);
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtLoadOptions(LoadFormat) {#constructor_1}

Creates the options for loading text file.

```csharp
public TxtLoadOptions(LoadFormat loadFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loading format |

### See Also

* enum [LoadFormat](../../loadformat/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


