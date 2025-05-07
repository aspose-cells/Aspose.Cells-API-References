---
title: FontSetting.Font
second_title: Aspose.Cells for .NET API Reference
description: FontSetting property. Returns the font of this object
type: docs
url: /net/aspose.cells/fontsetting/font/
---
## FontSetting.Font property

Returns the font of this object.

```csharp
public Font Font { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(fs.Font.IsBold);
[Test]
        public void Property_Font()
        {
            Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "CellsNet45649_2.xlsx");
            Worksheet ws = workbook.Worksheets[0];
            int idx = ws.Comments.Add("E8");
            Comment cm = ws.Comments[idx];
            //cm.HtmlNote = "<Font Style=\"FONT-WEIGHT: bold;FONT-FAMILY: Tahoma;FONT-SIZE: 9pt;COLOR: #000000;TEXT-ALIGN: left;\">Heading: </Font><Font Style=\"FONT-FAMILY: Tahoma;FONT-SIZE: 9pt;COLOR: #000000;TEXT-ALIGN: left;\">This is some para. </Font><Font Style=\"FONT-WEIGHT: bold;FONT-FAMILY: Tahoma;FONT-SIZE: 9pt;COLOR: #000000;TEXT-ALIGN: left;\">Heading2:</Font><Font Style=\"FONT-FAMILY: Tahoma;FONT-SIZE: 9pt;COLOR: #000000;TEXT-ALIGN: left;\"> This is some para2.</Font>"; 
            cm.HtmlNote = workbook.Worksheets[0].Comments[0].HtmlNote; //<<<<<<<<<<<<<<<<<<<<<< 
            cm.IsVisible = true;
            Console.WriteLine(workbook.Worksheets[0].Comments[0].HtmlNote);
            Console.WriteLine(cm.HtmlNote);

            FontSetting fs = cm.Characters(10, 1);
            Assert.IsFalse(fs.Font.IsBold);
            workbook.Save(Constants.destPath + "CellsNet45649.xlsx");
        }
```

### See Also

* class [Font](../../font/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


