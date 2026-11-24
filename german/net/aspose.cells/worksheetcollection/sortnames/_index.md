---
title: "WorksheetCollection.SortNames"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Sortiert die definierten Namen"
type: docs
url: /de/net/aspose.cells/worksheetcollection/sortnames/
---
## WorksheetCollection.SortNames method

Sortiert die definierten Namen.

```csharp
public void SortNames()
```

### Hinweise

Wenn Sie eine große Anzahl benannter Bereiche in der Excel-Datei erstellen, rufen Sie diese Methode bitte auf, nachdem alle benannten Bereiche erstellt wurden und bevor Sie speichern.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSortNamesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Einige benannte Bereiche hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test1");
            worksheet.Cells.CreateRange("A1").Name = "Range2";
            worksheet.Cells["B1"].PutValue("Test2");
            worksheet.Cells.CreateRange("B1").Name = "Range1";
            
            // Namen vor dem Sortieren anzeigen
            Console.WriteLine("Before sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Namen sortieren
            workbook.Worksheets.SortNames();
            
            // Namen nach dem Sortieren anzeigen
            Console.WriteLine("\nAfter sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


