---
title: Worksheet.Type
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents worksheet type
type: docs
url: /net/aspose.cells/worksheet/type/
---
## Worksheet.Type property

Represents worksheet type.

```csharp
public SheetType Type { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(expected.Type, result.Type, info + &amp;quot;.Type&amp;quot;);
private static void Property_Type(Worksheet expected, Worksheet result, string info)
        {
            //Options
            AssertHelper.AreEqual(expected.Name, result.Name, info + &quot;.Name&quot;);
            AssertHelper.AreEqual(expected.Index, result.Index, info + &quot;.Index&quot;);
            AssertHelper.AreEqual(expected.ActiveCell, result.ActiveCell, info + &quot;.ActiveCell&quot;);
            AssertHelper.AreEqual(expected.CodeName, result.CodeName, info + &quot;.CodeName&quot;);
            AssertHelper.AreEqual(expected.IsVisible, result.IsVisible, info + &quot;.IsVisible&quot;);
            AssertHelper.equals(expected.TabColor, result.TabColor, info + &quot;.TabColor&quot;);
            AssertHelper.AreEqual(expected.Type, result.Type, info + &quot;.Type&quot;);
            AssertHelper.AreEqual(expected.Zoom, result.Zoom, info + &quot;.Zoom&quot;);
            AssertHelper.AreEqual(expected.DisplayRightToLeft, result.DisplayRightToLeft, info + &quot;.DisplayRightToLeft&quot;);
            AssertHelper.AreEqual(expected.FirstVisibleColumn, result.FirstVisibleColumn, info + &quot;.FirstVisibleColumn&quot;);
            AssertHelper.AreEqual(expected.FirstVisibleRow, result.FirstVisibleRow, info + &quot;.FirstVisibleRow&quot;);
            AssertHelper.AreEqual(expected.IsGridlinesVisible, result.IsGridlinesVisible, info + &quot;.IsGridlinesVisible&quot;);
            AssertHelper.AreEqual(expected.IsPageBreakPreview, result.IsPageBreakPreview, info + &quot;.IsPageBreakPreview&quot;);
            AssertHelper.AreEqual(expected.IsProtected, result.IsProtected, info + &quot;.IsProtected&quot;);
            AssertHelper.AreEqual(expected.IsRowColumnHeadersVisible, result.IsRowColumnHeadersVisible, info + &quot;.IsRowColumnHeadersVisible&quot;);
            AssertHelper.AreEqual(expected.IsVisible, result.IsVisible, info + &quot;.IsVisible&quot;);         
        }
```

### See Also

* enum [SheetType](../../sheettype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


