---
title: "Klass RevisionDefinedName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionDefinedName klass. Representerar en revisionspost för en ändring av ett definierat namn"
type: docs
url: /sv/net/aspose.cells.revisions/revisiondefinedname/
---
## RevisionDefinedName class

Representerar en revisionspost för en ändring av ett definierat namn.

```csharp
public class RevisionDefinedName : Revision
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Hämtar numret för denna revision.(Arv från [`Revision`](../revision/).) |
| [NewFormula](../../aspose.cells.revisions/revisiondefinedname/newformula/) { get; } | Hämtar formeln. |
| [OldFormula](../../aspose.cells.revisions/revisiondefinedname/oldformula/) { get; } | Hämtar den gamla formeln. |
| [Text](../../aspose.cells.revisions/revisiondefinedname/text/) { get; } | Hämtar texten för det definierade namnet. |
| override [Type](../../aspose.cells.revisions/revisiondefinedname/type/) { get; } | Representerar typen av revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Hämtar kalkylbladet.(Arv från [`Revision`](../revision/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDefinedNameDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till ett definierat namn i arbetsboken
                int nameIndex = workbook.Worksheets.Names.Add("TestDefinedName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Ändra det definierade namnet för att skapa en revision
                definedName.RefersTo = "=Sheet1!$B$1";

                // Spara arbetsboken för att generera revisionsloggar
                string filePath = "RevisionDefinedNameDemo.xlsx";
                workbook.Save(filePath);

                // Öppna arbetsboken igen för att komma åt revisionsinformation
                Workbook revisionWorkbook = new Workbook(filePath);

                // Iterera genom revisionsloggar för att hitta RevisionDefinedName-poster
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;

                            // Visa egenskaperna för RevisionDefinedName
                            Console.WriteLine($"Revision Type: {revisionDefinedName.Type}");
                            Console.WriteLine($"Defined Name Text: {revisionDefinedName.Text}");
                            Console.WriteLine($"Old Formula: {revisionDefinedName.OldFormula}");
                            Console.WriteLine($"New Formula: {revisionDefinedName.NewFormula}");
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


