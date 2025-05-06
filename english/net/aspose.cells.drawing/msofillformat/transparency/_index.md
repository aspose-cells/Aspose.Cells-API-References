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
// Called: AssertHelper.AreEqual(0.2, picture.FillFormat.Transparency, 0.01, &amp;quot;picture.FillFormat.Transparency&amp;quot;);
public void Property_Transparency(Picture picture)
        {
            if (picture.UpperLeftRow == 4 &amp;&amp; picture.UpperLeftColumn == 2
                &amp;&amp; picture.LowerRightRow == 9 &amp;&amp; picture.LowerRightColumn == 6)
            {
               
                ReflectInvoker.invoke(&quot;picture&quot;, picture, new Object[][]{
                    new Object[] {&quot;HeightCM&quot;, 2.65, 0.01},
                    new Object[] {&quot;WidthCM&quot;, 6.61, 0.01},
                    new Object[] {&quot;RotationAngle&quot;, 0.0},
                    new Object[] {&quot;HeightScale&quot;, 100},
                    new Object[] {&quot;WidthScale&quot;, 100},
                    new Object[] {&quot;IsLockAspectRatio&quot;, true},
                   // new Object[] {&quot;OriginalHeight&quot;, 2.65, 0.01},
                  //  new Object[] {&quot;OriginalWidth&quot;, 6.62, 0.01},
                    new Object[] {&quot;IsLocked&quot;, true},
                    new Object[] {&quot;Placement&quot;, PlacementType.MoveAndSize},
                    new Object[] {&quot;IsPrintable&quot;, true}
                 });
               
                AssertHelper.AreEqual(true, picture.FillFormat.IsVisible, &quot;picture.FillFormat.IsVisible&quot;);
               
                AssertHelper.equals(Color.Red, picture.FillFormat.ForeColor, &quot;picture.FillFormat.ForeColor&quot;);
               
                AssertHelper.AreEqual(0.0, picture.FillFormat.Transparency, &quot;picture.FillFormat.Transparency&quot;);
                
            }
            else if (picture.UpperLeftRow == 6 &amp;&amp; picture.UpperLeftColumn == 7 &amp;&amp; picture.LowerRightRow == 16 &amp;&amp; picture.LowerRightColumn == 8)
            {
                AssertHelper.equals(Color.Blue, picture.FillFormat.ForeColor, &quot;picture.FillFormat.ForeColor&quot;);
                AssertHelper.AreEqual(0.2, picture.FillFormat.Transparency, 0.01, &quot;picture.FillFormat.Transparency&quot;);
                
                ReflectInvoker.invoke(&quot;picture&quot;, picture, new Object[][]{
                    new Object[] {&quot;BorderLineColor&quot;, Color.Red},
                    new Object[] {&quot;BorderWeight&quot;, 0.75, 0.01},
                    //new Object[] {&quot;HeightCM&quot;, 1.69, 0.01},
                    //new Object[] {&quot;WidthCM&quot;, 5.37, 0.01},
                    new Object[] {&quot;RotationAngle&quot;, 60.0},
                    //new Object[] {&quot;HeightScale&quot;, 100},
                    //new Object[] {&quot;WidthScale&quot;, 100},
                    new Object[] {&quot;IsLockAspectRatio&quot;, true},
                    //new Object[] {&quot;OriginalHeight&quot;, 1.69},
                   // new Object[] {&quot;OriginalWidth&quot;, 5.37},
                    new Object[] {&quot;IsLockAspectRatio&quot;, true},
                    new Object[] {&quot;IsLocked&quot;, true},
                    new Object[] {&quot;Placement&quot;, PlacementType.Move},
                    new Object[] {&quot;IsPrintable&quot;, true}
                 });
            }
        }
```

### See Also

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


