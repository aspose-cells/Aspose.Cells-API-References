---
title: "RevisionDefinedName.OldFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionDefinedName‑Eigenschaft. Gibt die alte Formel zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisiondefinedname/oldformula/
---
## RevisionDefinedName.OldFormula property

Liest die alte Formel.

```csharp
public string OldFormula { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionDefinedNamePropertyOldFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Fügen Sie einen definierten Namen hinzu, um die Revisionshistorie zu erzeugen
                int nameIndex = workbook.Worksheets.Names.Add("SampleName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Ändere den definierten Namen, um eine Revision zu erstellen
                definedName.RefersTo = "=Sheet1!$B$1";

                // Speichern Sie die Arbeitsmappe, um die Revisionen zu erhalten
                string filePath = "OldFormulaDemo.xlsx";
                workbook.Save(filePath);

                // Öffnen Sie die Arbeitsmappe erneut, um auf Revisionsprotokolle zuzugreifen
                Workbook revisionWorkbook = new Workbook(filePath);

                // Durchlaufen Sie die Revisionsprotokolle, um Revisionen definierter Namen zu finden
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;
                            Console.WriteLine("Defined Name Text: " + revisionDefinedName.Text);
                            Console.WriteLine("Old Formula: " + revisionDefinedName.OldFormula);
                            Console.WriteLine("New Formula: " + revisionDefinedName.NewFormula);
                        }
                    }
                }
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

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


