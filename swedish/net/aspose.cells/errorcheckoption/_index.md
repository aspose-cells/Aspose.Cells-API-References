---
title: "Klass ErrorCheckOption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ErrorCheckOption-klass. Felkontrollinställning som tillämpas på vissa områden"
type: docs
url: /sv/net/aspose.cells/errorcheckoption/
---
## ErrorCheckOption class

Felkontrollinställning som tillämpas på vissa områden.

```csharp
public class ErrorCheckOption
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddRange](../../aspose.cells/errorcheckoption/addrange/)(CellArea) | Lägger till ett påverkad område med denna inställning. |
| [GetCountOfRange](../../aspose.cells/errorcheckoption/getcountofrange/)() | Hämtar antalet områden som påverkats av denna inställning. |
| [GetRange](../../aspose.cells/errorcheckoption/getrange/)(int) | Hämtar det påverkade området för denna inställning enligt angivet index. |
| [IsErrorCheck](../../aspose.cells/errorcheckoption/iserrorcheck/)(ErrorCheckType) | Kontrollerar om given feltyp kommer att kontrolleras. |
| [RemoveRange](../../aspose.cells/errorcheckoption/removerange/)(int) | Tar bort ett område med angivet index. |
| [SetErrorCheck](../../aspose.cells/errorcheckoption/seterrorcheck/)(ErrorCheckType, bool) | Ställer in om given feltyp ska kontrolleras. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionDemo
    {
        public static void ErrorCheckOptionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta ErrorCheckOptionCollection från kalkylbladet
            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;

            // Lägg till ett nytt ErrorCheckOption i samlingen
            int optionIdx = opts.Add();
            ErrorCheckOption opt = opts[optionIdx];

            // Ställ in felkontrollalternativ
            opt.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            opt.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            opt.SetErrorCheck(ErrorCheckType.TextDate, false);
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.SetErrorCheck(ErrorCheckType.Validation, false);

            // Definiera ett cellområde och lägg till det i ErrorCheckOption
            CellArea ca = CellArea.CreateCellArea("A1", "B10");
            opt.AddRange(ca);

            // Spara arbetsboken
            workbook.Save("ErrorCheckOptionExample.xlsx");
            workbook.Save("ErrorCheckOptionExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


