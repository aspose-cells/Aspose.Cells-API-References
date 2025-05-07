---
title: ListColumnCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ListColumnCollection property. Gets the ListColumn by the index
type: docs
url: /net/aspose.cells.tables/listcolumncollection/item/
---
## ListColumnCollection indexer (1 of 2)

Gets the ListColumn by the index.

```csharp
public ListColumn this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

the ListColumn object.

### Examples

```csharp
// Called: var listColumn = selectedTable.ListColumns[2];
[Test]
        public void Property_Int32_()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET47547_";
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
                slicer.Title = "tabtab";
                slicer.AlternativeText = "descdescdescdesc";

                workbook.Save(savePath + @"out.xlsx");
            }
        }
```

### See Also

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ListColumnCollection indexer (2 of 2)

Gets the ListColumn by the name.

```csharp
public ListColumn this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The name of the ListColumn |

### Return Value

The ListColumn object.

### See Also

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


