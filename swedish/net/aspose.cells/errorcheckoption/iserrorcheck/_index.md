---
title: "ErrorCheckOption.IsErrorCheck"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ErrorCheckOption-metoden. Kontrollerar om given feltyp kommer att kontrolleras"
type: docs
url: /sv/net/aspose.cells/errorcheckoption/iserrorcheck/
---
## ErrorCheckOption.IsErrorCheck method

Kontrollerar om given feltyp kommer att kontrolleras.

```csharp
public bool IsErrorCheck(ErrorCheckType errorCheckType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | feltyp kan kontrolleras |

### Returvärde

return true om given feltyp kommer att kontrolleras(grön triangel visas för cellen om kontrollen misslyckas).

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodIsErrorCheckWithErrorCheckTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            int index = options.Add();
            ErrorCheckOption option = options[index];

            // Konfigurera felkontrollinställningar
            option.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            option.SetErrorCheck(ErrorCheckType.EvaluationError, true);
            option.SetErrorCheck(ErrorCheckType.InconsistRange, false);

            // Lägg till område för att tillämpa dessa inställningar
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 10;
            area.StartColumn = 0;
            area.EndColumn = 5;
            option.AddRange(area);

            // Verifiera och visa inställningarna
            Console.WriteLine("NumberStoredAsText check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.NumberStoredAsText));
            Console.WriteLine("EvaluationError check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.EvaluationError));
            Console.WriteLine("InconsistRange check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.InconsistRange));
        }
    }
}
```

### Se även

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


