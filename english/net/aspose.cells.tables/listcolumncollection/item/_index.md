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
// Called: Assert.AreEqual(&amp;quot;2.6882&amp;quot;, workbook.Worksheets[0].ListObjects[5].ListColumns[8].Name);
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET55477_1.xlsx&quot;);
          
            workbook.Save(Constants.destPath + &quot;CELLSNET55477_1.xlsx&quot;);
            Assert.AreEqual(&quot;2.6882&quot;, workbook.Worksheets[0].ListObjects[5].ListColumns[8].Name);
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

### See Also

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


