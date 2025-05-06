---
title: Worksheet.Slicers
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Get the Slicer collection in the worksheet
type: docs
url: /net/aspose.cells/worksheet/slicers/
---
## Worksheet.Slicers property

Get the Slicer collection in the worksheet

```csharp
public SlicerCollection Slicers { get; }
```

### Examples

```csharp
// Called: Slicer slicer = sheet.Slicers[index];
[Test]
        public void Property_Slicers()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET47547_&quot;;
            string savePath = CreateFolder(filePath);
            using (var workbook = new Workbook())
            {
                var sheet = PrepareSheet47547(workbook);
                // Create Table
                var selectedTable = sheet.ListObjects[sheet.ListObjects.Add(0, 0, sheet.Cells.MaxDataRow, sheet.Cells.MaxDataColumn, true)];
                var listColumn = selectedTable.ListColumns[2];
                int index = sheet.Slicers.Add(selectedTable, listColumn, 5, 7);

                Slicer slicer = sheet.Slicers[index];
                slicer.TopPixel = 8;
                slicer.LeftPixel = 8;
                slicer.Placement = PlacementType.FreeFloating;
                slicer.IsPrintable = true;
                slicer.IsLocked = true;
                slicer.Title = &quot;tabtab&quot;;
                slicer.AlternativeText = &quot;descdescdescdesc&quot;;

                workbook.Save(savePath + @&quot;out.xlsx&quot;);
            }
        }
```

### See Also

* class [SlicerCollection](../../../aspose.cells.slicers/slicercollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


