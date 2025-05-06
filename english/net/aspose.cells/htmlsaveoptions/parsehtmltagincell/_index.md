---
title: HtmlSaveOptions.ParseHtmlTagInCell
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether html tagsuch as div/div in cell should be parsed as cell value or preserved as it is. The default value is true
type: docs
url: /net/aspose.cells/htmlsaveoptions/parsehtmltagincell/
---
## HtmlSaveOptions.ParseHtmlTagInCell property

Indicates whether html tag(such as `<div></div>`) in cell should be parsed as cell value or preserved as it is. The default value is true.

```csharp
public bool ParseHtmlTagInCell { get; set; }
```

### Examples

```csharp
// Called: htmlSaveOptions.ParseHtmlTagInCell = true;
public void Property_ParseHtmlTagInCell()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA41603/&quot;;

            String dynamicRange = &quot;&apos;Projects&apos;!B4:E19&quot;;
            String worksheetName = &quot;Projects&quot;;

            Workbook workbook = new Workbook(filePath + &quot;test.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[worksheetName];

            int rangeIndex = workbook.Worksheets.Names.Add(&quot;dummyrange&quot;);
            Name name = workbook.Worksheets.Names[rangeIndex];
            name.RefersTo = dynamicRange;
            name = workbook.Worksheets.Names[rangeIndex];
            Aspose.Cells.Range sourceRange = name.GetRange();

            Workbook newWorkbook = new Workbook(FileFormatType.Xlsx);
            WorksheetCollection targetWsc = newWorkbook.Worksheets;
            Worksheet targetWs = (Worksheet)targetWsc[0];

            Aspose.Cells.Range targetRange = targetWs.Cells.CreateRange(0, 0, sourceRange.RowCount, sourceRange.ColumnCount);

            PasteOptions options = new PasteOptions();

            //Copy column widths
            options.PasteType = PasteType.ColumnWidths;
            targetRange.Copy(sourceRange, options);

            // Copy row heights
            int rowCount = sourceRange.RowCount;
            int firstRow = sourceRange.FirstRow;
            for (int i = 0; i &lt; rowCount; i++)
            {
                double rowHeight = sourceRange.Worksheet.Cells.GetRowHeight(firstRow++);
                targetWs.Cells.SetRowHeight(i, rowHeight);
            }

            //Copy everything else
            options.PasteType = PasteType.All;

            targetRange.Copy(sourceRange, options);

            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;
            htmlSaveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove;
            htmlSaveOptions.ParseHtmlTagInCell = true;

            newWorkbook.Save(Constants.destPath + &quot;JAVA41603.html&quot;, htmlSaveOptions);
            newWorkbook.Save(Constants.destPath + &quot;JAVA41603.xlsx&quot;);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


