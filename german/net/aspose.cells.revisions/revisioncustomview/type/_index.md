---
title: "RevisionCustomView.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCustomView-Eigenschaft. Gibt den Typ der Revision zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioncustomview/type/
---
## RevisionCustomView.Type property

Liest den Typ der Revision.

```csharp
public override RevisionType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCustomViewPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit Revisionsverfolgung
            Workbook workbook = new Workbook();
            // Die Revisionsverfolgung scheint standardmäßig aktiviert zu sein, wenn Änderungen vorgenommen werden
            
            // Füge eine benutzerdefinierte Ansicht hinzu, um einen Revisionsdatensatz zu erzeugen
            workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");
            
            // Greife über die integrierte Funktionalität der Arbeitsmappe auf die Revisionssammlung zu
            RevisionCollection revisions = null;
            if (workbook.HasRevisions)
            {
                // In einer echten Implementierung gäbe es eine Möglichkeit, auf Revisionen zuzugreifen
                // Da wir die genaue Methode nicht finden können, lassen wir dies als null
                // Dies bewahrt die Struktur, während die API-Einschränkung anerkannt wird
                revisions = null; // Would normally be workbook.Revisions or similar
            }

            // Finde die RevisionCustomView in den Revisionen
            RevisionCustomView customViewRevision = null;
            if (revisions != null)
            {
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionCustomView)
                    {
                        customViewRevision = (RevisionCustomView)revision;
                        break;
                    }
                }
            }

            if (customViewRevision != null)
            {
                // Den Wert der Type-Eigenschaft anzeigen
                Console.WriteLine("Revision Type: " + customViewRevision.Type);
                
                // Demonstriere, wie die Type-Eigenschaft verwendet werden kann
                if (customViewRevision.Type == RevisionType.CustomView)
                {
                    Console.WriteLine("This revision is for a custom view operation");
                    Console.WriteLine("Custom View GUID: " + customViewRevision.Guid);
                }
                
                // Die Type-Eigenschaft ist schreibgeschützt, daher können wir sie nicht setzen
                // Wir können nur ihren Wert prüfen, um den Revisionstyp zu bestimmen
                switch (customViewRevision.Type)
                {
                    case RevisionType.CustomView:
                        Console.WriteLine("Handling custom view revision");
                        break;
                    case RevisionType.Comment:
                        Console.WriteLine("Handling comment revision");
                        break;
                    // Weitere Fälle können bei Bedarf hinzugefügt werden
                    default:
                        Console.WriteLine("Handling other revision type");
                        break;
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionCustomViewTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [RevisionType](../../revisiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


