---
title: "RevisionRenameSheet.NewName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionRenameSheet-Eigenschaft. Gibt den neuen Namen des Arbeitsblatts zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisionrenamesheet/newname/
---
## RevisionRenameSheet.NewName property

Ermittelt den neuen Namen des Arbeitsblatts.

```csharp
public string NewName { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionRenameSheetPropertyNewNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge ein Arbeitsblatt hinzu und benenne es um, um eine Revision auszulösen
            Worksheet sheet = workbook.Worksheets[0];
            string originalName = sheet.Name;
            string newName = "RenamedSheet";
            sheet.Name = newName;

            // In einen Speicher‑Stream speichern, um Revisionen zu erzeugen
            System.IO.MemoryStream ms = new System.IO.MemoryStream();
            workbook.Save(ms, SaveFormat.Xlsx);

            // Öffnen Sie die Arbeitsmappe erneut, um auf Revisionsprotokolle zuzugreifen
            workbook = new Workbook(ms);
            
            // Prüfen Sie die Revisionsprotokolle für die Umbenennungsoperation
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.RenameSheet)
                    {
                        RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
                        Console.WriteLine("Sheet renamed from '{0}' to '{1}'", 
                            renameSheet.OldName, renameSheet.NewName);
                        
                        // Demonstriere die Verwendung der NewName-Eigenschaft
                        if (renameSheet.NewName == newName)
                        {
                            Console.WriteLine("NewName property verification successful");
                        }
                    }
                }
            }
        }
    }
}
```

### Siehe auch

* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


