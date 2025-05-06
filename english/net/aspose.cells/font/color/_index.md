---
title: Font.Color
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets the Color of the font
type: docs
url: /net/aspose.cells/font/color/
---
## Font.Color property

Gets or sets the Color of the font.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(targetRange[0, 0].GetStyle().Font.Color, System.Drawing.Color.Black);
[Test]
        public void Property_Color()
        {
            String dynamicRange = &quot;&apos;Daily Schedule&apos;!B4:C36&quot;;
            String worksheetName = &quot;Daily Schedule&quot;;
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA41697.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[worksheetName];
            //workbook.calculateFormula(); 
            int rangeIndex = workbook.Worksheets.Names.Add(&quot;dummyrange&quot;);
            Name name = workbook.Worksheets.Names[rangeIndex];
            name.RefersTo = (dynamicRange);
            name = workbook.Worksheets.Names[rangeIndex];
            Aspose.Cells.Range sourceRange = name.GetRange();

            Workbook newWorkbook = new Workbook(FileFormatType.Xlsx);
            WorksheetCollection targetWsc = newWorkbook.Worksheets;
            Worksheet targetWs = (Worksheet)targetWsc[0];

            Aspose.Cells.Range targetRange = targetWs.Cells.CreateRange(0, 0, sourceRange.RowCount, sourceRange.ColumnCount);

            PasteOptions options = new PasteOptions();
            //Copy everything else 
            options.PasteType = (PasteType.All);

            targetRange.Copy(sourceRange, options);
            AssertHelper.AreEqual(targetRange[0, 0].GetStyle().Font.Color, System.Drawing.Color.Black);
            Util.ReSave(newWorkbook, SaveFormat.Xlsx);
            Util.SaveAsBuffer(newWorkbook, SaveFormat.Pdf);
            //newWorkbook.Save(Constants.destPath + &quot;CELLSJAVA41697.xlsx&quot;);
            //newWorkbook.Save(Constants.destPath + &quot;CELLSJAVA41697.pdf&quot;);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


