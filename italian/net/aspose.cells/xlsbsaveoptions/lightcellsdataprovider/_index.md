---
title: "XlsbSaveOptions.LightCellsDataProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XlsbSaveOptions. Il provider di dati per il salvataggio della cartella di lavoro in modalità leggera"
type: docs
url: /it/net/aspose.cells/xlsbsaveoptions/lightcellsdataprovider/
---
## XlsbSaveOptions.LightCellsDataProvider property

Il provider di dati per salvare la cartella di lavoro in modalità leggera.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola alcuni dati di esempio
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Data {i}");
            }

            // Crea le opzioni di salvataggio XLSB
            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            // Salva la cartella di lavoro con LightCellsDataProvider
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Verifica i dati salvati
                stream.Seek(0, SeekOrigin.Begin);
                Workbook savedWorkbook = new Workbook(stream);
                Console.WriteLine("Workbook saved successfully with LightCellsDataProvider");
            }
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        public bool IsGatherString()
        {
            return true;
        }

        public int NextCell()
        {
            // Implementa qui la logica di iterazione delle celle
            return -1; // Return -1 when no more cells
        }

        public int NextRow()
        {
            // Implementa qui la logica di iterazione delle righe
            return -1; // Return -1 when no more rows
        }

        public void StartCell(Cell cell)
        {
            // Implementa qui la logica di elaborazione delle celle
        }

        public void StartRow(Row row)
        {
            // Implementa qui la logica di elaborazione delle righe
        }

        public bool StartSheet(int sheetIndex)
        {
            // Implementa qui la logica di elaborazione del foglio
            return true; // Return true to process the sheet
        }
    }
}
```

### Vedi anche

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


