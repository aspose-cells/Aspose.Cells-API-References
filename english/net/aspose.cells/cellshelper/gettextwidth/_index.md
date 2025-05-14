---
title: CellsHelper.GetTextWidth
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Get width of text in unit of points
type: docs
url: /net/aspose.cells/cellshelper/gettextwidth/
---
## CellsHelper.GetTextWidth method

Get width of text in unit of points.

```csharp
public static double GetTextWidth(string text, Font font, double scaling)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text. |
| font | Font | The font of the text. |
| scaling | Double | The scaling of text. |

### Examples

```csharp
// Called: Assert.AreEqual(9.75,CellsHelper.GetTextWidth("   ", workbook.DefaultStyle.Font, 1));
public void CellsHelper_Method_GetTextWidth()
{
    Workbook workbook = new Workbook();
    Assert.AreEqual(9.75,CellsHelper.GetTextWidth("   ", workbook.DefaultStyle.Font, 1));
}
```

### See Also

* class [Font](../../font/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


