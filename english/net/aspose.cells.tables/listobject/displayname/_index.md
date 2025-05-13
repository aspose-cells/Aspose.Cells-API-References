---
title: ListObject.DisplayName
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets the display name
type: docs
url: /net/aspose.cells.tables/listobject/displayname/
---
## ListObject.DisplayName property

Gets and sets the display name.

```csharp
public string DisplayName { get; set; }
```

### Examples

```csharp
// Called: listObject.DisplayName = "Table";
public void ListObject_Property_DisplayName()
{
    Workbook book = new Workbook();
    Worksheet sheet = book.Worksheets[0];

    sheet.Cells[0, 0].PutValue("Column A");
    sheet.Cells[0, 1].PutValue("Column B");

    ListObject listObject =
      sheet.ListObjects[sheet.ListObjects.Add(0, 0, 1, sheet.Cells.MaxColumn, true)];
    listObject.TableStyleType = TableStyleType.TableStyleMedium2;
    listObject.DisplayName = "Table";
    string fml = "=[Column A] + 1";
    listObject.ListColumns[1].Formula = fml;
    Assert.AreEqual(book.Settings.FormulaSettings.PreservePaddingSpaces
        ? "=[Column A] + 1" : "=[Column A]+1", sheet.Cells["B2"].Formula);
    book = Util.ReSave(book, SaveFormat.Xlsx);
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


