---
title: "ErrorCheckOption.SetErrorCheck"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ErrorCheckOption-metoden. Anger om given feltyp ska kontrolleras"
type: docs
url: /sv/net/aspose.cells/errorcheckoption/seterrorcheck/
---
## ErrorCheckOption.SetErrorCheck method

Ställer in om given feltyp ska kontrolleras.

```csharp
public void SetErrorCheck(ErrorCheckType errorCheckType, bool isCheck)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | feltyp kan kontrolleras. |
| isCheck | Boolean | true om given feltyp behöver kontrolleras(grön triangel visas för cellen om kontrollen misslyckas). |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodSetErrorCheckWithErrorCheckTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("Sample text for error checking");
            
            // Konfigurera felkontrollalternativ
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];
            
            // Demonstrera SetErrorCheck med olika ErrorCheckType-värden
            errorCheckOption.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, true);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            
            // Tillämpa på hela kalkylbladet
            errorCheckOption.AddRange(CellArea.CreateCellArea(0, 0, worksheet.Cells.MaxRow, worksheet.Cells.MaxDataColumn));
            
            workbook.Save("ErrorCheckExample.xlsx");
        }
    }
}
```

### Se även

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


