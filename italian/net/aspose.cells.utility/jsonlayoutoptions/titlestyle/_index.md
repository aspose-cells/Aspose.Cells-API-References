---
title: "JsonLayoutOptions.TitleStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonLayoutOptions. Ottiene e imposta lo stile del titolo"
type: docs
url: /it/net/aspose.cells.utility/jsonlayoutoptions/titlestyle/
---
## JsonLayoutOptions.TitleStyle property

Ottiene e imposta lo stile del titolo.

```csharp
public Style TitleStyle { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati JSON di esempio
            string jsonInput = @"
            {
                ""Name"": ""John"",
                ""Age"": 30,
                ""JoinDate"": ""2023-05-15""
            }";

            // Crea stile personalizzato per i titoli
            CellsFactory factory = new CellsFactory();
            Style titleStyle = factory.CreateStyle();
            titleStyle.HorizontalAlignment = TextAlignmentType.Center;
            titleStyle.Font.Color = System.Drawing.Color.BlueViolet;
            titleStyle.Font.IsBold = true;

            // Configura le opzioni di importazione JSON
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.TitleStyle = titleStyle;
            options.ConvertNumericOrDate = true;
            options.DateFormat = "yyyy-MM-dd";

            // Importa dati JSON con stile del titolo personalizzato
            JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);

            // Adatta automaticamente le colonne per una migliore visibilità
            worksheet.AutoFitColumns();

            // Salva la cartella di lavoro
            workbook.Save("JsonWithStyledTitles.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../../aspose.cells/style/)
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


