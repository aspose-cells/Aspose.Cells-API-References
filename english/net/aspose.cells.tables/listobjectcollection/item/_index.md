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
// Called: Assert.AreEqual(&amp;quot;Column4&amp;quot;, workbook.Worksheets[0].ListObjects[0].ListColumns[1].Name);
[Test]
        // How do I insert a new column into a table (list object)
        // http://www.aspose.com/community/forums/thread/296197.aspx
        public void Property_Int32_()
        {
            Console.WriteLine(&quot;Property_Int32_()&quot;);
            string infn = path + @&quot;20110411\CELLSNET-26049\Book1.xlsx&quot;;
            string outfn = Constants.destPath + @&quot;CELLSNET-26049.xlsx&quot;;

            Workbook workbook = new Workbook(infn);
            Cells cells = workbook.Worksheets[0].Cells;

            cells.InsertColumns(2, 2);
            Assert.AreEqual(&quot;Column4&quot;, workbook.Worksheets[0].ListObjects[0].ListColumns[1].Name);
            workbook.Save(outfn);
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
// Called: table = worksheets[&amp;quot;S.19.01.01.paid&amp;quot;].ListObjects[&amp;quot;ClaimsStored&amp;quot;];
[Test]
        public void Property_String_()
        {
            Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + &quot;CELLSJAVA42431.xlsx&quot;);
            WorksheetCollection worksheets = workbook.Worksheets;
            ListObject table;

            table = worksheets[&quot;S.19.01.01.paid&quot;].ListObjects[&quot;ClaimsStored&quot;];
            table.Resize(table.StartRow, table.StartColumn, table.EndRow + 17, table.EndColumn, table.ShowHeaderRow);
            table = worksheets[&quot;S.19.01.01.RBNS&quot;].ListObjects[&quot;ClaimsStored8&quot;];
            table.Resize(table.StartRow, table.StartColumn, table.EndRow + 17, table.EndColumn, table.ShowHeaderRow);
            Assert.AreEqual(worksheets[&quot;S.19.01.01.paid&quot;].Cells[&quot;J37&quot;].Formula, &quot;=[@C0170]&quot;);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA42431.xlsx&quot;);
        }
```

### See Also

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


