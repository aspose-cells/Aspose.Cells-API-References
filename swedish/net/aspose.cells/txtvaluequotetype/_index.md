---
title: "Enum TxtValueQuoteType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.TxtValueQuoteType‑enum. Anger typen av användning av citationstecken för värden i textformatfiler."
type: docs
url: /sv/net/aspose.cells/txtvaluequotetype/
---
## TxtValueQuoteType enumeration

Anger typen av användning av citationstecken för värden i textformatfiler.

```csharp
public enum TxtValueQuoteType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Normal | `0` | Alla värden som innehåller specialtecken såsom citationstecken eller separator‑tecken kommer att omges av citationstecken. Samma beteende som i MS Excel vid export av textfil. |
| Always | `1` | Alla värden kommer alltid att omges av citationstecken. |
| Minimum | `2` | Citattecken sätts endast runt värden när det behövs. Till exempel, om ett värde innehåller ett citationstecken men citationstecknet inte står i början av värdet, kommer detta värde inte att omges av citationstecken. |
| Never | `3` | Inga värden kommer att omges av citationstecken. Den exporterade textfilen med denna typ kanske inte kan läsas in korrekt eftersom nödvändiga citationstecken saknas. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtValueQuoteTypeDemo
    {
        public static void TxtValueQuoteTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells[0, 0].Value = "Name";
            worksheet.Cells[0, 1].Value = "Age";
            worksheet.Cells[1, 0].Value = "John Doe";
            worksheet.Cells[1, 1].Value = 30;
            worksheet.Cells[2, 0].Value = "Jane Smith";
            worksheet.Cells[2, 1].Value = 25;

            // Skapa TxtSaveOptions och ange QuoteType
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.QuoteType = TxtValueQuoteType.Always;

            // Spara arbetsboken som en textfil med den angivna citationsteckentypen
            workbook.Save("TxtValueQuoteTypeExample.txt", saveOptions);

            Console.WriteLine("Workbook saved with TxtValueQuoteType.Always");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


