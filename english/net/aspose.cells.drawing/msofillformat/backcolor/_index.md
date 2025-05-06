---
title: MsoFillFormat.BackColor
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormat property. Gets and sets the file back color
type: docs
url: /net/aspose.cells.drawing/msofillformat/backcolor/
---
## MsoFillFormat.BackColor property

Gets and sets the file back color.

```csharp
public Color BackColor { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.equals(groupSrc.FillFormat.BackColor, groupDest.FillFormat.BackColor, info + &amp;quot;.FillFormat.BackColor&amp;quot;);
public static void Property_BackColor(GroupShape groupSrc, GroupShape groupDest, string info)
        {
            
            if (AssertHelper.checkNull(groupSrc, groupDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(groupSrc.UpperLeftRow, groupDest.UpperLeftRow, info + &quot;.UpperLeftRow&quot;);
            AssertHelper.AreEqual(groupSrc.UpperLeftColumn, groupDest.UpperLeftColumn, info + &quot;.UpperLeftColumn&quot;);
            AssertHelper.AreEqual(groupSrc.LowerRightRow, groupDest.LowerRightRow, info + &quot;.LowerRightRow&quot;);
            AssertHelper.AreEqual(groupSrc.LowerRightColumn, groupDest.LowerRightColumn, info + &quot;.LowerRightColumn&quot;);   
            //==================compare colors and lines===============//
            AssertHelper.AreEqual(groupSrc.FillFormat.IsVisible, groupDest.FillFormat.IsVisible, info + &quot;.FillFormat.IsVisible&quot;);
            if (groupSrc.FillFormat.IsVisible &amp;&amp; groupDest.FillFormat.IsVisible)
            {
                AssertHelper.Property_BackColor(groupSrc.FillFormat.ForeColor, groupDest.FillFormat.ForeColor, info + &quot;.FillFormat.ForeColor&quot;);
                AssertHelper.Property_BackColor(groupSrc.FillFormat.BackColor, groupDest.FillFormat.BackColor, info + &quot;.FillFormat.BackColor&quot;);
                AssertHelper.AreEqual(groupSrc.FillFormat.Transparency, groupDest.FillFormat.Transparency, info + &quot;.FillFormat.Transparency&quot;);
            }
            AssertHelper.AreEqual(groupSrc.LineFormat.IsVisible, groupDest.LineFormat.IsVisible, info + &quot;.LineFormat.IsVisible&quot;);
            if (groupSrc.LineFormat.IsVisible &amp;&amp; groupDest.LineFormat.IsVisible)
            {
                AssertHelper.Property_BackColor(groupSrc.LineFormat.ForeColor, groupDest.LineFormat.ForeColor, info + &quot;.LineFormat.ForeColor&quot;);
                AssertHelper.AreEqual(groupSrc.LineFormat.BackColor, groupDest.LineFormat.BackColor, info + &quot;.LineFormat.BackColor&quot;);
                AssertHelper.AreEqual(groupSrc.LineFormat.Style, groupDest.LineFormat.Style, info + &quot;.LineFormat.Style&quot;);
                AssertHelper.AreEqual(groupSrc.LineFormat.DashStyle, groupDest.LineFormat.DashStyle, info + &quot;.LineFormat.DashStyle&quot;);
                AssertHelper.AreEqual(groupSrc.LineFormat.Weight, groupDest.LineFormat.Weight, info + &quot;.LineFormat.Weight&quot;);
            }
            //======================compare size=====================//
            AssertHelper.AreEqual(groupSrc.HeightCM, groupDest.HeightCM, info + &quot;.HeightCM&quot;);
            AssertHelper.AreEqual(groupSrc.WidthCM, groupDest.WidthCM, info + &quot;.WidthCM&quot;);
            AssertHelper.AreEqual(groupSrc.RotationAngle, groupDest.RotationAngle, info + &quot;.RotationAngle&quot;);
            AssertHelper.AreEqual(groupSrc.HeightScale, groupDest.HeightScale, info + &quot;.HeightScale&quot;);
            AssertHelper.AreEqual(groupSrc.WidthScale, groupDest.WidthScale, info + &quot;.WidthScale&quot;);
            AssertHelper.AreEqual(groupSrc.IsLockAspectRatio, groupDest.IsLockAspectRatio, info + &quot;.IsLockAspectRatio&quot;);
            //======================compare protection================//
            AssertHelper.AreEqual(groupSrc.IsLocked, groupDest.IsLocked, info + &quot;.IsLocked&quot;);
            //======================compare properties================//
            AssertHelper.AreEqual(groupSrc.Placement, groupDest.Placement, info + &quot;.Placement&quot;);
            AssertHelper.AreEqual(groupSrc.IsPrintable, groupDest.IsPrintable, info + &quot;.IsPrintable&quot;);
        }
```

### See Also

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


