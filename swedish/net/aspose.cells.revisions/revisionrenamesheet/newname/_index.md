---
title: "RevisionRenameSheet.NewName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionRenameSheet-egenskapen. Hämtar det nya namnet på kalkylbladet"
type: docs
url: /sv/net/aspose.cells.revisions/revisionrenamesheet/newname/
---
## RevisionRenameSheet.NewName property

Hämtar det nya namnet på arbetsbladet.

```csharp
public string NewName { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och byt namn på det för att utlösa en revision
            Worksheet sheet = workbook.Worksheets[0];
            string originalName = sheet.Name;
            string newName = "RenamedSheet";
            sheet.Name = newName;

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
                        Console.WriteLine("Sheet renamed from '{0}' to '{1}'", 
                            renameSheet.OldName, renameSheet.NewName);
                        
                        // Demonstrera användning av egenskapen NewName
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

### Se även

* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


