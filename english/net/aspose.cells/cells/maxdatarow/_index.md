---
title: Cells.MaxDataRow
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Maximum row index of cell which contains data
type: docs
url: /net/aspose.cells/cells/maxdatarow/
---
## Cells.MaxDataRow property

Maximum row index of cell which contains data.

```csharp
public int MaxDataRow { get; }
```

### Remarks

Return -1 if there is no cell which contains data.

### Examples

```csharp
// Called: table.Resize(table.StartRow, table.StartColumn, sheet.Cells.MaxDataRow, sheet.Cells.MaxDataColumn, true);
[Test]
        public void Property_MaxDataRow()
        {
            Workbook wbSource = new Workbook(Constants.sourcePath + "CELLSNET46375.xlsm");
            Worksheet sheet = wbSource.Worksheets[0];

            ListObject table = sheet.ListObjects[0];

            table.Resize(table.StartRow, table.StartColumn, sheet.Cells.MaxDataRow, sheet.Cells.MaxDataColumn, true);
            Style style = sheet.Cells["B26"].GetStyle();
           AssertHelper.AreEqual(style.Font.Color, Color.White);
            wbSource.Save(Constants.destPath + "CELLSNET46375.xlsx");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


