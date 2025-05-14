---
title: DefaultStyleSettings.VerticalAlignment
second_title: Aspose.Cells for .NET API Reference
description: DefaultStyleSettings property. Gets/Sets the default value for vertical alignment
type: docs
url: /net/aspose.cells/defaultstylesettings/verticalalignment/
---
## DefaultStyleSettings.VerticalAlignment property

Gets/Sets the default value for vertical alignment

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Examples

```csharp
// Called: options.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
public void DefaultStyleSettings_Property_VerticalAlignment()
{
    string filePath = Constants.PivotTableSourcePath + @"NET50344_";
    string savePath = CreateFolder(filePath);

    LoadOptions options = new LoadOptions();
    //set default vertical alignment
    options.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;

    Workbook wb = new Workbook(filePath + "testdoc.XLSM", options);
    wb.Save(savePath + "out.pdf");

    Cells cells = wb.Worksheets[0].Cells;
    Assert.AreEqual(cells["C12"].GetStyle().IsTextWrapped, true);
    Assert.AreEqual(cells["D12"].GetStyle().IsTextWrapped, false);
    Assert.AreEqual(cells["E12"].GetStyle().IsTextWrapped, false);

    Assert.AreEqual(cells["C12"].GetStyle().VerticalAlignment, TextAlignmentType.Bottom);
    Assert.AreEqual(cells["D12"].GetStyle().VerticalAlignment, TextAlignmentType.Bottom);
    Assert.AreEqual(cells["E12"].GetStyle().VerticalAlignment, TextAlignmentType.Bottom);
}
```

### See Also

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


