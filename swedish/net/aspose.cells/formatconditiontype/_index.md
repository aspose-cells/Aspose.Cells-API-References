---
title: "Enum FormatConditionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FormatConditionType enum. Typ av villkorsformatregel"
type: docs
url: /sv/net/aspose.cells/formatconditiontype/
---
## FormatConditionType enumeration

Villkorlig formatregeltyp.

```csharp
public enum FormatConditionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| CellValue | `1` | Denna villkorsformateringsregel jämför ett cellvärde med ett formelberäknat resultat med hjälp av en operator. |
| Expression | `2` | Denna villkorsformateringsregel innehåller en formel att utvärdera. När formelresultatet är sant markeras cellen. |
| Top10 | `4` | Denna villkorsformateringsregel markerar celler vars värden faller inom de översta N eller nedersta N intervallen, enligt specifikationen. |
| UniqueValues | `8` | Denna villkorsformateringsregel markerar unika värden i intervallet. |
| DuplicateValues | `16` | Denna villkorsformateringsregel markerar duplicerade värden. |
| ContainsText | `32` | Denna villkorsformateringsregel markerar celler som innehåller given text. Motsvarande att använda bladfunktionen SEARCH() för att avgöra om cellen innehåller texten. |
| NotContainsText | `64` | Denna villkorsformateringsregel markerar celler som inte innehåller given text. Motsvarande att använda bladfunktionen SEARCH() för att avgöra om cellen innehåller texten eller inte. |
| BeginsWith | `128` | Denna villkorsformateringsregel markerar celler i intervallet som börjar med given text. Motsvarande att använda bladfunktionen LEFT() och jämföra värden. |
| EndsWith | `256` | Denna villkorsformateringsregel markerar celler som slutar med given text. Motsvarande att använda bladfunktionen RIGHT() och jämföra värden. |
| ContainsBlanks | `512` | Denna villkorsformateringsregel markerar celler som är helt tomma. Motsvarande att använda LEN(TRIM()). Detta betyder att om cellen endast innehåller tecken som TRIM() skulle ta bort, betraktas den som tom. En tom cell betraktas också som tom. |
| NotContainsBlanks | `1024` | Denna villkorsformateringsregel markerar celler som inte är tomma. Motsvarande att använda LEN(TRIM()). Detta betyder att om cellen endast innehåller tecken som TRIM() skulle ta bort, betraktas den som tom. En tom cell betraktas också som tom. |
| ContainsErrors | `2048` | Denna villkorsformateringsregel markerar celler med formelfel. Motsvarande att använda bladfunktionen ISERROR() för att avgöra om det finns ett formelfel. |
| NotContainsErrors | `4096` | Denna villkorsformateringsregel markerar celler utan formelfel. Motsvarande att använda bladfunktionen ISERROR() för att avgöra om det finns ett formelfel. |
| TimePeriod | `8192` | Denna villkorsformateringsregel markerar celler som innehåller datum under den angivna tidsperioden. Cellens underliggande värde utvärderas, därför behöver cellen inte vara formaterad som ett datum för att utvärderas. Till exempel, med en cell som innehåller värdet 38913 ska den villkorsstyrda formateringen tillämpas om regeln kräver ett värde av 7/14/2006. |
| AboveAverage | `16384` | Denna villkorsformateringsregel markerar celler som ligger över eller under genomsnittet för alla värden i intervallet. |
| ColorScale | `32768` | Denna villkorsformateringsregel skapar en graderad färgskala på cellerna. |
| DataBar | `65536` | Denna villkorsformateringsregel visar en graderad datastapel i cellintervallet. |
| IconSet | `131072` | Denna villkorsformateringsregel tillämpar ikoner på celler enligt deras värden. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionTypeDemo
    {
        public static void FormatConditionTypeExample()
        {
            // Skapa en ny arbetsbok.
            Workbook workbook = new Workbook();

            // Hämta det första kalkylbladet.
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägger till en tom villkorlig formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Ställer in det villkorsstyrda formatintervallet.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Lägger till ett villkor för AboveAverage
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // Ställer in egenskaper för AboveAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // Lägger till ett villkor för CellValue
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = Color.Red;

            // Lägger till ett villkor för ContainsText
            int conditionIndex3 = fcs.AddCondition(FormatConditionType.ContainsText);
            FormatCondition fc3 = fcs[conditionIndex3];
            fc3.Text = "Sample";
            fc3.Style.BackgroundColor = Color.Green;

            // Spara Excel-filen
            workbook.Save("FormatConditionTypeExample.xlsx");
            workbook.Save("FormatConditionTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


