---
title: "ExternalLinkCollection.RemoveAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalLinkCollection-Methode. Entfernt den angegebenen externen Link aus der Arbeitsmappe"
type: docs
url: /de/net/aspose.cells/externallinkcollection/removeat/
---
## RemoveAt(int) {#removeat}

Entfernt den angegebenen externen Link aus der Arbeitsmappe.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | der Index des zu entfernenden externen Links. |

### Hinweise

Beim Entfernen des externen Links werden alle Formeln, die darauf verweisen, ebenfalls entfernt, weil die Verweise ungültig werden.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe mit Beispiel-externen Links
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Beispiel-externen Links hinzu
            worksheet.Cells["A1"].Formula = "='C:/ExternalFiles/File1.xlsx'!Sheet1!A1";
            worksheet.Cells["A2"].Formula = "='C:/ExternalFiles/File2.xlsx'!Sheet1!A1";
            worksheet.Cells["A3"].Formula = "='C:/ImportantFiles/File3.xlsx'!Sheet1!A1";

            // Abrufen der Sammlung externer Links
            ExternalLinkCollection elc = workbook.Worksheets.ExternalLinks;
            Console.WriteLine("Initial external links count: " + elc.Count);

            // Entferne externe Links, die "ImportantFiles" nicht im Pfad enthalten
            for (int i = elc.Count - 1; i >= 0; i--)
            {
                if (!elc[i].DataSource.Contains("ImportantFiles"))
                {
                    elc.RemoveAt(i);
                }
            }

            Console.WriteLine("Remaining external links count: " + elc.Count);
            Console.WriteLine("Remaining external link path: " + elc[0].DataSource);
        }
    }
}
```

### Siehe auch

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, bool) {#removeat_1}

Entfernt den angegebenen externen Link aus der Arbeitsmappe.

```csharp
public void RemoveAt(int index, bool updateReferencesAsLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | der Index des zu entfernenden externen Links. |
| updateReferencesAsLocal | Boolean | Ob alle Verweise des angegebenen externen Links auf den Verweis der aktuellen Arbeitsmappe selbst aktualisiert werden sollen. Siehe [`Clear`](../clear/), um weitere Details zu diesem Parameter zu erhalten. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodRemoveAtWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook wb = new Workbook();
            
            // Füge einige externe Links hinzu
            ExternalLinkCollection elc = wb.Worksheets.ExternalLinks;
            elc.Add("externallink1.xlam", new string[] { "externallink1.xlam" });
            elc.Add("externallink2.xlam", new string[] { "externallink2.xlam" });
            elc.Add("externallink3.xlam", new string[] { "externallink3.xlam" });
            elc.Add("externallink4.xlam", new string[] { "externallink4.xlam" });

            // Füge einige Formeln hinzu, die diese externen Links referenzieren
            Worksheet ws = wb.Worksheets[0];
            for (int i = 0; i < 4; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    ws.Cells[j, i].Formula = $"=externallink{i+1}.xlam!customfunc{j+1}()";
                }
            }

            Console.WriteLine($"Initial external links count: {elc.Count}");
            Console.WriteLine("Formulas before removal:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {ws.Cells[0, i].Formula}");
            }

            // Entfernen bei Index 1 mit updateReferences=true
            elc.RemoveAt(1, true);
            
            Console.WriteLine($"\nAfter removing at index 1 (updateReferences=true):");
            Console.WriteLine($"External links count: {elc.Count}");
            Console.WriteLine("Updated formulas:");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {ws.Cells[0, i].Formula}");
            }

            // Entfernen bei Index 0 mit updateReferences=false
            elc.RemoveAt(0, false);
            
            Console.WriteLine($"\nAfter removing at index 0 (updateReferences=false):");
            Console.WriteLine($"External links count: {elc.Count}");
            Console.WriteLine("Formulas (should be cleared where references were removed):");
            for (int i = 0; i < 2; i++)
            {
                Console.WriteLine($"Cell A{i+1}: Has formula? {ws.Cells[0, i].IsFormula}");
            }
        }
    }
}
```

### Siehe auch

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


