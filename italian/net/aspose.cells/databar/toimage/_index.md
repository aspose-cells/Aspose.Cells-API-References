---
title: "DataBar.ToImage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DataBar. Renderizza la barra dei dati nella cella in un array di byte immagine"
type: docs
url: /it/net/aspose.cells/databar/toimage/
---
## DataBar.ToImage method

Renderizza la DataBar nella cella in un array di byte dell'immagine.

```csharp
public byte[] ToImage(Cell cell, ImageOrPrintOptions imgOpts)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cella | Cella | Indica la barra dei dati nella cella da renderizzare |
| imgOpts | ImageOrPrintOptions | ImageOrPrintOptions contiene alcune proprietà dell'immagine di output |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class DataBarMethodToImageWithCellImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e formattazione condizionale
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            
            // Aggiungi formattazione condizionale della barra dati
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);
            
            idx = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcc[idx];
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            
            // Ottieni la cella con formattazione condizionale
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            
            if (result != null && result.ConditionalFormattingDataBar != null)
            {
                DataBar bar = result.ConditionalFormattingDataBar;
                ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
                
                // Converti la barra dei dati in immagine
                byte[] img = bar.ToImage(cell, imgOpts);
                
                // Salva l'immagine
                string outputPath = "DataBarImage.png";
                File.WriteAllBytes(outputPath, img);
                
                // Per la verifica dell'immagine, è necessario aggiungere il pacchetto System.Drawing.Common
                // e utilizzare System.Drawing.Image se necessario
                Console.WriteLine($"Data bar image saved to {outputPath}");
            }
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


