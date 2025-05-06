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
[Test]
        public void Property_VerticalAlignment()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET50344_&quot;;
            string savePath = CreateFolder(filePath);

            LoadOptions options = new LoadOptions();
            //set default vertical alignment
            options.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;

            Workbook wb = new Workbook(filePath + &quot;testdoc.XLSM&quot;, options);
            wb.Save(savePath + &quot;out.pdf&quot;);

            Cells cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(cells[&quot;C12&quot;].GetStyle().IsTextWrapped, true);
            Assert.AreEqual(cells[&quot;D12&quot;].GetStyle().IsTextWrapped, false);
            Assert.AreEqual(cells[&quot;E12&quot;].GetStyle().IsTextWrapped, false);

            Assert.AreEqual(cells[&quot;C12&quot;].GetStyle().VerticalAlignment, TextAlignmentType.Bottom);
            Assert.AreEqual(cells[&quot;D12&quot;].GetStyle().VerticalAlignment, TextAlignmentType.Bottom);
            Assert.AreEqual(cells[&quot;E12&quot;].GetStyle().VerticalAlignment, TextAlignmentType.Bottom);
        }
```

### See Also

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


