---
title: "RevisionHeader.UserName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionHeader‑egenskap. Hämtar och anger namnet på användaren som gör revisionen"
type: docs
url: /sv/net/aspose.cells.revisions/revisionheader/username/
---
## RevisionHeader.UserName property

Hämtar och anger namnet på användaren som gör revisionen.

```csharp
public string UserName { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertyUserNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Skapa en RevisionHeader‑instans
                RevisionHeader revisionHeader = new RevisionHeader();

                // Ange egenskapen UserName
                revisionHeader.UserName = "JohnDoe";

                // Visa det aktuella värdet för egenskapen UserName
                Console.WriteLine("UserName value: " + revisionHeader.UserName);

                // Ändra egenskapen UserName
                revisionHeader.UserName = "JaneSmith";
                Console.WriteLine("Modified UserName value: " + revisionHeader.UserName);

                // Spara arbetsboken för att demonstrera att egenskapen används
                workbook.Save("UserNameDemo.xlsx");
                Console.WriteLine("UserName property has been demonstrated and workbook saved.");
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

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


