---
title: "RevisionDefinedName.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionDefinedName-egenskap. Representerar typen av revision"
type: docs
url: /sv/net/aspose.cells.revisions/revisiondefinedname/type/
---
## RevisionDefinedName.Type property

Representerar typen av revision.

```csharp
public override RevisionType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionDefinedNamePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok och lägg till ett definierat namn
                Workbook wb = new Workbook();
                Worksheet ws = wb.Worksheets[0];

                int nameIdx = wb.Worksheets.Names.Add("DemoName");
                Name definedName = wb.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Ändra det definierade namnet för att skapa en revisionspost
                definedName.RefersTo = "=Sheet1!$B$1";

                // Spara arbetsboken för att bädda in revisionsinformation
                string filePath = "RevisionDefinedName_TypeDemo.xlsx";
                wb.Save(filePath);

                // Öppna arbetsboken igen för att läsa revisionsloggen
                Workbook revWb = new Workbook(filePath);

                // Iterera genom revisioner och visa Typen för varje RevisionDefinedName‑post
                foreach (RevisionLog log in revWb.Worksheets.RevisionLogs)
                {
                    foreach (Revision rev in log.Revisions)
                    {
                        if (rev.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName rdn = (RevisionDefinedName)rev;
                            Console.WriteLine($"Revision Type: {rdn.Type}");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


