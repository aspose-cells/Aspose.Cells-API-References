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
public void WorksheetCollection_Property_TableStyles()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual(3,workbook.Worksheets.TableStyles.Count);
    workbook.RemoveUnusedStyles();
    Assert.AreEqual(2, workbook.Worksheets.TableStyles.Count);
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [TableStyleCollection](../../../aspose.cells.tables/tablestylecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


