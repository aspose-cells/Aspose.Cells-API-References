---
title: XlsSaveOptions.MatchColor
second_title: Aspose.Cells for .NET API Reference
description: XlsSaveOptions property. Indicates whether matching font color because there are 56 colors in the standard color palette
type: docs
url: /net/aspose.cells/xlssaveoptions/matchcolor/
---
## XlsSaveOptions.MatchColor property

Indicates whether matching font color because there are 56 colors in the standard color palette.

```csharp
public bool MatchColor { get; set; }
```

### Examples

```csharp
// Called: saveOptions.MatchColor = true;
[Test]
        public void Property_MatchColor()
        {
            //}
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsJava43110.xls&quot;);
            Cell cellB2 = workbook.Worksheets[0].Cells[1, 1];

            // getting the B2 cell FontSetting object
            FontSetting B2_fontSetting = cellB2.Characters(0, 5);

            // original cell text RGB values in byte primitive data type
            byte redColorByte = B2_fontSetting.Font.Color.R;
            byte greenColorByte = B2_fontSetting.Font.Color.G;
            byte blueColorByte = B2_fontSetting.Font.Color.B;

            // original cell text RGB values converted to int primitive data type
            int redColorInt = redColorByte &amp; 0xFF;
            int greenColorInt = greenColorByte &amp; 0xFF;
            int blueColorInt = blueColorByte &amp; 0xFF;

            // assert statements that confirm the RGB values of the cell text color
            //assertEquals(7, redColorInt);
            //assertEquals(12, greenColorInt);
            //assertEquals(255, blueColorInt);


            // making some changes over cell B2
            //  B2_fontSetting.Font.IsBold = (false);
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MatchColor = true;
            workbook.Save(Constants.destPath + &quot;CellsJava43110.xls&quot;, saveOptions);
            workbook = new Workbook(Constants.destPath + &quot;CellsJava43110.xls&quot;);
            cellB2 = workbook.Worksheets[0].Cells[1, 1];

            // getting the B2 cell FontSetting object
            B2_fontSetting = cellB2.Characters(0, 5);
           AssertHelper.AreEqual(Color.Blue, B2_fontSetting.Font.Color);
        }
```

### See Also

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


