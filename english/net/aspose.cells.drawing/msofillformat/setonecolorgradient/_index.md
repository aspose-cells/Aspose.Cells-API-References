---
title: MsoFillFormat.SetOneColorGradient
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormat method. Sets the specified fill to a onecolor gradient
type: docs
url: /net/aspose.cells.drawing/msofillformat/setonecolorgradient/
---
## MsoFillFormat.SetOneColorGradient method

Sets the specified fill to a one-color gradient.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | One gradient color. |
| degree | Double | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### Examples

```csharp
// Called: fillFormat.SetOneColorGradient(Color.Green, 0.3, GradientStyleType.Horizontal, 1);
public static void Method_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an arc shape to the worksheet
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Access the fill format of the shape
            MsoFillFormat fillFormat = arcShape.FillFormat;

            // Set the fill fore color
            fillFormat.ForeColor = Color.Blue;

            // Set the fill back color
            fillFormat.BackColor = Color.LightBlue;

            // Set the transparency
            fillFormat.Transparency = 0.5;

            // Check if the fill is visible
            bool isVisible = fillFormat.IsVisible;
            Console.WriteLine(&quot;Is Fill Visible: &quot; + isVisible);

            // Set a one-color gradient fill
            fillFormat.SetOneColorGradient(Color.Green, 0.3, GradientStyleType.Horizontal, 1);

            // Save the workbook
            workbook.Save(&quot;MsoFillFormatExample.xlsx&quot;);
        }
```

### See Also

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


