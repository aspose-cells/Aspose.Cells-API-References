---
title: Cell.GetWidthOfValue
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the width of the value in unit of pixels
type: docs
url: /net/aspose.cells/cell/getwidthofvalue/
---
## Cell.GetWidthOfValue method

Gets the width of the value in unit of pixels.

```csharp
public int GetWidthOfValue()
```

### Examples

```csharp
// Called: Assert.AreEqual(cell.GetWidthOfValue(), 89);
[Test]
         public void Method_GetWidthOfValue()
         {
             Workbook workbook = new Workbook();
             Cell cell = workbook.Worksheets[0].Cells[&quot;A1&quot;];
             cell.PutValue(&quot;CellsJava40307&quot;);
             Assert.AreEqual(cell.GetWidthOfValue(), 89);
         }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


