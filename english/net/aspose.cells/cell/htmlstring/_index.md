---
title: Cell.HtmlString
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets and sets the html string which contains data and some formats in this cell
type: docs
url: /net/aspose.cells/cell/htmlstring/
---
## Cell.HtmlString property

Gets and sets the html string which contains data and some formats in this cell.

```csharp
public string HtmlString { get; set; }
```

### Examples

```csharp
// Called: cell.HtmlString = ("<p><em>Italics</em></p>");
[Test]
        public void Property_HtmlString()
        {
            Workbook workbook = new Workbook();
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            cell.HtmlString = ("<td height=17 class=xl66 width=64 style='height:12.75pt;width:48pt'><a href=\"http://google.com\" target=\"_parent\">google</a></td>");
            Assert.AreEqual(1, workbook.Worksheets[0].Hyperlinks.Count);

            cell = workbook.Worksheets[0].Cells["A3"];
            cell.HtmlString = ("<p>First Line</p><p>Next Line</p>");
            Assert.IsTrue(cell.GetStyle().IsTextWrapped);

            cell = workbook.Worksheets[0].Cells["A6"];
            cell.HtmlString = ("<ul><li>First Bullet</li><li>Second Bullet</li></ul>");

            cell = workbook.Worksheets[0].Cells["A9"];
            cell.HtmlString = ("<p><em>Italics</em></p>");
            Assert.IsTrue(cell.GetStyle().Font.IsItalic);

            cell = workbook.Worksheets[0].Cells["A12"];
            cell.HtmlString = ("<p style='margin:0cm;margin-bottom:.0001pt;font-size:16px;font-family:Cambria;'><span style='font-family:&quot;Arial Black&quot;'>Arial Black</span></p>");
            Assert.AreEqual(cell.GetStyle().Font.Name, "Arial Black" );

            cell = workbook.Worksheets[0].Cells["A15"];
            cell.HtmlString = ("<p style='margin:0cm;margin-bottom:.0001pt;font-size:16px;font-family:Cambria;'>First Para</p><p style='margin:0cm;margin-bottom:.0001pt;font-size:16px;font-family:Cambria;'><br></p><p style='margin:0cm;margin-bottom:.0001pt;font-size:16px;font-family:Cambria;'>Second Para</p><p style='margin:0cm;margin-bottom:.0001pt;font-size:16px;font-family:Cambria;'><br></p><p style='margin:0cm;margin-bottom:.0001pt;font-size:16px;font-family:Cambria;'>Third Para</p>");


            workbook.Save(Constants.destPath + "CELLSJAVA43039.xlsx");
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


