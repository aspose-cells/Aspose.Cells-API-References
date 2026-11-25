---
title: "ListObject.AutoFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Ottiene il filtro automatico di questa tabella"
type: docs
url: /it/net/aspose.cells.tables/listobject/autofilter/
---
## ListObject.AutoFilter property

Ottiene il filtro automatico di questa tabella.

```csharp
public AutoFilter AutoFilter { get; }
```

### Osservazioni

Funziona solo quando [`HasAutoFilter`](../hasautofilter/) è false.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Mary");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Peter");
            worksheet.Cells["B4"].PutValue(35);

            // Crea un ListObject
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Ridimensiona l'oggetto elenco per includere tutti i dati
            listObject.Resize(0, 0, 4, 2, true);

            // Accedi e dimostra la funzionalità AutoFilter
            if (listObject.AutoFilter != null)
            {
                // Applica il filtro sulla colonna Età (colonna 2)
                listObject.AutoFilter.Filter(1, "25");
                
                // Mostra i dati filtrati
                Console.WriteLine("Filtered Data:");
                for (int row = 1; row <= 4; row++)
                {
                    if (!worksheet.Cells.Rows[row].IsHidden)
                    {
                        Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                    }
                }

                // Cancella il filtro
                listObject.AutoFilter.RemoveFilter(1);
            }

            // Salva la cartella di lavoro
            workbook.Save("ListObjectAutoFilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


