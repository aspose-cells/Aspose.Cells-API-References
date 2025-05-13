---
title: WorksheetCollection.Names
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Gets the collection of all the Name objects in the spreadsheet
type: docs
url: /net/aspose.cells/worksheetcollection/names/
---
## WorksheetCollection.Names property

Gets the collection of all the Name objects in the spreadsheet.

```csharp
public NameCollection Names { get; }
```

### Examples

```csharp
// Called: NameCollection nc = wb.Worksheets.Names;
public void WorksheetCollection_Property_Names()
{
    Assert.IsFalse(CellsHelper.NeedQuoteInFormula("My.Test"));
    Workbook wb = new Workbook();
    wb.Worksheets.Add("My.Test");
    NameCollection nc = wb.Worksheets.Names;
    Name n = nc[nc.Add("My.Test!TestName")];
    Assert.AreEqual("My.Test!TestName", n.FullText, "FullText");
}
```

### See Also

* class [NameCollection](../../namecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


