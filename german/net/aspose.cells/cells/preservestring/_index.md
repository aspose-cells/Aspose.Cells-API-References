---
title: "Cells.PreserveString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob alle Arbeitsblattwerte als Zeichenketten erhalten bleiben. Standard ist false"
type: docs
url: /de/net/aspose.cells/cells/preservestring/
---
## Cells.PreserveString property

Liest oder legt einen Wert fest, der angibt, ob alle Arbeitsblattwerte als Zeichenfolgen erhalten bleiben. Standard ist false.

```csharp
public bool PreserveString { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyPreserveStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setzen Sie die PreserveString-Eigenschaft auf true
            cells.PreserveString = true;

            // Zeichenkettenwerte zu Zellen hinzufügen
            cells["A1"].PutValue("Preserved String 1");
            cells["B1"].PutValue("Preserved String 2");

            // Greifen Sie auf die Werte zu (sie werden als Zeichenketten erhalten bleiben)
            Console.WriteLine("Cell A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + cells["B1"].StringValue);

            // Speichere die Arbeitsmappe
            workbook.Save("PreserveStringDemo.xlsx", SaveFormat.Xlsx);

            // Laden Sie die gespeicherte Arbeitsmappe, um die Erhaltung zu überprüfen
            Workbook loadedWorkbook = new Workbook("PreserveStringDemo.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;

            // Geben Sie die erhaltenen Werte aus
            Console.WriteLine("\nAfter loading:");
            Console.WriteLine("Cell A1 value: " + loadedCells["A1"].StringValue);
            Console.WriteLine("Cell B1 value: " + loadedCells["B1"].StringValue);

            // Demonstriere den Vergleich der PreserveString-Eigenschaft
            Console.WriteLine("\nPreserveString property matches: " + 
                (cells.PreserveString == loadedCells.PreserveString));
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


