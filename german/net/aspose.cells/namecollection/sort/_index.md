---
title: "NameCollection.Sort"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NameCollection-Methode. Sortiert definierte Namen"
type: docs
url: /de/net/aspose.cells/namecollection/sort/
---
## NameCollection.Sort method

Sortiert definierte Namen.

```csharp
public void Sort()
```

### Hinweise

Wenn Sie eine große Anzahl benannter Bereiche in der Excel-Datei erstellen, rufen Sie diese Methode bitte auf, nachdem alle benannten Bereiche erstellt wurden und bevor Sie speichern.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodSortDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hole die NameCollection aus der Arbeitsmappe
            NameCollection names = workbook.Worksheets.Names;
            
            // Füge einige benannte Bereiche hinzu, um die Sortierung zu demonstrieren
            names.Add("RangeC");
            names.Add("RangeA");
            names.Add("RangeB");
            
            try
            {
                // Namen vor dem Sortieren anzeigen
                Console.WriteLine("Names before sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
                
                // Rufen Sie die Sort‑Methode auf
                names.Sort();
                
                // Namen nach dem Sortieren anzeigen
                Console.WriteLine("\nNames after sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Sort method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("NameCollectionSortDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


