---
title: FillFormat.FillType
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Gets and sets fill type
type: docs
url: /net/aspose.cells.drawing/fillformat/filltype/
---
## FillFormat.FillType property

Gets and sets fill type

```csharp
public FillType FillType { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(FillType.Texture, chartarea.Area.FillFormat.FillType, &amp;quot;chartarea.Area.FillFormat.FillType&amp;quot;);
private void Property_FillType(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[&quot;Sheet3&quot;];
            Chart chart = sheet.Charts[0];
            ChartArea chartarea = chart.ChartArea;
            AssertHelper.AreEqual(FillType.Texture, chartarea.Area.FillFormat.FillType, &quot;chartarea.Area.FillFormat.FillType&quot;);
        }
```

### See Also

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


