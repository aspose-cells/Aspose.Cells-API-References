---
title: ListObjectCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ListObjectCollection property. Gets the ListObject by index
type: docs
url: /net/aspose.cells.tables/listobjectcollection/item/
---
## ListObjectCollection indexer (1 of 2)

Gets the ListObject by index.

```csharp
public ListObject this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

The ListObject

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].ListObjects[0].TableStyleType, TableStyleType.None);
public void ListObjectCollection_Property_Item()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual(workbook.Worksheets[0].ListObjects[0].TableStyleType, TableStyleType.None);
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual(workbook.Worksheets[0].ListObjects[0].TableStyleType, TableStyleType.None);
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ListObjectCollection indexer (2 of 2)

Gets the ListObject by specified name.

```csharp
public ListObject this[string tableName] { get; }
```

| Parameter | Description |
| --- | --- |
| tableName | ListObject name. |

### Return Value

The ListObject

### Examples

```csharp
// Called: ListObject listObject = ws.ListObjects[tname];
public void ListObjectCollection_Property_Item()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet ws = workbook.Worksheets["Pg2 Acct Code Breakdown"];

    ArrayList dNames = new ArrayList();
    for (int i = 0; i < ws.ListObjects.Count; i++)
    {
        string tname = ws.ListObjects[i].DisplayName;
        dNames.Add(tname);

    }

    if (dNames.Count != 0)
    {
        for (int i = 0; i < dNames.Count; i++)
        {
            string tname = dNames[i].ToString();
            ListObject listObject = ws.ListObjects[tname];
            listObject.ConvertToRange();//Exception
        }
    }

    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


