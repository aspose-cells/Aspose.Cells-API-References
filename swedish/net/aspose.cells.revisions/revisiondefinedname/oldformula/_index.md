---
title: "RevisionDefinedName.OldFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionDefinedName-egenskap. Hämtar den gamla formeln"
type: docs
url: /sv/net/aspose.cells.revisions/revisiondefinedname/oldformula/
---
## RevisionDefinedName.OldFormula property

Hämtar den gamla formeln.

```csharp
public string OldFormula { get; }
```

### Exempel

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
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till ett definierat namn för att skapa revisionshistorik
                int nameIndex = workbook.Worksheets.Names.Add("SampleName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Ändra det definierade namnet för att skapa en revision
                definedName.RefersTo = "=Sheet1!$B$1";

                // Spara arbetsboken för att bevara revisioner
                string filePath = "OldFormulaDemo.xlsx";
                workbook.Save(filePath);

                // Öppna arbetsboken igen för att komma åt revisionsloggar
                Workbook revisionWorkbook = new Workbook(filePath);

                // Iterera genom revisionsloggar för att hitta revisioner av definierade namn
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

### Se även

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


