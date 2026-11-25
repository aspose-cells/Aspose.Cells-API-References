---
title: "AbstractTextLoadOptions.LoadStyleStrategy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractTextLoadOptions. Indica la strategia da applicare allo stile per i valori analizzati quando si converte una stringa in numero o data/ora"
type: docs
url: /it/net/aspose.cells/abstracttextloadoptions/loadstylestrategy/
---
## AbstractTextLoadOptions.LoadStyleStrategy property

Indica la strategia da applicare allo stile per i valori analizzati quando si converte una stringa in numero o data/ora.

```csharp
public TxtLoadStyleStrategy LoadStyleStrategy { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyLoadStyleStrategyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta uno stile personalizzato per la dimostrazione
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.Name = "Arial";
            customStyle.Font.Size = 12;
            customStyle.Font.Color = System.Drawing.Color.Blue;
            customStyle.Pattern = BackgroundType.Solid;
            customStyle.ForegroundColor = System.Drawing.Color.LightYellow;

            // Applica lo stile a una cella
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");
            cell.SetStyle(customStyle);

            // Crea dati CSV
            string csvData = "Data1,Data2\nValue1,Value2";
            byte[] byteArray = Encoding.ASCII.GetBytes(csvData);
            MemoryStream stream = new MemoryStream(byteArray);

            // Crea opzioni di caricamento testo con LoadStyleStrategy
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn
            };

            // Importa i dati CSV con le opzioni di caricamento specificate
            cells.ImportCSV(stream, loadOptions, 0, 0);

            // Salvare la cartella di lavoro per dimostrare il risultato
            workbook.Save("LoadStyleStrategyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* enum [TxtLoadStyleStrategy](../../txtloadstylestrategy/)
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


