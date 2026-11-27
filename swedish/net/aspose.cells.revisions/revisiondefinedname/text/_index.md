---
title: "RevisionDefinedName.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionDefinedName‑egenskap. Hämtar texten för det definierade namnet"
type: docs
url: /sv/net/aspose.cells.revisions/revisiondefinedname/text/
---
## RevisionDefinedName.Text property

Hämtar texten för det definierade namnet.

```csharp
public string Text { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett definierat namn
            int index = workbook.Worksheets.Names.Add("TestName");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1";
            
            // Ändra det definierade namnet för att skapa en revision
            name.RefersTo = "=Sheet1!$B$1";
            
            // Spara till fil för att generera revisioner
            workbook.Save("RevisionDefinedName.xlsx");
            
            // Öppna filen igen för att läsa revisioner
            Workbook revisionWorkbook = new Workbook("RevisionDefinedName.xlsx");
            
            // Kontrollera revisioner
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

### Se även

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


