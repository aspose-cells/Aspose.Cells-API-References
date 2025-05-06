---
title: ReplaceOptions.MatchEntireCellContents
second_title: Aspose.Cells for .NET API Reference
description: ReplaceOptions property. Indicates whether to match entire cells contents
type: docs
url: /net/aspose.cells/replaceoptions/matchentirecellcontents/
---
## ReplaceOptions.MatchEntireCellContents property

Indicates whether to match entire cells contents

```csharp
public bool MatchEntireCellContents { get; set; }
```

### Remarks

The default value is true.

### Examples

```csharp
// Called: options.MatchEntireCellContents = false;
[Test]
        public void Property_MatchEntireCellContents()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet56074.xlsx&quot;);

            string text = &quot;asdf&quot;;
            string replacementText = &quot;text&quot;;

            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            FontSetting setting1 = new FontSetting(0, replacementText.Length, workbook.Worksheets);
            setting1.Font.IsBold = true;
            setting1.Font.Color = System.Drawing.Color.Blue;
            options.FontSettings = new FontSetting[] { setting1 };

            workbook.Replace(text, replacementText, options);


            FontSetting fs = workbook.Worksheets[0].Cells[&quot;B1&quot;].Characters(3, 4);
           Assert.IsTrue(Util.CompareColor(Color.Blue, fs.Font.Color));
            Assert.IsTrue(fs.Font.IsBold);

            workbook.Save(Constants.destPath + &quot;CellsNet56074.xlsx&quot;);
        }
```

### See Also

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


