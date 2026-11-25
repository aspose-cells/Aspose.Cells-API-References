---
title: "PivotFilter.GetDateTimeValues"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotFilter. Ottiene i valori del filtro numerico"
type: docs
url: /it/net/aspose.cells.pivot/pivotfilter/getdatetimevalues/
---
## PivotFilter.GetDateTimeValues method

Restituisce i valori del filtro numerico.

```csharp
public DateTime[] GetDateTimeValues()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetDateTimeValuesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Date";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = DateTime.Now;
            cells["B2"].Value = 1000;
            cells["A3"].Value = DateTime.Now.AddDays(1);
            cells["B3"].Value = 2000;
            cells["A4"].Value = DateTime.Now.AddDays(2);
            cells["B4"].Value = 3000;

            // Crea tabella pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Aggiungi campo riga e applica filtro data
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.BaseFields[0].FilterByDate(PivotFilterType.DateBetween, DateTime.Now, DateTime.Now.AddDays(1));
            
            // Ottieni il filtro e dimostra GetDateTimeValues
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            DateTime[] dateValues = filter.GetDateTimeValues();
            
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("First Date Value: " + dateValues[0]);
            Console.WriteLine("Second Date Value: " + dateValues[1]);
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


