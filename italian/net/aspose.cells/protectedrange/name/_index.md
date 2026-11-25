---
title: "ProtectedRange.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ProtectedRange. Ottiene il titolo dell'intervallo. Questo è usato come descrittore, non come definizione di intervallo denominato"
type: docs
url: /it/net/aspose.cells/protectedrange/name/
---
## ProtectedRange.Name property

Ottiene il titolo dell'intervallo. Questo è usato come descrizione, non come definizione di intervallo nominato.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea la collezione di intervalli protetti
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Aggiungi un intervallo protetto con nome "MyRange"
            int index = allowRanges.Add("MyRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];
            protectedRange.Password = "123";

            // Accedi e visualizza la proprietà Name
            Console.WriteLine("Protected range name: " + protectedRange.Name);
            Console.WriteLine("Cell area: {0},{1} to {2},{3}", 
                protectedRange.CellArea.StartRow,
                protectedRange.CellArea.StartColumn,
                protectedRange.CellArea.EndRow,
                protectedRange.CellArea.EndColumn);

            // Aggiungi un altro intervallo denominato
            index = allowRanges.Add("SecondRange", 3, 3, 5, 5);
            ProtectedRange secondRange = allowRanges[index];
            Console.WriteLine("Second protected range name: " + secondRange.Name);

            // Salva la cartella di lavoro
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


