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
// Called: MsoFillFormatTest.equals(picSrc.FillFormat, picDest.FillFormat, info + ".FillFormat");
public static void Shape_Property_FillFormat(Picture picSrc, Picture picDest, string info)
        {
            if (AssertHelper.checkNull(picSrc, picDest, info))
            {
                return;
            }
            AssertHelper.Shape_Property_FillFormat(picSrc.BorderLineColor, picDest.BorderLineColor, info + ".BorderLineColor");
            AssertHelper.AreEqual(picSrc.BorderWeight, picDest.BorderWeight, info + ".BorderWeight");
            //AssertHelper.AreEqual(picSrc.Data,
            MsoFillFormatTest.Shape_Property_FillFormat(picSrc.FillFormat, picDest.FillFormat, info + ".FillFormat");
            //AssertHelper.AreEqual(picSrc.Left, picDest.Left, info + ".Left");
            //AssertHelper.AreEqual(picSrc.LeftCM, picDest.LeftCM, delta, info + ".LeftCM");
            //AssertHelper.AreEqual(picSrc.LeftInch, picDest.LeftInch, delta, info + ".LeftInch");
            //AssertHelper.AreEqual(picSrc.LeftInShape, picDest.LeftInShape, info + ".LeftInShape");
            //AssertHelper.AreEqual(picSrc.OriginalHeight, picDest.OriginalHeight, info + ".OriginalHeight");
            //AssertHelper.AreEqual(picSrc.OriginalWidth, picDest.OriginalWidth, info + ".OriginalWidth");
            //AssertHelper.AreEqual(picSrc.Top, picDest.Top, info + ".Top");
            //AssertHelper.AreEqual(picSrc.TopCM, picDest.TopCM, delta, info + ".TopCM");
            //AssertHelper.AreEqual(picSrc.TopInch, picDest.TopInch, delta, info + ".TopInch");
            //AssertHelper.AreEqual(picSrc.TopInShape, picDest.TopInShape, info + ".TopInShape");
            AssertHelper.AreEqual(picSrc.ImageType, picDest.ImageType, info + ".ImageFormat");
        }
```

### See Also

* class [MsoFillFormat](../../msofillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


