---
title: MsoFillFormat.Transparency
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormat property. Returns or sets the degree of transparency of the specified fill as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells.drawing/msofillformat/transparency/
---
## MsoFillFormat.Transparency property

Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(0.2, comment.CommentShape.FillFormat.Transparency, "comment.CommentShape.LineFormat.Transparency");
public void Property_Transparency(Comment comment,int index)
        {
            if (comment.CommentShape.UpperLeftRow == 2 && comment.CommentShape.LowerRightRow == 6 &&
                comment.CommentShape.UpperLeftColumn == 3 && comment.CommentShape.LowerRightColumn == 4)
            {
                ReflectInvoker.invoke("comment", comment, new Object[][]{
                new Object[] {"Note", "YuYu:\naspose"},
                new Object[] {"IsVisible", true},
                    //==========Alignment========//
                    new Object[] {"AutoSize", false}                   
              });    
                ReflectInvoker.invoke("comment.CommentShape", comment.CommentShape, new Object[][]{
                     //==========Size============//
                    new Object[] {"HeightCM", 1.96, 0.01},
                    new Object[] {"WidthCM", 3.39, 0.01},
                    new Object[] {"HeightScale", 100},
                    new Object[] {"WidthScale", 100},
                    new Object[] {"IsLockAspectRatio", false},
                    //==========Protection==========//
                    new Object[] {"IsLocked", true},
                    //==========Properties==========//
                    new Object[] {"Placement", PlacementType.FreeFloating}
                });
                if(index != 0)
                {
                    ReflectInvoker.invoke("comment.CommentShape.LineFormat", comment.CommentShape.LineFormat, new Object[][]{
                     //==========Lines============//
                         new Object[] {"DashStyle", MsoLineDashStyle.Dash},
                         new Object[] {"Style", MsoLineStyle.ThickBetweenThin},
                         new Object[] {"Weight", 1.0}
                      });
                }
                
                AssertHelper.AreEqual(0.2, comment.CommentShape.FillFormat.Transparency, "comment.CommentShape.LineFormat.Transparency");
                AssertHelper.equals(Color.Red, comment.CommentShape.FillFormat.ForeColor, "comment.CommentShape.FillFormat.ForeColor");     
                AssertHelper.equals(Color.Black, comment.CommentShape.LineFormat.ForeColor, "comment.CommentShape.LineFormat.ForeColor");

                ReflectInvoker.invoke("comment.Font", comment.Font, new Object[][]{
                    new Object[] {"Name", "Tahoma"},
                    new Object[] {"Size", 8},
                    new Object[] {"Underline", FontUnderlineType.None},
                    new Object[] {"IsStrikeout", false},
                    new Object[] {"IsSubscript", false},
                    new Object[] {"IsSuperscript", false}
                   });
            }
            else if (comment.CommentShape.UpperLeftRow == 7 && comment.CommentShape.LowerRightRow == 9 &&
                comment.CommentShape.UpperLeftColumn == 5 && comment.CommentShape.LowerRightColumn == 6)
            {
                ReflectInvoker.invoke("comment", comment, new Object[][]{
                new Object[] {"Note", "YuYu:\n"},
                new Object[] {"IsVisible", true},
                    //==========Alignment========//
                    new Object[] {"AutoSize", false}                   
              });
                ReflectInvoker.invoke("comment.CommentShape", comment.CommentShape, new Object[][]{
                     //==========Size============//
                    new Object[] {"HeightCM", 0.98, 0.01},
                    new Object[] {"WidthCM", 1.69, 0.01},
                    new Object[] {"HeightScale", 100},
                    new Object[] {"WidthScale", 100},
                    new Object[] {"IsLockAspectRatio", true},
                    //==========Protection==========//
                    new Object[] {"IsLocked", true},
                    //==========Properties==========//
                    new Object[] {"Placement", PlacementType.FreeFloating}
                });
                ReflectInvoker.invoke("comment.CommentShape.LineFormat", comment.CommentShape.LineFormat, new Object[][]{
                     //==========Lines============//
                         new Object[] {"DashStyle", MsoLineDashStyle.Solid},
                         new Object[] {"Style", MsoLineStyle.Single},
                         new Object[] {"Weight", 0.75}
                      });              
                AssertHelper.equals(Color.Black, comment.CommentShape.LineFormat.ForeColor, "comment.CommentShape.LineFormat.ForeColor");

                ReflectInvoker.invoke("comment.Font", comment.Font, new Object[][]{
                    new Object[] {"Name", "Verdana"},
                    new Object[] {"Size", 10},
                    new Object[] {"Underline", FontUnderlineType.Single},
                    new Object[] {"IsStrikeout", false},
                    new Object[] {"IsSubscript", false},
                    new Object[] {"IsSuperscript", false}
                   });
            }
        }
```

### See Also

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


