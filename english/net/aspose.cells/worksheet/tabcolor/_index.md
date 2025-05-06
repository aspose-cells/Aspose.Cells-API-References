---
title: Worksheet.TabColor
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents worksheet tab color
type: docs
url: /net/aspose.cells/worksheet/tabcolor/
---
## Worksheet.TabColor property

Represents worksheet tab color.

```csharp
public Color TabColor { get; set; }
```

### Remarks

This feature is only supported in ExcelXP(Excel2002) and later versions. If you save file as Excel97 or Excel2000 format, it will be omitted.

### Examples

```csharp
// Called: AssertHelper.equals(color[i], worksheet.TabColor, worksheet.Name + &amp;quot;.TabColor&amp;quot;);
[Test]
        public void Property_TabColor()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Worksheet\\TabColor.xls&quot;);
            int n = workbook.Worksheets.Count;
            string sheet;
            Color[] color = new Color[] { Color.Red, Color.Black, Color.White, Color.Blue, Color.Empty };
            Worksheet worksheet;
            for (int i = 0; i &lt; n; i++)
            {
                sheet = &quot;sheet&quot; + (i + 1).ToString();
                worksheet = workbook.Worksheets[sheet];
                AssertHelper.equals(color[i], worksheet.TabColor, worksheet.Name + &quot;.TabColor&quot;);
            }           

        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


