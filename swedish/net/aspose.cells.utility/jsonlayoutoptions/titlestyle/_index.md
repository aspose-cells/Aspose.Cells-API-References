---
title: "JsonLayoutOptions.TitleStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonLayoutOptions-egenskap. Hämtar och anger stilen för titeln"
type: docs
url: /sv/net/aspose.cells.utility/jsonlayoutoptions/titlestyle/
---
## JsonLayoutOptions.TitleStyle property

Hämtar och sätter stilen för titeln.

```csharp
public Style TitleStyle { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyTitleStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempel på JSON‑data
            string jsonInput = @"
            {
                ""Name"": ""John"",
                ""Age"": 30,
                ""JoinDate"": ""2023-05-15""
            }";

            // Skapa anpassad stil för titlar
            CellsFactory factory = new CellsFactory();
            Style titleStyle = factory.CreateStyle();
            titleStyle.HorizontalAlignment = TextAlignmentType.Center;
            titleStyle.Font.Color = System.Drawing.Color.BlueViolet;
            titleStyle.Font.IsBold = true;

            // Konfigurera alternativ för JSON-import
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.TitleStyle = titleStyle;
            options.ConvertNumericOrDate = true;
            options.DateFormat = "yyyy-MM-dd";

            // Importera JSON-data med anpassad titelstil
            JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);

            // Autoanpassa kolumner för bättre synlighet
            worksheet.AutoFitColumns();

            // Spara arbetsboken
            workbook.Save("JsonWithStyledTitles.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../../aspose.cells/style/)
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


