---
title: "XlsSaveOptions.LightCellsDataProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XlsSaveOptions‑egenskap. Dataleverantören för att spara arbetsboken i lättläge"
type: docs
url: /sv/net/aspose.cells/xlssaveoptions/lightcellsdataprovider/
---
## XlsSaveOptions.LightCellsDataProvider property

Dataleverantören för att spara arbetsboken i lättläge.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa XLS‑sparalternativ
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            
            // Ställ in LightCellsDataProvider
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();
            
            // Spara arbetsboken med LightCells-läge
            workbook.Save("output.xls", saveOptions);
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
            return 0; // Only process first cell for demonstration
        }

        public int NextRow()
        {
            return 0; // Only process first row for demonstration
        }

        public void StartCell(Cell cell)
        {
            // Ställ in ett långt strängvärde för att demonstrera LightCells-hantering
            cell.PutValue(new string('X', 257));
        }

        public void StartRow(Row row)
        {
            // Ingen speciell radhantering behövs för den här demonstrationen
        }

        public bool StartSheet(int sheetIndex)
        {
            // Ingen speciell bladhantering behövs för den här demonstrationen
            return false;
        }
    }
}
```

### Se även

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


