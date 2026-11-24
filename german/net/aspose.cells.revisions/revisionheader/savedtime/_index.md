---
title: "RevisionHeader.SavedTime"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionHeader-Eigenschaft. Gibt Datum und Uhrzeit zurück und setzt sie, wann dieser Satz von Revisionen gespeichert wurde"
type: docs
url: /de/net/aspose.cells.revisions/revisionheader/savedtime/
---
## RevisionHeader.SavedTime property

Liest und setzt das Datum und die Uhrzeit, wann dieser Satz von Revisionen gespeichert wurde.

```csharp
public DateTime SavedTime { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertySavedTimeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstellen Sie eine RevisionHeader-Instanz
            RevisionHeader revisionHeader = new RevisionHeader();
            
            try
            {
                // Setzen Sie die SavedTime-Eigenschaft
                revisionHeader.SavedTime = DateTime.Now;
                
                // Abrufen und Anzeigen des SavedTime-Werts
                Console.WriteLine("SavedTime value: " + revisionHeader.SavedTime);
                
                // Ändern Sie die SavedTime-Eigenschaft
                revisionHeader.SavedTime = DateTime.Now.AddHours(-1);
                Console.WriteLine("Modified SavedTime value: " + revisionHeader.SavedTime);
                
                // Speichern Sie die Arbeitsmappe, um zu demonstrieren, dass die Eigenschaft verwendet wird
                workbook.Save("SavedTimeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


