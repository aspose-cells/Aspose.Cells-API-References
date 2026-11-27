---
title: "RevisionRenameSheet.OldName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionRenameSheet-egenskap. Hämtar det gamla namnet på kalkylbladet"
type: docs
url: /sv/net/aspose.cells.revisions/revisionrenamesheet/oldname/
---
## RevisionRenameSheet.OldName property

Hämtar det gamla namnet på arbetsbladet.

```csharp
public string OldName { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionRenameSheetPropertyOldNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och byt namn på det för att utlösa en revision
            Worksheet sheet = workbook.Worksheets[0];
            string originalName = sheet.Name;
            sheet.Name = "RenamedSheet";

            // Åtkomst till revisionsloggarna
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.RenameSheet)
                    {
                        RevisionRenameSheet rsnm = (RevisionRenameSheet)rv;
                        Console.WriteLine("Sheet renamed from: {0} to: {1}", rsnm.OldName, rsnm.NewName);
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


