---
title: "CustomFilter.FilterOperatorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CustomFilter. Ottiene e imposta il tipo di operatore del filtro"
type: docs
url: /it/net/aspose.cells/customfilter/filteroperatortype/
---
## CustomFilter.FilterOperatorType property

Ottiene e imposta il tipo di operatore del filtro.

```csharp
public FilterOperatorType FilterOperatorType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Mike");
            worksheet.Cells["A5"].PutValue("Emily");

            // Applica filtro automatico
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Applica il filtro personalizzato con l'operatore Contains
            filter.Custom(0, FilterOperatorType.Contains, "e");
            
            // Ottieni il primo filtro personalizzato
            CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];
            
            // Dimostra la proprietà FilterOperatorType
            Console.WriteLine("Initial Filter Operator: " + customFilter.FilterOperatorType);
            Console.WriteLine("Criteria: " + customFilter.Criteria);
            
            // Modifica il tipo di operatore del filtro
            customFilter.FilterOperatorType = FilterOperatorType.EndsWith;
            Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
            
            // Salva la cartella di lavoro
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


