---
title: "Klass RevisionRenameSheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionRenameSheet klass. Representerar en revision av att byta namn på bladet"
type: docs
url: /sv/net/aspose.cells.revisions/revisionrenamesheet/
---
## RevisionRenameSheet class

Representerar en revision av att byta namn på blad.

```csharp
public class RevisionRenameSheet : Revision
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Hämtar numret för denna revision.(Arv från [`Revision`](../revision/).) |
| [NewName](../../aspose.cells.revisions/revisionrenamesheet/newname/) { get; } | Hämtar det nya namnet på arbetsbladet. |
| [OldName](../../aspose.cells.revisions/revisionrenamesheet/oldname/) { get; } | Hämtar det gamla namnet på arbetsbladet. |
| override [Type](../../aspose.cells.revisions/revisionrenamesheet/type/) { get; } | Representerar typen av revisionen. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Hämtar kalkylbladet.(Arv från [`Revision`](../revision/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionRenameSheetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Spara originalnamnet och byt namn på bladet
                string originalName = worksheet.Name;
                worksheet.Name = "RenamedSheet";

                // Spara till minnesström för att generera revisioner
                System.IO.MemoryStream ms = new System.IO.MemoryStream();
                workbook.Save(ms, SaveFormat.Xlsx);

                // Öppna arbetsboken igen för att komma åt revisionsloggar
                workbook = new Workbook(ms);

                // Kontrollera revisionsloggar för namnbytesoperation
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rv in log.Revisions)
                    {
                        if (rv.Type == RevisionType.RenameSheet)
                        {
                            RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
                            Console.WriteLine("Revision Type: " + renameSheet.Type);
                            Console.WriteLine("Old Sheet Name: " + renameSheet.OldName);
                            Console.WriteLine("New Sheet Name: " + renameSheet.NewName);
                        }
                    }
                }

                // Spara arbetsboken
                workbook.Save("RevisionRenameSheetDemo.xlsx");
                Console.WriteLine("RevisionRenameSheet demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RevisionRenameSheet demo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


