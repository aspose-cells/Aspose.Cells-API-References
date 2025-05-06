---
title: LoadOptions.StandardFontSize
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Sets the default standard font size
type: docs
url: /net/aspose.cells/loadoptions/standardfontsize/
---
## LoadOptions.StandardFontSize property

Sets the default standard font size.

```csharp
[Obsolete("Use DefaultStyleSettings.FontSize property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double StandardFontSize { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: loadOptions.StandardFontSize = 11;
[Test]
        public void Property_StandardFontSize()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET45057/&quot;;
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.SupportDivTag = true;
            loadOptions.KeepPrecision = true;
            loadOptions.DeleteRedundantSpaces = true;
            loadOptions.AutoFitColsAndRows = true;
            loadOptions.StandardFont = &quot;Calibri&quot;;
            loadOptions.StandardFontSize = 11;

            Workbook wb = new Workbook(filePath + &quot;s1.htm&quot;, loadOptions);


            var worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;
            Assert.AreEqual(cells[&quot;A1&quot;].GetStyle().Font.Name, &quot;Calibri&quot;);
            Assert.AreEqual(cells[&quot;A1&quot;].GetStyle().Font.Size, 11);

            Assert.AreEqual(cells[&quot;D11&quot;].GetStyle().IsTextWrapped, true);
            Assert.AreEqual(cells[&quot;G11&quot;].GetStyle().IsTextWrapped, true);

            Assert.AreEqual(cells[&quot;A28&quot;].GetStyle().IsTextWrapped, true);
            Assert.AreEqual(cells[&quot;A28&quot;].GetStyle().VerticalAlignment, TextAlignmentType.Center);
            Console.WriteLine(cells[&quot;A28&quot;].GetStyle().Font.Color);
            if (cells[&quot;A28&quot;].IsRichText())
            {
                Assert.AreEqual(cells[&quot;A28&quot;].GetCharacters()[0].Font.Color, Color.FromArgb(255, 220, 20, 60));
            }
            else
            {
                Assert.AreEqual(cells[&quot;A28&quot;].GetStyle().Font.Color, Color.FromArgb(255, 220, 20, 60));
            }

            Assert.AreEqual(cells[&quot;A292&quot;].GetStyle().Borders[BorderType.TopBorder].LineStyle, CellBorderType.None);

            Assert.Greater(cells.Columns[0].Width, 35);
            Assert.Greater(cells.Columns[6].Width, 25);

            for (int i = 0; i &lt; worksheet.Pictures.Count; i++)
            {
                Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[i];
                pic.Height = 250;
                pic.Width = 300;
                worksheet.Cells.SetRowHeight(pic.UpperLeftRow, 200);

            }

            wb.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;);
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


