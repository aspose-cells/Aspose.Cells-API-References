---
title: WorksheetCollection.TableStyles
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Gets TableStyles object
type: docs
url: /net/aspose.cells/worksheetcollection/tablestyles/
---
## WorksheetCollection.TableStyles property

Gets `TableStyles` object.

```csharp
public TableStyleCollection TableStyles { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(3,workbook.Worksheets.TableStyles.Count);
[Test]
        public void Property_TableStyles()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET45613.xls");
            Assert.AreEqual(3,workbook.Worksheets.TableStyles.Count);
            workbook.RemoveUnusedStyles();
            Assert.AreEqual(2, workbook.Worksheets.TableStyles.Count);
            workbook.Save(Constants.destPath + "CellsNet45613.xls");
        }
```

### See Also

* class [TableStyleCollection](../../../aspose.cells.tables/tablestylecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


