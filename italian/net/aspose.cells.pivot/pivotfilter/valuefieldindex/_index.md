---
title: "PivotFilter.ValueFieldIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFilter. Ottiene l'indice del campo valore nella regione dei valori"
type: docs
url: /it/net/aspose.cells.pivot/pivotfilter/valuefieldindex/
---
## PivotFilter.ValueFieldIndex property

Restituisce l'indice del campo valore nella regione dei valori.

```csharp
public int ValueFieldIndex { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyValueFieldIndexDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 7;

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity
            
            // Aggiungi filtro di conteggio al campo riga
            PivotField rowField = pivotTable.RowFields[0];
            rowField.FilterTop10(0, PivotFilterType.Count, true, 2);
            
            // Ottieni il filtro e dimostra ValueFieldIndex
            PivotFilter filter = rowField.GetFilters()[0];
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Value Field Index: " + filter.ValueFieldIndex);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFilterValueFieldIndexDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


