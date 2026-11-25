---
title: "Workbook.HasCustomFunction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Rileva se è presente una funzione personalizzata utilizzata in questo workbook, ad esempio nelle formule delle celle nei nomi definiti"
type: docs
url: /it/net/aspose.cells/workbook/hascustomfunction/
---
## Workbook.HasCustomFunction property

Rileva se nel workbook è presente una funzione personalizzata, ad esempio nella formula di una cella o nei nomi definiti...

```csharp
public bool HasCustomFunction { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Aggiungi una formula standard a un nome
            NameCollection names = wb.Worksheets.Names;
            int index = names.Add("StandardName");
            names[index].RefersTo = "=SUM(Sheet1!$A$1:$A$2)";
            Console.WriteLine($"Workbook has custom function (should be false): {wb.HasCustomFunction}");

            // Aggiungi una funzione personalizzata a un nome
            index = names.Add("CustomName");
            names[index].RefersTo = "=MYFUNC()";
            Console.WriteLine($"Workbook has custom function (should be true): {wb.HasCustomFunction}");

            // Testa con formule delle celle
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Funzione standard nella cella
            cells["A1"].Formula = "=SUM(B1:B2)";
            Console.WriteLine($"Cell has custom function (should be false): {cells["A1"].HasCustomFunction}");

            // Funzione personalizzata nella cella
            cells["A2"].Formula = "=MYFUNC(B1)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A2"].HasCustomFunction}");

            // Riferimento a un nome con funzione personalizzata
            cells["A3"].Formula = "=CustomName";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A3"].HasCustomFunction}");

            // Funzioni personalizzate combinate
            cells["A4"].Formula = "=MYFUNC(CustomName)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A4"].HasCustomFunction}");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


