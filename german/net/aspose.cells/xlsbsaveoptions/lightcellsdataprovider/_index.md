---
title: "XlsbSaveOptions.LightCellsDataProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XlsbSaveOptions-Eigenschaft. Der Datenanbieter zum Speichern der Arbeitsmappe im Light-Modus"
type: docs
url: /de/net/aspose.cells/xlsbsaveoptions/lightcellsdataprovider/
---
## XlsbSaveOptions.LightCellsDataProvider property

Der Datenanbieter zum Speichern der Arbeitsmappe im Light‑Modus.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Beispiele

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
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Beispieldaten einfügen
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Data {i}");
            }

            // Erstellen Sie XLSB-Speicheroptionen
            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            // Speichern Sie die Arbeitsmappe mit LightCellsDataProvider
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Überprüfen Sie die gespeicherten Daten
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
            // Implementieren Sie hier die Logik zur Zelliteration
            return -1; // Return -1 when no more cells
        }

        public int NextRow()
        {
            // Implementieren Sie hier die Logik zur Zeileniteration
            return -1; // Return -1 when no more rows
        }

        public void StartCell(Cell cell)
        {
            // Implementieren Sie hier die Logik zur Zellverarbeitung
        }

        public void StartRow(Row row)
        {
            // Implementieren Sie hier die Logik zur Zeilenverarbeitung
        }

        public bool StartSheet(int sheetIndex)
        {
            // Implementieren Sie hier die Logik zur Blattverarbeitung
            return true; // Return true to process the sheet
        }
    }
}
```

### Siehe auch

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


