---
title: Font.ArgbColor
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets and sets the color with a 32bit ARGB value
type: docs
url: /net/aspose.cells/font/argbcolor/
---
## Font.ArgbColor property

Gets and sets the color with a 32-bit ARGB value.

```csharp
public int ArgbColor { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(0xFFFF0000, cell.GetDisplayStyle().Font.ArgbColor &amp;amp; 0xFFFFFFFF);
[Test]
        public void Property_ArgbColor()
        {
            string sourcePath = Constants.sourcePath + &quot;CELLSNET-49610/&quot;;
            Workbook wb = new Workbook(sourcePath + &quot;Template.xlsx&quot;);

            wb.ImportXml(sourcePath + &quot;xml.xml&quot;, &quot;Sheet1&quot;, 0, 0);

            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                ms.Position = 0;

                Workbook reloadWb = new Workbook(ms);
                Worksheet sheet = reloadWb.Worksheets[0];
                Assert.AreEqual(148, sheet.ListObjects[0].EndRow + 1);

                Cells cells = sheet.Cells;
                Cell cell = cells[&quot;A148&quot;];
                Assert.AreEqual(&quot;AGR/SB/WATERGANG3078&quot;, cell.DisplayStringValue);
                Assert.AreEqual(0xFFFFFF00, cell.GetDisplayStyle().ForegroundArgbColor &amp; 0xFFFFFFFF);

                cell = cells[&quot;J148&quot;];
                Assert.AreEqual(&quot;Bellville&quot;, cell.DisplayStringValue);
                Assert.AreEqual(0xFF4472C4, cell.GetDisplayStyle().ForegroundArgbColor &amp; 0xFFFFFFFF);

                cell = cells[&quot;F148&quot;];
                Assert.AreEqual(&quot;29 January 2021&quot;, cell.DisplayStringValue);
                Assert.AreEqual(0xFFFF0000, cell.GetDisplayStyle().Font.ArgbColor &amp; 0xFFFFFFFF);


                //TODO:
                //Assert.AreEqual(&quot;04228958007&quot;, cells[&quot;C148&quot;].DisplayStringValue);
                //Assert.AreEqual(&quot;Domestic Low 01&quot;, cells[&quot;D148&quot;].DisplayStringValue);
                //Assert.AreEqual(&quot;Cape Town&quot;, cells[&quot;H148&quot;].DisplayStringValue);
                //Assert.AreEqual(&quot;NP_TEST&quot;, cells[&quot;G148&quot;].DisplayStringValue);

                //Assert.IsTrue(string.IsNullOrEmpty(cells[&quot;C25&quot;].DisplayStringValue));
                //Assert.IsTrue(string.IsNullOrEmpty(cells[&quot;D25&quot;].DisplayStringValue));

                //Assert.IsTrue(string.IsNullOrEmpty(cells[&quot;H39&quot;].DisplayStringValue));
                //Assert.IsTrue(string.IsNullOrEmpty(cells[&quot;I39&quot;].DisplayStringValue));


            }

        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


