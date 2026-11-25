---
title: "Range.CurrentRegion"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Restituisce un oggetto Range che rappresenta la regione corrente. La regione corrente è un intervallo delimitato da qualsiasi combinazione di righe vuote e colonne vuote"
type: docs
url: /it/net/aspose.cells/range/currentregion/
---
## Range.CurrentRegion property

Restituisce un oggetto Range che rappresenta la regione corrente. La regione corrente è un intervallo delimitato da qualsiasi combinazione di righe vuote e colonne vuote.

```csharp
public Range CurrentRegion { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyCurrentRegionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola i dati con alcune celle vuote per creare regioni
            worksheet.Cells["A1"].PutValue("Region 1");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["A4"].PutValue("Data 3");
            
            // Lascia la riga 5 vuota per separare le regioni
            
            worksheet.Cells["A6"].PutValue("Region 2");
            worksheet.Cells["A7"].PutValue("Data 4");
            worksheet.Cells["B7"].PutValue("Data 5");
            worksheet.Cells["A8"].PutValue("Data 6");

            // Ottieni una cella nella prima regione e converti in Range
            Aspose.Cells.Range cellInRegion1 = worksheet.Cells.CreateRange("A2", "A2");
            Aspose.Cells.Range currentRegion1 = cellInRegion1.CurrentRegion;
            
            Console.WriteLine("CurrentRegion for A2: " + currentRegion1.Address);
            Console.WriteLine("Row count in region: " + currentRegion1.RowCount);
            Console.WriteLine("Column count in region: " + currentRegion1.ColumnCount);

            // Ottieni una cella nella seconda regione e converti in Range
            Aspose.Cells.Range cellInRegion2 = worksheet.Cells.CreateRange("B7", "B7");
            Aspose.Cells.Range currentRegion2 = cellInRegion2.CurrentRegion;
            
            Console.WriteLine("\nCurrentRegion for B7: " + currentRegion2.Address);
            Console.WriteLine("Row count in region: " + currentRegion2.RowCount);
            Console.WriteLine("Column count in region: " + currentRegion2.ColumnCount);

            // Applica la formattazione all'intera regione corrente
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            currentRegion1.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("RangePropertyCurrentRegionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


