---
title: "CustomFilter.Criteria"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CustomFilter. Ottiene e imposta i criteri"
type: docs
url: /it/net/aspose.cells/customfilter/criteria/
---
## CustomFilter.Criteria property

Ottiene e imposta i criteri.

```csharp
public object Criteria { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Numbers");
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(5);
            worksheet.Cells["A5"].PutValue(9);
            worksheet.Cells["A6"].PutValue(3);

            // Applica filtro automatico
            worksheet.AutoFilter.Range = "A1:A6";
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Aggiungi filtro personalizzato
            int fieldIndex = 0;
            autoFilter.Custom(fieldIndex, FilterOperatorType.GreaterOrEqual, 5);
            
            // Ottieni la colonna del filtro e mostra i criteri
            FilterColumn fc = autoFilter.FilterColumns[fieldIndex];
            CustomFilter cf = ((CustomFilterCollection)fc.Filter)[0];
            Console.WriteLine("Filter Criteria: " + cf.Criteria);
            
            // Aggiorna il filtro
            autoFilter.Refresh();
            
            // Salva la cartella di lavoro
            workbook.Save("CustomFilterExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


