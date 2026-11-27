---
title: "XlsbSaveOptions.LightCellsDataProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XlsbSaveOptions-egenskap. Dataleverantören för att spara arbetsbok i lättläge"
type: docs
url: /sv/net/aspose.cells/xlsbsaveoptions/lightcellsdataprovider/
---
## XlsbSaveOptions.LightCellsDataProvider property

Dataleverantören för att spara arbetsboken i lättläge.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Exempel

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
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i lite exempeldata
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Data {i}");
            }

            // Skapa XLSB-sparalternativ
            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            // Spara arbetsboken med LightCellsDataProvider
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Verifiera den sparade datan
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
            // Implementera cellitereringslogik här
            return -1; // Return -1 when no more cells
        }

        public int NextRow()
        {
            // Implementera raditereringslogik här
            return -1; // Return -1 when no more rows
        }

        public void StartCell(Cell cell)
        {
            // Implementera cellbearbetningslogik här
        }

        public void StartRow(Row row)
        {
            // Implementera radbearbetningslogik här
        }

        public bool StartSheet(int sheetIndex)
        {
            // Implementera bladbearbetningslogik här
            return true; // Return true to process the sheet
        }
    }
}
```

### Se även

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


