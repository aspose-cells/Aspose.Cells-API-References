---
title: "FindOptions.SearchNext"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FindOptions. Ordine di ricerca. True per cercare il successivo. False per cercare il precedente"
type: docs
url: /it/net/aspose.cells/findoptions/searchnext/
---
## FindOptions.SearchNext property

Ordine di ricerca. True: cerca il successivo. False: cerca il precedente.

```csharp
[Obsolete("Use FindOptions.SearchBackward property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SearchNext { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà FindOptions.SearchBackward. Questa proprietà sarà rimossa 12 mesi dopo, a partire da novembre 2018. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertySearchNextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("apple");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("apple pie");

            // Crea opzioni di ricerca
            FindOptions findOptions = new FindOptions();
            findOptions.CaseSensitive = false;
            findOptions.LookAtType = LookAtType.Contains;

            // Dimostra la proprietà SearchNext (obsoleta, ma mostrata a scopo dimostrativo)
            Console.WriteLine("Initial SearchNext value: " + findOptions.SearchNext);
            
            // Cerca in avanti (comportamento predefinito)
            findOptions.SearchNext = true;
            Cell firstForward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First forward search result: " + (firstForward != null ? firstForward.Name + " - " + firstForward.StringValue : "Not found"));

            // Cerca all'indietro
            findOptions.SearchNext = false;
            Cell firstBackward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First backward search result: " + (firstBackward != null ? firstBackward.Name + " - " + firstBackward.StringValue : "Not found"));

            // Salva la cartella di lavoro
            workbook.Save("PropertySearchNextDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


