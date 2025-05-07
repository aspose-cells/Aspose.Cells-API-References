---
title: TextOptions.LanguageCode
second_title: Aspose.Cells for .NET API Reference
description: TextOptions property. Gets and sets the user interface language
type: docs
url: /net/aspose.cells.drawing.texts/textoptions/languagecode/
---
## TextOptions.LanguageCode property

Gets and sets the user interface language.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(CountryCode.Japan,ws.Shapes[0].TextOptions.LanguageCode);
[Test]
        public void Property_LanguageCode()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet54628.xls");
            wb.Settings.Region = CountryCode.Japan;
            Worksheet ws = wb.Worksheets[0];
            ws.Shapes[0].HtmlText = ws.Shapes[1].HtmlText.Replace("REP", "１２３４５６７８９０１２３４５６７８９０１２３４５６７８９０１２３４５６７８９０１２３４５６７８９'０１２３４５６７８９０１２３４５６７８９０");
            Assert.AreEqual(CountryCode.Japan,ws.Shapes[0].TextOptions.LanguageCode);
            //FontSetting fs = shape.TextBody[0];
            wb.Save(Constants.destPath + "CellsNet54628.xls");
        }
```

### See Also

* enum [CountryCode](../../../aspose.cells/countrycode/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


