---
title: "ListObject.ShowHeaderRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Ottiene e imposta se questa Tabella mostra la riga di intestazione"
type: docs
url: /it/net/aspose.cells.tables/listobject/showheaderrow/
---
## ListObject.ShowHeaderRow property

Ottiene e imposta se questa Tabella mostra la riga di intestazione.

```csharp
public bool ShowHeaderRow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowHeaderRowDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e un foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Crea un oggetto elenco/tabella
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium2;
            table.ShowHeaderRow = true; // Header row is visible by default

            Console.WriteLine("Header row is visible: " + table.ShowHeaderRow);
            Console.WriteLine("Header cell value: " + worksheet.Cells["A1"].StringValue);

            // Nascondi la riga di intestazione
            table.ShowHeaderRow = false;
            Console.WriteLine("\nAfter setting ShowHeaderRow to false:");
            Console.WriteLine("Header row is visible: " + table.ShowHeaderRow);
            Console.WriteLine("Header cell value: " + worksheet.Cells["A1"].StringValue);

            // Salva la cartella di lavoro
            workbook.Save("ListObjectShowHeaderRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


