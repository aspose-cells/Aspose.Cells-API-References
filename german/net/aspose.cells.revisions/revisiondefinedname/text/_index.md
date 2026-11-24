---
title: "RevisionDefinedName.Text"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionDefinedName-Eigenschaft. Gibt den Text des definierten Namens zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisiondefinedname/text/
---
## RevisionDefinedName.Text property

Liest den Text des definierten Namens.

```csharp
public string Text { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionDefinedNamePropertyTextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Arbeitsblatt hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie einen definierten Namen
            int index = workbook.Worksheets.Names.Add("TestName");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1";
            
            // Ändern Sie den definierten Namen, um eine Revision zu erzeugen
            name.RefersTo = "=Sheet1!$B$1";
            
            // Speichern Sie in einer Datei, um Revisionen zu erzeugen
            workbook.Save("RevisionDefinedName.xlsx");
            
            // Öffnen Sie die Datei erneut, um Revisionen zu lesen
            Workbook revisionWorkbook = new Workbook("RevisionDefinedName.xlsx");
            
            // Überprüfen Sie Revisionen
            foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.DefinedName)
                    {
                        RevisionDefinedName rdn = (RevisionDefinedName)rv;
                        Console.WriteLine("Defined Name Text: " + rdn.Text);
                        Console.WriteLine("Old Formula: " + rdn.OldFormula);
                        Console.WriteLine("New Formula: " + rdn.NewFormula);
                    }
                }
            }
        }
    }
}
```

### Siehe auch

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


