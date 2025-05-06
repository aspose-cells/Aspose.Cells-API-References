---
title: WorksheetCollection.GetRangeByName
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Gets Range object by predefined name
type: docs
url: /net/aspose.cells/worksheetcollection/getrangebyname/
---
## GetRangeByName(string) {#getrangebyname}

Gets Range object by pre-defined name.

```csharp
public Range GetRangeByName(string rangeName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | String | Name of range. |

### Return Value

Range object.

Returns null if the named range does not exist.

### Examples

```csharp
// Called: Aspose.Cells.Range range = book.Worksheets.GetRangeByName(&amp;quot;test&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook book = new Workbook(Constants.sourcePath + @&quot;CELLSNET48624.xlsx&quot;);
            book.Save(Constants.destPath + @&quot;CELLSNET48624.ods&quot;);
            book = new Workbook(Constants.destPath + @&quot;CELLSNET48624.ods&quot;);
            Aspose.Cells.Range range = book.Worksheets.GetRangeByName(&quot;test&quot;);
            Assert.AreEqual(range.RowCount, 0x100000);
            Assert.AreEqual(range.FirstRow, 0);
            Assert.AreEqual(&quot;=Sheet1!$C:$C&quot;, range.RefersTo);
        }
```

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRangeByName(string, int, bool) {#getrangebyname_1}

Gets [`Range`](../../range/) by pre-defined name or table's name

```csharp
public Range GetRangeByName(string rangeName, int currentSheetIndex, bool includeTable)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | String | Name of range or table's name. |
| currentSheetIndex | Int32 | The sheet index. -1 represents global . |
| includeTable | Boolean | Indicates whether checking all tables. |

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


