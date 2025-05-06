---
title: AbstractTextLoadOptions.KeepPrecision
second_title: Aspose.Cells for .NET API Reference
description: AbstractTextLoadOptions property. Indicates whether not parsing a string value if the length is 15
type: docs
url: /net/aspose.cells/abstracttextloadoptions/keepprecision/
---
## AbstractTextLoadOptions.KeepPrecision property

Indicates whether not parsing a string value if the length is 15.

```csharp
public bool KeepPrecision { get; set; }
```

### Examples

```csharp
// Called: loadOptions.KeepPrecision = true;
[Test]
        public void Property_KeepPrecision()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET44987And44988And44989And44990/&quot;;

            //var htmlString = File.ReadAllText(filePath + &quot;input_sourceBaidu.html&quot;);
            var htmlString = File.ReadAllText(filePath + &quot;input.html&quot;);
            using (MemoryStream ms = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(htmlString)))
            {

                Aspose.Cells.HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
                loadOptions.SupportDivTag = true;
                loadOptions.KeepPrecision = true;
                Workbook wb = new Workbook(ms, loadOptions);
                wb.Worksheets[0].AutoFitRows();
                wb.Worksheets[0].AutoFitColumns();
                var worksheet = wb.Worksheets[0];
                for (int i = 0; i &lt; worksheet.Pictures.Count; i++)
                {
                    Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[i];
                    pic.Height = 250;
                    pic.Width = 300;
                    worksheet.Cells.SetRowHeight(pic.UpperLeftRow, 200);
                }
                Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A1&quot;].StringValue, &quot;testtesttest teststeststestes&quot;);

                Cell a28 = wb.Worksheets[0].Cells[&quot;A28&quot;];
                Assert.AreEqual(a28.StringValue, &quot;test&quot;);

                if (a28.IsRichText())
                {
                    Assert.AreEqual(a28.GetCharacters()[0].Font.Color, Color.FromArgb(255, 220, 20, 60));
                    Assert.AreEqual(a28.GetCharacters()[0].Font.IsBold, true);
                }
                else
                {
                    Assert.AreEqual(a28.GetStyle().Font.Color, Color.FromArgb(255, 220, 20, 60));
                    Assert.AreEqual(a28.GetStyle().Font.IsBold, true);
                }


                Assert.AreEqual(wb.Worksheets[0].Cells[&quot;D26&quot;].GetStyle().Font.IsBold, true);

                Assert.AreEqual(wb.Worksheets[0].Cells[&quot;D27&quot;].GetStyle().Font.IsBold, true);
                wb.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;, Aspose.Cells.SaveFormat.Xlsx);
            }
        }
```

### See Also

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


