---
title: Hyperlink.TextToDisplay
second_title: Aspose.Cells for .NET API Reference
description: Hyperlink property. Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink
type: docs
url: /net/aspose.cells/hyperlink/texttodisplay/
---
## Hyperlink.TextToDisplay property

Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink.

```csharp
public string TextToDisplay { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets[0].Hyperlinks[0].TextToDisplay = &amp;quot;test&amp;quot;;
[Test]
        public void Property_TextToDisplay()
        {
            Workbook workbook = new Workbook();

            workbook.Worksheets[0].Hyperlinks.Add(&quot;A1&quot;, 1, 1, &quot;www.baidu.com&quot;);
            workbook.Worksheets[0].Hyperlinks[0].TextToDisplay = &quot;test&quot;;

           AssertHelper.AreEqual(System.Drawing.Color.Blue, workbook.Worksheets[0].Cells[&quot;A1&quot;].GetStyle().Font.Color);
            workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA42722.xlsx&quot;);
            workbook.Worksheets[0].Hyperlinks[0].TextToDisplay = &quot;test&quot;;
            Assert.AreEqual(20, workbook.Worksheets[0].Cells[&quot;B4&quot;].GetStyle().Font.Size);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA42722.xlsx&quot;);
        }
```

### See Also

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


