---
title: "Enum ErrorCheckType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ErrorCheckType enum. Representerar alla felkontrolltyper"
type: docs
url: /sv/net/aspose.cells/errorchecktype/
---
## ErrorCheckType enumeration

Representerar alla felkontrolltyper.

```csharp
public enum ErrorCheckType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| EvaluationError | `1` | Ignorera fel när celler innehåller formler som resulterar i ett fel. |
| Calc | `1` |  |
| EmptyCellRef | `2` | Ignorera fel när formler refererar till tomma celler. |
| NumberStoredAsText | `4` | Ignorera fel när tal är formaterade som text eller föregås av ett apostrof |
| TextNumber | `4` | Ignorera fel när tal är formaterade som text eller föregås av ett apostrof |
| InconsistRange | `8` | Ignorera fel när formler utelämnar vissa celler i ett område. |
| InconsistFormula | `16` | Ignorera fel när en formel i ett område i ditt kalkylblad skiljer sig från andra formler i samma område. |
| TwoDigitTextYear | `32` | Ignorera fel när formler innehåller textformaterade celler med år representerade med två siffror. |
| TextDate | `32` | Ignorera fel när formler innehåller textformaterade celler med år representerade med två siffror. |
| UnlockedFormula | `64` | Ignorera fel när olåsta celler innehåller formler. |
| UnproctedFormula | `64` | Ignorera fel när olåsta celler innehåller formler. |
| TableDataValidation | `128` | Ignorera fel när ett cells värde i en tabell inte följer de angivna datavalideringsreglerna. |
| Validation | `128` | Ignorera fel när ett cells värde i en tabell inte följer de angivna datavalideringsreglerna. |
| CalculatedColumn | `129` | Ignorera fel när celler innehåller ett värde som skiljer sig från en beräknad kolumnformel. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckTypeDemo
    {
        public static void ErrorCheckTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till ErrorCheckOptionCollection
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;

            // Lägg till ett nytt ErrorCheckOption
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];

            // Ställ in olika felkontrolltyper till falskt
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.Validation, false);

            // Definiera ett cellområde för felkontrollalternativet
            CellArea cellArea = CellArea.CreateCellArea("A1", "B10");
            errorCheckOption.AddRange(cellArea);

            // Spara arbetsboken
            workbook.Save("ErrorCheckTypeExample.xlsx");
            workbook.Save("ErrorCheckTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


