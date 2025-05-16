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
// Called: Assert.AreEqual("T1", ListObject.ListColumns[0].Name);
public void ListColumnCollection_Property_Item()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Worksheet worksheet = workbook.Worksheets[0];

    ListObject ListObject = worksheet.ListObjects[0];
    Assert.AreEqual("T1",ListObject.ListColumns[0].Name);
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
     worksheet = workbook.Worksheets[0];

    ListObject = worksheet.ListObjects[0];
    Assert.AreEqual("T1", ListObject.ListColumns[0].Name);
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

### Examples

```csharp
namespace AsposeCellsExamples.ListColumnCollectionPropertyItemDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 2.5;
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = 1.8;

            int tableIndex = worksheet.ListObjects.Add("A1", "B3", true); // Split range into start/end cells
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowHeaderRow = true;

            ListColumnCollection listColumns = table.ListColumns;

            ListColumn column = listColumns["Product"];
            Console.WriteLine("Current column name: " + column.Name);

            column.Name = "Item";
            Console.WriteLine("Updated column name: " + column.Name);

            workbook.Save("ListColumnCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### See Also

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


