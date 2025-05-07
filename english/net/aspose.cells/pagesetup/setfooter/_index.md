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
// Called: ps.SetFooter(0, "Footer");
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            ps.IsHFDiffFirst = true;
            ps.IsHFDiffOddEven = true;
            ps.SetEvenFooter(0, "EvenFooter");
            ps.SetFooter(0, "Footer");
            ps.SetFirstPageFooter(0, "FirstPageFooter");
            workbook.Save(Constants.destPath + "CellsJava43425.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsJava43425.xlsx");
            ps = workbook.Worksheets[0].PageSetup;
            Assert.IsTrue(ps.IsHFDiffFirst);
            Assert.IsTrue(ps.IsHFDiffOddEven);
            Assert.AreEqual("EvenFooter", ps.GetEvenFooter(0));
            Assert.AreEqual("Footer", ps.GetFooter(0));
            Assert.AreEqual("FirstPageFooter", ps.GetFirstPageFooter(0));
            Workbook tmp = new Workbook();
            tmp.Copy(workbook);
            ps = tmp.Worksheets[0].PageSetup;
            Assert.IsTrue(ps.IsHFDiffFirst);
            Assert.IsTrue(ps.IsHFDiffOddEven);
            Assert.AreEqual("EvenFooter", ps.GetEvenFooter(0));
            Assert.AreEqual("Footer", ps.GetFooter(0));
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


