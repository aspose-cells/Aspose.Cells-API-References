---
title: Worksheet.TextBoxes
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets a TextBox collection
type: docs
url: /net/aspose.cells/worksheet/textboxes/
---
## Worksheet.TextBoxes property

Gets a [`TextBox`](../../../aspose.cells.drawing/textbox/) collection.

```csharp
public TextBoxCollection TextBoxes { get; }
```

### Examples

```csharp
// Called: TextBoxCollection textboxes = sheet.TextBoxes;
private void Property_TextBoxes(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            TextBoxCollection textboxes = sheet.TextBoxes;
            AssertHelper.AreEqual(1, textboxes.Count, &quot;sheet.TextBoxes.Count&quot;);
            TextBox textbox = textboxes[0];
            AssertHelper.AreEqual(TextOrientationType.NoRotation, textbox.TextOrientationType, &quot;textbox.TextOrientationType&quot;);
        }
```

### See Also

* class [TextBoxCollection](../../../aspose.cells.drawing/textboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


