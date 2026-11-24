---
title: "NameCollection.Remove"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NameCollection-Methode. Entfernt ein Array von Namen"
type: docs
url: /de/net/aspose.cells/namecollection/remove/
---
## Remove(string[]) {#remove_1}

Entfernt ein Array von Namen.

```csharp
public void Remove(string[] names)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Namen | String[] | Der Text der Namen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodRemoveWithStringArrayDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hole die NameCollection aus der Arbeitsmappe
            NameCollection names = workbook.Worksheets.Names;
            
            // Fügen Sie einige benannte Bereiche hinzu, um die Entfernung zu demonstrieren
            names.Add("TestRange1");
            names.Add("TestRange2");
            names.Add("TestRange3");
            
            // Bereiten Sie das Array der zu entfernenden Namen vor
            string[] namesToRemove = new string[] { "TestRange1", "TestRange3" };

            try
            {
                // Rufen Sie die Remove-Methode mit dem Parameter String[] auf
                names.Remove(namesToRemove);
                
                Console.WriteLine("Names removed successfully:");
                foreach (string name in namesToRemove)
                {
                    Console.WriteLine(name);
                }
                
                // Zeigen Sie die verbleibenden Namen an
                Console.WriteLine("\nRemaining names in the collection:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("NameCollectionRemoveDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove}

Entfernt den Namen.

```csharp
public void Remove(string text)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | String | Der Text des Namens. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie einen benannten Bereich hinzu
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1", "B10");
            range.Name = "TestRange";
            
            // Zeigen Sie die Anzahl vor dem Entfernen an
            Console.WriteLine("Named ranges count before removal: " + workbook.Worksheets.Names.Count);
            
            // Entfernen Sie den benannten Bereich
            workbook.Worksheets.Names.Remove("TestRange");
            
            // Zeigen Sie die Anzahl nach dem Entfernen an
            Console.WriteLine("Named ranges count after removal: " + workbook.Worksheets.Names.Count);
        }
    }
}
```

### Siehe auch

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


