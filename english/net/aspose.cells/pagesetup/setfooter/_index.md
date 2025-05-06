---
title: PageSetup.SetFooter
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Sets a script formatting the footer of an Excel file
type: docs
url: /net/aspose.cells/pagesetup/setfooter/
---
## PageSetup.SetFooter method

Sets a script formatting the footer of an Excel file.

```csharp
public void SetFooter(int section, string footerScript)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | String | Footer format script. |

### Remarks

Script commands:

| **Command** | **Description** |
| --- | --- |
| &amp;P | Current page number |
| &amp;N | Page count |
| &amp;D | Current date |
| &amp;T | Current time |
| &amp;A | Sheet name |
| &amp;F | File name without path |
| &amp;"&lt;FontName&gt;" | Font name, for example: &amp;"Arial" |
| &amp;"&lt;FontName&gt;, &lt;FontStyle&gt;" | Font name and font style, for example: &amp;"Arial,Bold" |
| &amp;&lt;FontSize&gt; | Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character. |
| &amp;K&lt;RRGGBB&gt; | Font color, for example(RED): &amp;KFF0000 |
| &amp;G | Image script |

For example: "&amp;Arial,Bold&amp;8Footer Note"

### Examples

```csharp
// Called: pageSetup.SetFooter(0, &amp;quot;&amp;amp;G&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                PageSetup pageSetup = worksheet.PageSetup;
                byte[] pic = File.ReadAllBytes(Constants.sourcePath + &quot;image1.png&quot;);
                Picture picture = pageSetup.SetFooterPicture(0, pic);
                picture.RelativeToOriginalPictureSize = false;
                pageSetup.SetFooter(0, &quot;&amp;G&quot;);
            }

            workbook.Save(Constants.destPath + &quot;CELLSNET47485.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET47485.xlsx&quot;);
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            Assert.IsFalse(ps.GetPicture(false, 0).RelativeToOriginalPictureSize);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


