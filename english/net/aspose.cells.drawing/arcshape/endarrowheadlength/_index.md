---
title: ArcShape.EndArrowheadLength
second_title: Aspose.Cells for .NET API Reference
description: ArcShape property. Gets and sets the end arrow head length of the line
type: docs
url: /net/aspose.cells.drawing/arcshape/endarrowheadlength/
---
## ArcShape.EndArrowheadLength property

Gets and sets the end arrow head length of the line.

```csharp
[Obsolete("Use Shape.Line.EndArrowheadLength property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoArrowheadLength EndArrowheadLength { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use Shape.Line.EndArrowheadLength property. This property will be removed 12 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AssertHelper.AreEqual(arcSrc.EndArrowheadLength, arcDest.EndArrowheadLength, info + ".EndArrowheadLength");
public static void ArcShape_Property_EndArrowheadLength(ArcShape arcSrc, ArcShape arcDest, string info)
        {
            if (AssertHelper.checkNull(arcSrc, arcDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(arcSrc.UpperLeftRow, arcDest.UpperLeftRow, info + ".UpperLeftRow");
            AssertHelper.AreEqual(arcSrc.UpperLeftColumn, arcDest.UpperLeftColumn, info + ".UpperLeftColumn");
            AssertHelper.AreEqual(arcSrc.LowerRightRow, arcDest.LowerRightRow, info + ".LowerRightRow");
            AssertHelper.AreEqual(arcSrc.LowerRightColumn, arcDest.LowerRightColumn, info + ".LowerRightColumn");
            //===========get values of  format shape and compare these==========//    
            //Fill option
            AssertHelper.AreEqual(arcSrc.FillFormat.IsVisible, arcDest.FillFormat.IsVisible, info + ".FillFormat.IsVisible");
            if (arcSrc.FillFormat.IsVisible && arcDest.FillFormat.IsVisible)
            {
                AssertHelper.ArcShape_Property_EndArrowheadLength(arcSrc.FillFormat.BackColor, arcDest.FillFormat.BackColor, info + ".FillFormat.BackColor");
                AssertHelper.ArcShape_Property_EndArrowheadLength(arcSrc.FillFormat.ForeColor, arcDest.FillFormat.ForeColor, info + ".FillFormat.ForeColor");
                AssertHelper.AreEqual(arcSrc.FillFormat.Transparency, arcDest.FillFormat.Transparency, info + ".FillFormat.Transparency");  
                AssertHelper.ArcShape_Property_EndArrowheadLength(arcSrc.FillFormat.ImageData, arcDest.FillFormat.ImageData, info+".ImageData");
                AssertHelper.AreEqual(arcSrc.FillFormat.Texture, arcDest.FillFormat.Texture, info+".Texture");
            }
            //Line Color option
            AssertHelper.AreEqual(arcSrc.LineFormat.IsVisible, arcDest.LineFormat.IsVisible, info + ".LineFormat.IsVisible");
            if (arcSrc.LineFormat.IsVisible && arcDest.LineFormat.IsVisible)
            {
                AssertHelper.ArcShape_Property_EndArrowheadLength(arcSrc.LineFormat.BackColor, arcDest.LineFormat.BackColor, info + ".LineFormat.BackColor");
                AssertHelper.ArcShape_Property_EndArrowheadLength(arcSrc.LineFormat.ForeColor, arcDest.LineFormat.ForeColor, info + ".LineFormat.ForeColor");
                AssertHelper.AreEqual(arcSrc.LineFormat.DashStyle, arcDest.LineFormat.DashStyle, info + ".LineFormat.DashStyle");
                AssertHelper.AreEqual(arcSrc.LineFormat.Style, arcDest.LineFormat.Style, info + ".LineFormat.Style");
                AssertHelper.AreEqual(arcSrc.LineFormat.Weight, arcDest.LineFormat.Weight, info + ".LineFormat.Weight");
                AssertHelper.AreEqual(arcSrc.LineFormat.Transparency, arcDest.LineFormat.Transparency, info+".Transparency");
            }
            //Line style option
            AssertHelper.AreEqual(arcSrc.BeginArrowheadStyle, arcDest.BeginArrowheadStyle, info + ".BeginArrowheadStyle");
            if (arcSrc.BeginArrowheadStyle != MsoArrowheadStyle.None && arcDest.BeginArrowheadStyle != MsoArrowheadStyle.None)
            {
                AssertHelper.AreEqual(arcSrc.BeginArrowheadLength, arcDest.BeginArrowheadLength, info + ".BeginArrowheadLength");
                AssertHelper.AreEqual(arcSrc.BeginArrowheadWidth, arcDest.BeginArrowheadWidth, info + ".BeginArrowheadWidth");
            }
            AssertHelper.AreEqual(arcSrc.EndArrowheadStyle, arcDest.EndArrowheadStyle, info + ".EndArrowheadStyle");
            if (arcSrc.EndArrowheadStyle != MsoArrowheadStyle.None && arcDest.EndArrowheadStyle != MsoArrowheadStyle.None)
            {
                AssertHelper.AreEqual(arcSrc.EndArrowheadLength, arcDest.EndArrowheadLength, info + ".EndArrowheadLength");
                AssertHelper.AreEqual(arcSrc.EndArrowheadWidth, arcDest.EndArrowheadWidth, info + ".EndArrowheadWidth");
            }
            //Shadow option
            //3-D Format option
            //3-D Rotation option
            //Picture option
            //TextBox option
            AssertHelper.AreEqual(arcSrc.TextVerticalAlignment, arcDest.TextVerticalAlignment, info+".TextVerticalAlignment");
            //==============size and properties options================//
            //size option 
            AssertHelper.AreEqual(arcSrc.Height, arcDest.Height, info + ".Height");
            AssertHelper.AreEqual(arcSrc.Width, arcDest.Width, info + ".Width");
            AssertHelper.AreEqual(arcSrc.RotationAngle, arcDest.RotationAngle, info + ".RotationAngle");
            AssertHelper.AreEqual(arcSrc.HeightScale, arcDest.HeightScale, info + ".HeightScale");
            AssertHelper.AreEqual(arcSrc.WidthScale, arcDest.WidthScale, info + ".WidthScale");
            AssertHelper.AreEqual(arcSrc.IsLockAspectRatio, arcDest.IsLockAspectRatio, info + ".IsLockAspectRatio");
            AssertHelper.AreEqual(arcSrc.RelativeToOriginalPictureSize, arcDest.RelativeToOriginalPictureSize, info+".RelativeToOriginalPictureSize");
            
            AssertHelper.AreEqual(arcSrc.Left, arcDest.Left, info+".Left");
            AssertHelper.AreEqual(arcSrc.Top, arcDest.Top, info+".Top");
            //properties option 
            AssertHelper.AreEqual(arcSrc.Placement, arcDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(arcSrc.IsPrintable, arcDest.IsPrintable, info + ".IsPrintable");
            AssertHelper.AreEqual(arcSrc.IsLocked, arcDest.IsLocked, info+".IsLocked");
            //alt text option
            AssertHelper.AreEqual(arcSrc.AlternativeText, arcDest.AlternativeText, info+".AlternativeText");
            //===============compare other==============//
            //===============compare protection===========//
            AssertHelper.AreEqual(arcSrc.IsLocked, arcDest.IsLocked, info + ".IsLocked");
            HyperlinksTest.ArcShape_Property_EndArrowheadLength(arcSrc.Hyperlink, arcDest.Hyperlink, info + ".Hyperlink");
            CellsColorTest.ArcShape_Property_EndArrowheadLength(arcSrc.FormatPicture.TransparentColor, arcSrc.FormatPicture.TransparentColor, info + ".TransparentColor");        

        }
```

### See Also

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [ArcShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


