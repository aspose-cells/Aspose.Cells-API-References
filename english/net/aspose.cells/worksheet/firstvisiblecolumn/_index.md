---
title: Worksheet.FirstVisibleColumn
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents first visible column index
type: docs
url: /net/aspose.cells/worksheet/firstvisiblecolumn/
---
## Worksheet.FirstVisibleColumn property

Represents first visible column index.

```csharp
public int FirstVisibleColumn { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(expected.FirstVisibleColumn, result.FirstVisibleColumn, info + ".FirstVisibleColumn");
private static void Property_FirstVisibleColumn(Worksheet expected, Worksheet result, string info)
        {
            //Options
            AssertHelper.AreEqual(expected.Name, result.Name, info + ".Name");
            AssertHelper.AreEqual(expected.Index, result.Index, info + ".Index");
            AssertHelper.AreEqual(expected.ActiveCell, result.ActiveCell, info + ".ActiveCell");
            AssertHelper.AreEqual(expected.CodeName, result.CodeName, info + ".CodeName");
            AssertHelper.AreEqual(expected.IsVisible, result.IsVisible, info + ".IsVisible");
            AssertHelper.equals(expected.TabColor, result.TabColor, info + ".TabColor");
            AssertHelper.AreEqual(expected.Type, result.Type, info + ".Type");
            AssertHelper.AreEqual(expected.Zoom, result.Zoom, info + ".Zoom");
            AssertHelper.AreEqual(expected.DisplayRightToLeft, result.DisplayRightToLeft, info + ".DisplayRightToLeft");
            AssertHelper.AreEqual(expected.FirstVisibleColumn, result.FirstVisibleColumn, info + ".FirstVisibleColumn");
            AssertHelper.AreEqual(expected.FirstVisibleRow, result.FirstVisibleRow, info + ".FirstVisibleRow");
            AssertHelper.AreEqual(expected.IsGridlinesVisible, result.IsGridlinesVisible, info + ".IsGridlinesVisible");
            AssertHelper.AreEqual(expected.IsPageBreakPreview, result.IsPageBreakPreview, info + ".IsPageBreakPreview");
            AssertHelper.AreEqual(expected.IsProtected, result.IsProtected, info + ".IsProtected");
            AssertHelper.AreEqual(expected.IsRowColumnHeadersVisible, result.IsRowColumnHeadersVisible, info + ".IsRowColumnHeadersVisible");
            AssertHelper.AreEqual(expected.IsVisible, result.IsVisible, info + ".IsVisible");         
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


