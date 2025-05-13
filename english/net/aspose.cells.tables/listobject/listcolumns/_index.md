---
title: ListObject.ListColumns
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets ListColumns of the ListObject
type: docs
url: /net/aspose.cells.tables/listobject/listcolumns/
---
## ListObject.ListColumns property

Gets ListColumns of the ListObject.

```csharp
public ListColumnCollection ListColumns { get; }
```

### Examples

```csharp
// Called: listObjects[0].ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;
public void ListObject_Property_ListColumns()
{
    Console.WriteLine("ListObject_Property_ListColumns()");
    string infn = path + "Test_CreateTable.xlsx";
    string outfn = Constants.destPath + "Test_CreateTable_out.xlsx";

    Workbook workbook = new Workbook(infn);

    ListObjectCollection listObjects = workbook.Worksheets[0].ListObjects;
    listObjects.Add(1, 1, 11, 5, true);
    listObjects[0].ShowTotals = true;
    listObjects[0].ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;

    listObjects[0].TableStyleType = TableStyleType.TableStyleLight4;

    workbook.Save(outfn);
}
```

### See Also

* class [ListColumnCollection](../../listcolumncollection/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


