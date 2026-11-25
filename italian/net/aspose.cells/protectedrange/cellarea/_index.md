---
title: "ProtectedRange.CellArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ProtectedRange. Ottiene l'oggetto CellArea che rappresenta l'area di celle da proteggere"
type: docs
url: /it/net/aspose.cells/protectedrange/cellarea/
---
## ProtectedRange.CellArea property

Ottiene l'oggetto `CellArea` che rappresenta l'area di celle da proteggere.

```csharp
public CellArea CellArea { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyCellAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea intervalli protetti
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;
            
            // Aggiungi il primo intervallo protetto
            int index1 = allowRanges.Add("Range1", 0, 0, 2, 2);
            ProtectedRange range1 = allowRanges[index1];
            range1.Password = "123";

            // Aggiungi il secondo intervallo protetto
            int index2 = allowRanges.Add("Range2", 3, 3, 5, 5);
            ProtectedRange range2 = allowRanges[index2];
            range2.Password = "456";

            // Visualizza le informazioni di CellArea per entrambi gli intervalli
            Console.WriteLine("Protected Range 1:");
            Console.WriteLine($"Name: {range1.Name}");
            Console.WriteLine($"Area: {range1.CellArea.StartRow},{range1.CellArea.StartColumn} to {range1.CellArea.EndRow},{range1.CellArea.EndColumn}");

            Console.WriteLine("\nProtected Range 2:");
            Console.WriteLine($"Name: {range2.Name}");
            Console.WriteLine($"Area: {range2.CellArea.StartRow},{range2.CellArea.StartColumn} to {range2.CellArea.EndRow},{range2.CellArea.EndColumn}");

            // Salva la cartella di lavoro
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


