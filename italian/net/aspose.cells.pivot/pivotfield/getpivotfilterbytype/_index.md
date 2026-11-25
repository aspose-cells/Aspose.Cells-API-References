---
title: "PivotField.GetPivotFilterByType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Ottiene il filtro pivot del campo pivot per tipo"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/getpivotfilterbytype/
---
## PivotField.GetPivotFilterByType method

Recupera il filtro pivot del campo pivot per tipo

```csharp
public PivotFilter GetPivotFilterByType(PivotFilterType type)
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetPivotFilterByTypeWithPivotFilterTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["A5"].Value = "Apple";
            
            sheet.Cells["B1"].Value = "Count";
            sheet.Cells["B2"].Value = 1;
            sheet.Cells["B3"].Value = 2;
            sheet.Cells["B4"].Value = 3;
            sheet.Cells["B5"].Value = 4;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campo riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Applica filtro di conteggio
            PivotField rowField = pivotTable.RowFields[0];
            rowField.FilterTop10(0, PivotFilterType.Count, true, 2);
            
            // Ottieni il filtro di conteggio
            PivotFilter filter = rowField.GetPivotFilterByType(PivotFilterType.Count);
            
            // Restituisci i dettagli del filtro
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Value Field Index: " + filter.ValueFieldIndex);
            Console.WriteLine("Auto Filter: " + filter.AutoFilter);
            
            wb.Save("PivotFilterExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


