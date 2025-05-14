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
// Called: new Object[]{"EndArrowheadStyle", MsoArrowheadStyle.Arrow},
public void Drawing_Type_MsoArrowheadStyle(Shape shape, LineShape lineshape) 
        {
            if (shape.UpperLeftRow == 21 && shape.UpperLeftColumn == 3 && shape.LowerRightRow == 26 && shape.LowerRightColumn == 6)
            {    
                    ReflectInvoker.invoke("lineshape", lineshape, new Object[][]{
                    new Object[] {"HeightCM", 2.57, 0.01},
                    new Object[] {"WidthCM", 5.95, 0.01},
                    new Object[] {"RotationAngle", 0.0},
                    new Object[] {"HeightScale", 100},
                    new Object[] {"WidthScale", 100},
                    new Object[] {"IsLockAspectRatio", false},
                    new Object[] {"IsLocked", true},
                    new Object[] {"Placement", PlacementType.MoveAndSize},
                    new Object[] {"IsPrintable", true}
                 });

                  MsoLineFormat msolineFormat = shape.LineFormat;
                  ReflectInvoker.invoke("msolineFormat", msolineFormat, new Object[][]{
                        new Object[] {"ForeColor", Color.Black},
                        new Object[] {"DashStyle", MsoLineDashStyle.DashDot},
                        new Object[] {"Weight", 0.75},
                });     
                ReflectInvoker.invoke("lineshape.Line", lineshape.Line, new Object[][]{
				 new Object[]{"BeginArrowheadStyle",  MsoArrowheadStyle.ArrowStealth},
				   new Object[]{"EndArrowheadStyle", MsoArrowheadStyle.Arrow},
				   new Object[]{"BeginArrowheadLength",  MsoArrowheadLength.Medium},
				   new Object[]{"EndArrowheadLength", MsoArrowheadLength.Medium}
		       });
                   
            }
      
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


