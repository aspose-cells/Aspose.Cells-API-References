---
title: "ListColumn.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListColumn. Ottiene e imposta il nome della colonna"
type: docs
url: /it/net/aspose.cells.tables/listcolumn/name/
---
## ListColumn.Name property

Ottiene e imposta il nome della colonna.

```csharp
public string Name { get; set; }
```

### Osservazioni

Se imposta il nome della colonna, il valore della cella corrispondente verrà modificato anche.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Value");
            
            // Crea un oggetto tabella/elenco
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            Aspose.Cells.Tables.ListObject listObject = worksheet.ListObjects[index];

            // Accedi e modifica la proprietà Name della prima colonna dell'elenco
            listObject.ListColumns[0].Name = "NewID";
            
            // Verifica che il nome sia stato impostato
            Console.WriteLine("First column name: " + listObject.ListColumns[0].Name);
            
            // Salva la cartella di lavoro
            workbook.Save("ListColumnPropertyNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


