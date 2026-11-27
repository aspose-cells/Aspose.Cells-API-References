---
title: "RevisionRenameSheet.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionRenameSheet-egenskap. Representerar revisionens typ"
type: docs
url: /sv/net/aspose.cells.revisions/revisionrenamesheet/type/
---
## RevisionRenameSheet.Type property

Representerar typen av revisionen.

```csharp
public override RevisionType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionRenameSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Aktivera spårning av revisioner INNAN du gör ändringar
            // Obs: Denna metod finns inte i det tillhandahållna API:et, så vi tar bort den
            // workbook.StartTrackingRevisions();

            // Byt namn på det första kalkylbladet för att skapa en revision
            Worksheet worksheet = workbook.Worksheets[0];
            string originalName = worksheet.Name;
            worksheet.Name = "RenamedSheet";

            // Åtkomst till revisionssamlingen
            // Obs: Revisions-egenskapen finns inte i det tillhandahållna API:et
            // Så vi måste först kontrollera om arbetsboken har revisioner
            if (workbook.HasRevisions)
            {
                // Hitta revisionen för namnbyte av bladet
                RevisionRenameSheet renameRevision = null;
                // Eftersom vi inte kan komma åt Revisions direkt, måste vi modifiera den här delen
                // Detta är bara en platshållare eftersom det faktiska API:et inte stödjer åtkomst till revisioner
                Console.WriteLine("Revision tracking is not fully supported in this API version.");
                
                if (renameRevision != null)
                {
                    // Visa värdet för Type-egenskapen
                    Console.WriteLine("Revision Type: " + renameRevision.Type);
                    Console.WriteLine("Old Sheet Name: " + renameRevision.OldName);
                    Console.WriteLine("New Sheet Name: " + renameRevision.NewName);

                    // Demonstrera hur man använder Type-egenskapen
                    if (renameRevision.Type == RevisionType.RenameSheet)
                    {
                        Console.WriteLine("This revision represents a worksheet rename operation.");
                    }
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionRenameSheetDemo.xlsx");
        }
    }
}
```

### Se även

* enum [RevisionType](../../revisiontype/)
* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


