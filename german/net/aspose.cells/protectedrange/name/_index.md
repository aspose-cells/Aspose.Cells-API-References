---
title: "ProtectedRange.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ProtectedRange-Eigenschaft. Gibt den Titel des Bereichs zurück. Dies wird als Beschreiber verwendet, nicht als benannte Bereichsdefinition"
type: docs
url: /de/net/aspose.cells/protectedrange/name/
---
## ProtectedRange.Name property

Ruft den Titel des Bereichs ab. Dieser wird als Bezeichner verwendet, nicht als Definition eines benannten Bereichs.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ProtectedRange-Sammlung erstellen
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Füge einen geschützten Bereich mit dem Namen "MyRange" hinzu
            int index = allowRanges.Add("MyRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];
            protectedRange.Password = "123";

            // Zugreifen und die Name-Eigenschaft anzeigen
            Console.WriteLine("Protected range name: " + protectedRange.Name);
            Console.WriteLine("Cell area: {0},{1} to {2},{3}", 
                protectedRange.CellArea.StartRow,
                protectedRange.CellArea.StartColumn,
                protectedRange.CellArea.EndRow,
                protectedRange.CellArea.EndColumn);

            // Einen weiteren benannten Bereich hinzufügen
            index = allowRanges.Add("SecondRange", 3, 3, 5, 5);
            ProtectedRange secondRange = allowRanges[index];
            Console.WriteLine("Second protected range name: " + secondRange.Name);

            // Speichere die Arbeitsmappe
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


