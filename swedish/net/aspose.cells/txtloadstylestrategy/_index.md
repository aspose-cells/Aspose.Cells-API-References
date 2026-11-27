---
title: "Enum TxtLoadStyleStrategy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.TxtLoadStyleStrategy enum. Anger hur stil ska tillämpas för analyserade värden när en strängvärde konverteras till nummer eller datum/tid"
type: docs
url: /sv/net/aspose.cells/txtloadstylestrategy/
---
## TxtLoadStyleStrategy enumeration

Anger hur stil ska tillämpas för analyserade värden när en strängvärde konverteras till tal eller datum/tid.

```csharp
public enum TxtLoadStyleStrategy
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ställer inte in stil för det analyserade värdet. |
| BuiltIn | `1` | Ställ in stilen som inbyggt nummer/datum-tid när det analyserade värdet är enkla numeriska/datum-tid-värden. |
| ExactFormat | `2` | Ställ in exakt anpassat format för det analyserade värdet så att det formaterade värdet blir samma som det ursprungliga inmatade. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtLoadStyleStrategyDemo
    {
        public static void TxtLoadStyleStrategyExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Definiera ett exempel på CSV-innehåll
            string csvContent = "Name,Date,Value\nJohn,2023-01-01,100\nDoe,2023-01-02,200";

            // Spara CSV-innehållet till en temporär fil
            string tempCsvFilePath = "sample.csv";
            System.IO.File.WriteAllText(tempCsvFilePath, csvContent);

            // Skapa TxtLoadOptions och ställ in LoadStyleStrategy
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.ExactFormat;

            // Läs in CSV-filen i arbetsboken
            workbook = new Workbook(tempCsvFilePath, loadOptions);

            // Spara arbetsboken till en Excel-fil
            workbook.Save("TxtLoadStyleStrategyExample.xlsx");

            // Rensa upp den temporära CSV-filen
            System.IO.File.Delete(tempCsvFilePath);

            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


