---
title: Enum MsoArrowheadStyle
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.MsoArrowheadStyle enum. Enumerates the line end type of the shape border line
type: docs
url: /net/aspose.cells.drawing/msoarrowheadstyle/
---
## MsoArrowheadStyle enumeration

Enumerates the line end type of the shape border line.

```csharp
public enum MsoArrowheadStyle
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No line end type. |
| Arrow | `1` | Arrow line end type. |
| ArrowStealth | `2` | Arrow Stealth line end type. |
| ArrowDiamond | `3` | Arrow Diamond Line end type. |
| ArrowOval | `4` | Arrow Oval line end type. |
| ArrowOpen | `5` | Arrow Open line end type. |

### Examples

```csharp
// Called: new Object[]{&amp;quot;BeginArrowheadStyle&amp;quot;,  MsoArrowheadStyle.ArrowStealth},
public void Type_MsoArrowheadStyle(Shape shape, LineShape lineshape) 
        {
            if (shape.UpperLeftRow == 21 &amp;&amp; shape.UpperLeftColumn == 3 &amp;&amp; shape.LowerRightRow == 26 &amp;&amp; shape.LowerRightColumn == 6)
            {    
                    ReflectInvoker.invoke(&quot;lineshape&quot;, lineshape, new Object[][]{
                    new Object[] {&quot;HeightCM&quot;, 2.57, 0.01},
                    new Object[] {&quot;WidthCM&quot;, 5.95, 0.01},
                    new Object[] {&quot;RotationAngle&quot;, 0.0},
                    new Object[] {&quot;HeightScale&quot;, 100},
                    new Object[] {&quot;WidthScale&quot;, 100},
                    new Object[] {&quot;IsLockAspectRatio&quot;, false},
                    new Object[] {&quot;IsLocked&quot;, true},
                    new Object[] {&quot;Placement&quot;, PlacementType.MoveAndSize},
                    new Object[] {&quot;IsPrintable&quot;, true}
                 });

                  MsoLineFormat msolineFormat = shape.LineFormat;
                  ReflectInvoker.invoke(&quot;msolineFormat&quot;, msolineFormat, new Object[][]{
                        new Object[] {&quot;ForeColor&quot;, Color.Black},
                        new Object[] {&quot;DashStyle&quot;, MsoLineDashStyle.DashDot},
                        new Object[] {&quot;Weight&quot;, 0.75},
                });     
                ReflectInvoker.invoke(&quot;lineshape.Line&quot;, lineshape.Line, new Object[][]{
				 new Object[]{&quot;BeginArrowheadStyle&quot;,  MsoArrowheadStyle.ArrowStealth},
				   new Object[]{&quot;EndArrowheadStyle&quot;, MsoArrowheadStyle.Arrow},
				   new Object[]{&quot;BeginArrowheadLength&quot;,  MsoArrowheadLength.Medium},
				   new Object[]{&quot;EndArrowheadLength&quot;, MsoArrowheadLength.Medium}
		       });
                   
            }
      
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


