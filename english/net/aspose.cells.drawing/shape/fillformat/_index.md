---
title: Shape.FillFormat
second_title: Aspose.Cells for .NET API Reference
description: Shape property. Returns a MsoFillFormat object that contains fill formatting properties for the specified shape
type: docs
url: /net/aspose.cells.drawing/shape/fillformat/
---
## Shape.FillFormat property

Returns a MsoFillFormat object that contains fill formatting properties for the specified shape.

```csharp
[Obsolete("Use Shape.Fill property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoFillFormat FillFormat { get; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use Shape.Fill property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: MsoFillFormatTest.equals(ovalSrc.FillFormat, ovalDest.FillFormat, info + &amp;quot;.FillFormat&amp;quot;);
public static void Property_FillFormat(Oval ovalSrc, Oval ovalDest, string info)
        {
            if (AssertHelper.checkNull(ovalSrc, ovalDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(ovalSrc.MsoDrawingType, ovalDest.MsoDrawingType, info + &quot;.MsoDrawingType&quot;);
            AssertHelper.AreEqual(ovalSrc.UpperLeftRow, ovalDest.UpperLeftRow, info + &quot;.UpperLeftRow&quot;);
            AssertHelper.AreEqual(ovalSrc.UpperLeftColumn, ovalDest.UpperLeftColumn, info + &quot;.UpperLeftColumn&quot;);
            AssertHelper.AreEqual(ovalSrc.LowerRightRow, ovalDest.LowerRightRow, info + &quot;.LowerRightRow&quot;);
            AssertHelper.AreEqual(ovalSrc.LowerRightColumn, ovalDest.LowerRightColumn, info + &quot;.LowerRightColumn&quot;);
            AssertHelper.AreEqual(ovalSrc.Text, ovalDest.Text, info + &quot;.Text&quot;);
            //===================these properties are supported in excel 2003 format file================//
            //===font===//
            FontTest.Property_FillFormat(ovalSrc.Font, ovalDest.Font, info + &quot;.Font&quot;);
            //===Alignment===//
            AssertHelper.AreEqual(ovalSrc.TextHorizontalAlignment, ovalDest.TextHorizontalAlignment, info + &quot;.TextHorizontalAlignment&quot;);
            AssertHelper.AreEqual(ovalSrc.TextVerticalAlignment, ovalDest.TextVerticalAlignment, info + &quot;.TextVerticalAlignment&quot;);
            AssertHelper.AreEqual(ovalSrc.TextOrientationType, ovalDest.TextOrientationType, info + &quot;.TextOrientationType&quot;);             
            //ȱ��TextDirection
            //===colors and lines===//
            MsoFillFormatTest.Property_FillFormat(ovalSrc.FillFormat, ovalDest.FillFormat, info + &quot;.FillFormat&quot;);
            MsoLineFormatTest.Property_FillFormat(ovalSrc.LineFormat, ovalDest.LineFormat, info + &quot;.LineFormat&quot;);
            //===size===//
            AssertHelper.AreEqual(ovalSrc.HeightCM, ovalDest.HeightCM, info + &quot;.HeightCM&quot;);
            AssertHelper.AreEqual(ovalSrc.WidthCM, ovalDest.WidthCM, info + &quot;.WidthCM&quot;);
            AssertHelper.AreEqual(ovalSrc.RotationAngle, ovalDest.RotationAngle, info + &quot;.RotationAngle&quot;);
            AssertHelper.AreEqual(ovalSrc.HeightScale, ovalDest.HeightScale, info + &quot;.HeightScale&quot;);
            AssertHelper.AreEqual(ovalSrc.WidthScale, ovalDest.WidthScale, info + &quot;.WidthScale&quot;);
            AssertHelper.AreEqual(ovalSrc.IsLockAspectRatio, ovalDest.IsLockAspectRatio, info + &quot;.IsLockAspectRatio&quot;);
            //===protection===//
            AssertHelper.AreEqual(ovalSrc.IsLocked, ovalDest.IsLocked, info + &quot;.IsLocked&quot;);
            //===properties===//
            AssertHelper.AreEqual(ovalSrc.Placement, ovalDest.Placement, info + &quot;.Placement&quot;);
            AssertHelper.AreEqual(ovalSrc.IsPrintable, ovalDest.IsPrintable, info + &quot;.IsPrintable&quot;);
            //===Margins===//
            TextFrameTest.Property_FillFormat(ovalSrc.TextBody.TextAlignment, ovalDest.TextBody.TextAlignment, info + &quot;.TextFrame&quot;);
            //===web===//
            AssertHelper.AreEqual(ovalSrc.AlternativeText, ovalDest.AlternativeText, info + &quot;.AlternativeText&quot;);
            //other
            AssertHelper.AreEqual(ovalSrc.IsHidden, ovalDest.IsHidden, info + &quot;.IsHidden&quot;);
            AssertHelper.AreEqual(ovalSrc.IsGroup, ovalDest.IsGroup, info + &quot;.IsGroup&quot;);

             CharactersTest.Property_FillFormat(ovalSrc.GetRichFormattings(), ovalDest.GetRichFormattings(), info + &quot;.GetCharacters()&quot;);
            HyperlinksTest.Property_FillFormat(ovalSrc.Hyperlink, ovalDest.Hyperlink, info + &quot;.Hyperlink&quot;);


            //============================these properties are supported in excel 2007 format===============//
            
          
          
        }
```

### See Also

* class [MsoFillFormat](../../msofillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


