---
title: "AutoFilter.FilterColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoFilter. Ottiene la collezione delle colonne di filtro"
type: docs
url: /it/net/aspose.cells/autofilter/filtercolumns/
---
## AutoFilter.FilterColumns property

Ottiene la raccolta delle colonne filtro.

```csharp
public FilterColumnCollection FilterColumns { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyFilterColumnsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Status");
            
            worksheet.Cells["A2"].PutValue("HR");
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["C2"].PutValue("Present");
            
            worksheet.Cells["A3"].PutValue("IT");
            worksheet.Cells["B3"].PutValue("Sarah");
            worksheet.Cells["C3"].PutValue("Absent");
            
            worksheet.Cells["A4"].PutValue("HR");
            worksheet.Cells["B4"].PutValue("Mike");
            worksheet.Cells["C4"].PutValue("Present");

            // Applica filtro automatico
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:C1";
            
            // Filtra la colonna 2 (Status) per i valori "Present"
            autoFilter.Filter(2, "Present");
            
            // Accedi alla colonna di filtro
            FilterColumn filterColumn = autoFilter.FilterColumns[2];
            
            // Salva la cartella di lavoro
            workbook.Save("AutoFilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [FilterColumnCollection](../../filtercolumncollection/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


