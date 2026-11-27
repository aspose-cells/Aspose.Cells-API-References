---
title: "RevisionDefinedName.NewFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionDefinedName‑egenskap. Hämtar formeln"
type: docs
url: /sv/net/aspose.cells.revisions/revisiondefinedname/newformula/
---
## RevisionDefinedName.NewFormula property

Hämtar formeln.

```csharp
public string NewFormula { get; }
```

### Exempel

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
                // Skapa en ny arbetsbok och lägg till lite data
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].Value = "Initial";

                // Lägg till ett definierat namn som pekar på A1
                int nameIdx = workbook.Worksheets.Names.Add("DemoName");
                Name definedName = workbook.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Ändra det definierade namnet för att skapa en revision (pekar nu på B1)
                definedName.RefersTo = "=Sheet1!$B$1";

                // Spara arbetsboken för att bädda in revisionsinformation
                string fileName = "RevisionDefinedName_NewFormulaDemo.xlsx";
                workbook.Save(fileName);

                // Öppna arbetsboken igen för att läsa revisionsloggar
                Workbook revWorkbook = new Workbook(fileName);

                // Iterera genom revisioner och visa NewFormula
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

### Se även

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


