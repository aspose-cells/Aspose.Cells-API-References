---
title: JsonLayoutOptions.TitleStyle
second_title: Aspose.Cells for .NET API Reference
description: JsonLayoutOptions property. Gets and sets the style of the title
type: docs
url: /net/aspose.cells.utility/jsonlayoutoptions/titlestyle/
---
## JsonLayoutOptions.TitleStyle property

Gets and sets the style of the title.

```csharp
public Style TitleStyle { get; set; }
```

### Examples

```csharp
// Called: options.TitleStyle = style;
[Test]
        public void Property_TitleStyle()
        {
            Workbook workbook = new Aspose.Cells.Workbook();
            // Create a Worksheet and assign name
            Worksheet worksheet = workbook.Worksheets[0];
            //worksheet.Name = docMessage.JsonToExcelWorksheetName;

            // Read JSON File or data
            string jsonInput = File.ReadAllText(Constants.sourcePath + &quot;CELLSNET52690.json&quot;);

            // Set Styles
            CellsFactory factory = new CellsFactory();
            Aspose.Cells.Style style = factory.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.Font.Color = System.Drawing.Color.BlueViolet;
            style.Font.IsBold = true;

            // Set JsonLayoutOptions
            JsonLayoutOptions options = new JsonLayoutOptions();

            // I can see a visible difference to the output
            options.ArrayAsTable = true;
            options.IgnoreTitle = true;
            options.TitleStyle = style;

            // I can&apos;t see any difference to the outputted Excel spreadsheet apart from the Date format being set for dates 
            // options.IgnoreObjectTitle = true;
            options.ConvertNumericOrDate = true;
            options.IgnoreNull = true;
            options.DateFormat = &quot;yyyy/MM/dd&quot;;

            //Import JSON Data
            JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);

            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells[&quot;F1&quot;];
            Assert.AreEqual(cell.GetStyle().Custom, &quot;yyyy/MM/dd&quot;);
            Assert.AreEqual(cell.Type, CellValueType.IsDateTime);
            // Save Excel file
            workbook.Save(Constants.destPath + &quot;CELLSNET52690.xlsx&quot;);

        }
```

### See Also

* class [Style](../../../aspose.cells/style/)
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


