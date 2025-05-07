---
title: Cells.IsDefaultRowHidden
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Indicates whether the row is default hidden
type: docs
url: /net/aspose.cells/cells/isdefaultrowhidden/
---
## Cells.IsDefaultRowHidden property

Indicates whether the row is default hidden.

```csharp
public bool IsDefaultRowHidden { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(newSheet.Cells.IsDefaultRowHidden);
[Test]
        public void Property_IsDefaultRowHidden()
        {
            Workbook sourceWorkbook = new Workbook(Constants.sourcePath + "CELLSNET47213CopyExample.xlsx");
            var sourceSheet = sourceWorkbook.Worksheets[1];

            var workbook = new Workbook(Constants.sourcePath + "CELLSNET47213TargetSheet.xlsx");
            var newwSheetId = workbook.Worksheets.Add();
            var newSheet = workbook.Worksheets[newwSheetId];

            newSheet.Name = "insertedSheet";
            newSheet.Copy(sourceSheet);
            Console.WriteLine(newSheet.Cells.IsDefaultRowHidden);
            Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + "CellsNet47213.xlsx");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


