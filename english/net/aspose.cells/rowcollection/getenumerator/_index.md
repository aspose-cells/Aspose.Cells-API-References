---
title: RowCollection.GetEnumerator
second_title: Aspose.Cells for .NET API Reference
description: RowCollection method. Gets an enumerator that iterates rows through this collection
type: docs
url: /net/aspose.cells/rowcollection/getenumerator/
---
## GetEnumerator() {#getenumerator}

Gets an enumerator that iterates rows through this collection

```csharp
public IEnumerator GetEnumerator()
```

### Return Value

enumerator

### Examples

```csharp
[C#]
Workbook workbook = new Workbook("template.xlsx");
Cells cells = workbook.Worksheets[0].Cells;

IEnumerator en = cells.Rows.GetEnumerator();
while (en.MoveNext())
{
    Row row = (Row)en.Current;
    Console.WriteLine(row.Index + ": " + row.Height);
}
```

### See Also

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Gets an enumerator that iterates rows through this collection

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Parameter | Type | Description |
| --- | --- | --- |
| reversed | Boolean | whether enumerate rows in reversed order |
| sync | Boolean | whether the returned enumerator should check the modification of row collection and keep synchronized with it. |

### Return Value

The row enumerator

### Remarks

If the row collection will be modified(by operations that may cause new Row be instantiated or existing Row be removed) during the traversal with the enumerator, synchronized enumerator should be used instead of normal enumerator so that the traversal can continue from the position just after the one has been traversed by the last MoveNext(). However, together with the advantage that no element be skipped or traversed repeatedly, the disadvantage for synchronized enumerator is that the performance will be degraded a bit when comparing with normal enumerator.

### See Also

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


