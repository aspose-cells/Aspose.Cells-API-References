---
title: "RevisionInsertSheet.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionInsertSheet-egenskap. Hämtar namnet på kalkylbladet"
type: docs
url: /sv/net/aspose.cells.revisions/revisioninsertsheet/name/
---
## RevisionInsertSheet.Name property

Hämtar namnet på arbetsbladet.

```csharp
public string Name { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad för att eventuellt skapa en revisionspost
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

            try
            {
                // Simulera åtkomst till ett RevisionInsertSheet från revisioner
                // Obs: I ett verkligt scenario skulle detta komma från workbook.Revisions
                // För demonstration skapar vi ett simulerat scenario
                RevisionInsertSheet insertSheetRevision = null;

                // I faktisk användning skulle du hämta detta från revisionssamlingen
                // For example: insertSheetRevision = (RevisionInsertSheet)workbook.Revisions[0];

                // Eftersom vi inte kan skapa RevisionInsertSheet direkt, kommer vi att demonstrera
                // vad du skulle göra om du hade åtkomst till en
                if (insertSheetRevision != null)
                {
                    // Visa Name‑egenskapens värde (skrivskyddad)
                    Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);

                    // Demonstrera användning av Name‑egenskapen i en villkorskontroll
                    if (!string.IsNullOrEmpty(insertSheetRevision.Name))
                    {
                        Console.WriteLine("The sheet has a valid name: " + insertSheetRevision.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No RevisionInsertSheet found in revisions");
                }

                // Spara arbetsboken
                workbook.Save("RevisionInsertSheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


