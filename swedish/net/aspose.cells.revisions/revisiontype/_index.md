---
title: "Enum RevisionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionType enum. Representerar revisionstypen"
type: docs
url: /sv/net/aspose.cells.revisions/revisiontype/
---
## RevisionType enumeration

Representerar revisionstypen.

```csharp
public enum RevisionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| CustomView | `0` | Anpassad vy. |
| DefinedName | `1` | Definierat namn. |
| ChangeCells | `2` | Celländring. |
| AutoFormat | `3` | Autoformat. |
| MergeConflict | `4` | Sammanfogningskonflikt. |
| Comment | `5` | Kommentar. |
| Format | `6` | Format. |
| InsertSheet | `7` | Infoga kalkylblad. |
| MoveCells | `8` | Flytta celler. |
| Undo | `9` | Ångra. |
| QueryTable | `10` | Frågetabell. |
| InsertDelete | `11` | Infogning eller borttagning. |
| RenameSheet | `12` | Byt namn på kalkylblad. |
| Unknown | `13` | Okänt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demonstrera användning av olika RevisionType enum‑värden
                RevisionType customViewType = RevisionType.CustomView;
                RevisionType changeCellsType = RevisionType.ChangeCells;
                RevisionType insertSheetType = RevisionType.InsertSheet;

                // Visa enum‑värden och deras underliggande heltalsvärden
                Console.WriteLine("CustomView type: " + customViewType + " (Value: " + (int)customViewType + ")");
                Console.WriteLine("ChangeCells type: " + changeCellsType + " (Value: " + (int)changeCellsType + ")");
                Console.WriteLine("InsertSheet type: " + insertSheetType + " (Value: " + (int)insertSheetType + ")");

                // Demonstrera kontroll av revisionstyper
                if (workbook.HasRevisions)
                {
                    Console.WriteLine("Workbook contains revisions");
                }
                else
                {
                    Console.WriteLine("Workbook has no revisions");
                }

                // Spara arbetsboken
                workbook.Save("RevisionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionType: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


