---
title: WorksheetCollection.CreateRange
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Creates a Range object from an address of the range
type: docs
url: /net/aspose.cells/worksheetcollection/createrange/
---
## WorksheetCollection.CreateRange method

Creates a [`Range`](../../range/) object from an address of the range.

```csharp
public Range CreateRange(string address, int sheetIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | The address of the range. |
| sheetIndex | Int32 | The sheet index. |

### Return Value

A [`Range`](../../range/) object

### Examples

```csharp
// Called: range = workbook.Worksheets.CreateRange(&amp;quot;Sheet1!A1:A10&amp;quot;, 0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Aspose.Cells.Range range = workbook.Worksheets.CreateRange(&quot;A1:A10&quot;, 0);
            Assert.IsTrue(range != null);
            range = workbook.Worksheets.CreateRange(&quot;Sheet1!A1:A10&quot;, 0);
            Assert.IsTrue(range != null);
        }
```

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


