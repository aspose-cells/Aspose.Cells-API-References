---
title: "Protection.AllowSorting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se l'opzione di ordinamento è consentita su un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/allowsorting/
---
## Protection.AllowSorting property

Rappresenta se l'opzione di ordinamento è consentita su un foglio di lavoro protetto.

```csharp
public bool AllowSorting { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSortingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Abilita la protezione del foglio di lavoro
            worksheet.Protect(ProtectionType.All);
            
            // Imposta le proprietà di protezione includendo AllowSorting
            Protection protection = worksheet.Protection;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowEditingContent = false;

            // Restituisci le impostazioni di protezione
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowSorting: {protection.AllowSorting}");
            Console.WriteLine($"AllowFiltering: {protection.AllowFiltering}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Dimostra la capacità di ordinamento
            if (protection.AllowSorting)
            {
                Console.WriteLine("\nSorting is allowed on this protected worksheet");
            }
            else
            {
                Console.WriteLine("\nSorting is not allowed on this protected worksheet");
            }
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


