---
title: PivotField.IsInsertPageBreaksBetweenItems
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether inserting page breaks after each item. The default value is false
type: docs
url: /net/aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems/
---
## PivotField.IsInsertPageBreaksBetweenItems property

Indicates whether inserting page breaks after each item. The default value is false.

```csharp
public bool IsInsertPageBreaksBetweenItems { get; set; }
```

### Examples

```csharp
// Called: field.IsInsertPageBreaksBetweenItems = true;
public void PivotField_Property_IsInsertPageBreaksBetweenItems()
{
    Workbook book = AddDateWorkbok();
    PivotTable pivot = AddDatePivotTable(book);

    Worksheet sheet = book.Worksheets[0];
    SheetRender render = new SheetRender(sheet, new ImageOrPrintOptions());
    Assert.AreEqual(1, render.PageCount);

    Cells cells = sheet.Cells;
    PivotField field = pivot.RowFields[0];
    field.IsInsertPageBreaksBetweenItems = true;
    pivot.RefreshData();
    pivot.CalculateData();

    SheetRender newRender = new SheetRender(sheet, new ImageOrPrintOptions());
    Assert.AreEqual(6, newRender.PageCount);

    book.Save(Constants.destPath + "TestIsInsertPageBreaksBetweenItems.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


