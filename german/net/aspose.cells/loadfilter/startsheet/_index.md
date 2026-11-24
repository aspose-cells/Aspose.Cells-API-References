---
title: "LoadFilter.StartSheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadFilter-Methode. Bereitet Filteroptionen vor, bevor das angegebene Arbeitsblatt geladen wird. Die Implementierung von LoadFilter durch den Benutzer kann hier die LoadDataFilterOptions ändern, um festzulegen, wie Daten für dieses Arbeitsblatt geladen werden."
type: docs
url: /de/net/aspose.cells/loadfilter/startsheet/
---
## LoadFilter.StartSheet method

Bereitet die Filteroptionen vor dem Laden des angegebenen Arbeitsblatts vor. Die Implementierung von LoadFilter durch den Benutzer kann hier die LoadDataFilterOptions ändern, um festzulegen, wie Daten für dieses Arbeitsblatt geladen werden.

```csharp
public virtual void StartSheet(Worksheet sheet)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Blatt | Arbeitsblatt | Das zu ladende Arbeitsblatt. Es können hier nur wenige Eigenschaften des angegebenen Arbeitsblatt-Objekts verwendet werden, da die meisten Daten und Eigenschaften noch nicht geladen wurden. Die verfügbaren Eigenschaften sind: Name, Index, VisibilityType |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodStartSheetWithWorksheetDemo
    {
        // Erstelle eine benutzerdefinierte LoadFilter-Klasse, die LoadFilter erweitert
        class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                Console.WriteLine($"Processing sheet: {sheet.Name}");
                // Sie können hier benutzerdefinierte Logik hinzufügen, um bestimmte Tabellenblätter zu verarbeiten
            }
        }

        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "TestSheet";

            // Erstellen Sie eine Instanz unseres benutzerdefinierten Ladefilters
            CustomLoadFilter loadFilter = new CustomLoadFilter();

            try
            {
                // Rufen Sie die StartSheet-Methode mit dem worksheet-Parameter auf
                loadFilter.StartSheet(worksheet);
                
                Console.WriteLine("StartSheet method executed successfully");
                
                // Fügen Sie einige Daten hinzu, um zu demonstrieren, dass das Blatt zugänglich ist
                worksheet.Cells["A1"].PutValue("StartSheet Demo");
                worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("LoadFilterStartSheetDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../worksheet/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


