---
title: "RevisionDefinedName.NewFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionDefinedName-Eigenschaft. Gibt die Formel zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisiondefinedname/newformula/
---
## RevisionDefinedName.NewFormula property

Liest die Formel.

```csharp
public string NewFormula { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionDefinedNamePropertyNewFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine neue Arbeitsmappe und füge einige Daten hinzu
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].Value = "Initial";

                // Fügen Sie einen definierten Namen hinzu, der auf A1 verweist
                int nameIdx = workbook.Worksheets.Names.Add("DemoName");
                Name definedName = workbook.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Ändern Sie den definierten Namen, um eine Revision zu erzeugen (verweist jetzt auf B1)
                definedName.RefersTo = "=Sheet1!$B$1";

                // Speichern Sie die Arbeitsmappe, um Revisionsinformationen einzubetten
                string fileName = "RevisionDefinedName_NewFormulaDemo.xlsx";
                workbook.Save(fileName);

                // Öffnen Sie die Arbeitsmappe erneut, um Revisionsprotokolle zu lesen
                Workbook revWorkbook = new Workbook(fileName);

                // Iterieren Sie über Revisionen und zeigen Sie NewFormula an
                foreach (RevisionLog log in revWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rev in log.Revisions)
                    {
                        if (rev.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName rdn = (RevisionDefinedName)rev;
                            Console.WriteLine($"Defined Name Text: {rdn.Text}");
                            Console.WriteLine($"Old Formula: {rdn.OldFormula}");
                            Console.WriteLine($"New Formula: {rdn.NewFormula}");
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


