---
title: PivotField.OriginalItems
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Get the original base items
type: docs
url: /net/aspose.cells.pivot/pivotfield/originalitems/
---
## PivotField.OriginalItems property

Get the original base items;

```csharp
public string[] OriginalItems { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(field.OriginalItems[0], "2");
public void PivotField_Property_OriginalItems()
{
    Workbook wb = new Workbook(Constants.openPivottablePath + "AsposeGroupedField2.xlsx");
    PivotTable table = wb.Worksheets[0].PivotTables[0];
    PivotField field = table.RowFields[0];

    Assert.AreEqual(field.Items[0],"<2");
    Assert.AreEqual(field.OriginalItems[0], "2");
    //Console.WriteLine(field.IsIncludeNewItemsInFilter);
    //Console.WriteLine(field.IsRepeatItemLabels);
    //Console.WriteLine(field.ShowAllItems);
    //Console.WriteLine(field.IsInsertPageBreaksBetweenItems);

    //Console.WriteLine(table.Indent);
    //Console.WriteLine(table.IsMultipleFieldFilters);
    //Console.WriteLine(table.ShowDataTips);
    //Console.WriteLine(table.ShowMemberPropertyTips);
    //Console.WriteLine(table.ShowValuesRow);
    //Console.WriteLine(table.ShowEmptyRow);
    //Console.WriteLine(table.ShowEmptyCol);
    //Console.WriteLine(table.FieldListSortAscending);
    //Console.WriteLine(table.ShowDrill);
    //Console.WriteLine(table.MissingItemsLimit);
    //Console.WriteLine(table.EnableDataValueEditing);
    //Console.WriteLine(table.AltTextTitle);
    //Console.WriteLine(table.AltTextDescription);
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


