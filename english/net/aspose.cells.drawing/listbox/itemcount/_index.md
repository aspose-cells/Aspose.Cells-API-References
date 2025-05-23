---
title: ListBox.ItemCount
second_title: Aspose.Cells for .NET API Reference
description: ListBox property. Gets the number of items in the list box
type: docs
url: /net/aspose.cells.drawing/listbox/itemcount/
---
## ListBox.ItemCount property

Gets the number of items in the list box.

```csharp
public int ItemCount { get; }
```

### Examples

```csharp
// Called: int count = listbox.ItemCount;
public void ListBox_Property_ItemCount()
{
    Workbook workbook = new Workbook();
    Worksheet worksheet = workbook.Worksheets.Add("First Sheet");

    worksheet.Cells[0, 0].PutValue("Jason");
    worksheet.Cells[1, 0].PutValue("Rick");
    worksheet.Cells[2, 0].PutValue("Jane");
    worksheet.Cells[3, 0].PutValue("Rachel");

    Aspose.Cells.Drawing.ListBox listbox = worksheet.Shapes.AddListBox(0, 0, 1, 0, 40, 100);
    listbox.InputRange = "A1:A4";
    listbox.SelectionType = Aspose.Cells.Drawing.SelectionType.Multi;
    int count = listbox.ItemCount;
    Assert.AreEqual(count, 4);
    listbox.PageChange = count;
    listbox.Height = count * 15;


    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


