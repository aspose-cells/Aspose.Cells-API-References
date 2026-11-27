---
title: "ErrorCheckOption.GetRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ErrorCheckOption-metoden. Hämtar det påverkade området för denna inställning enligt angivet index"
type: docs
url: /sv/net/aspose.cells/errorcheckoption/getrange/
---
## ErrorCheckOption.GetRange method

Hämtar det påverkade området för denna inställning enligt angivet index.

```csharp
public CellArea GetRange(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | indexen för intervallet |

### Returvärde

returnerar påverkade intervallet vid angivet index.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionMethodGetRangeWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett ErrorCheckOption med hjälp av kalkylbladets ErrorCheckOptions-samling
            int errorCheckIndex = worksheet.ErrorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = worksheet.ErrorCheckOptions[errorCheckIndex];

            CellArea area = new CellArea();
            area.StartRow = 1;
            area.StartColumn = 1;
            area.EndRow = 3;
            area.EndColumn = 3;
            int addedIndex = errorCheckOption.AddRange(area);

            try
            {
                int rangeCount = errorCheckOption.GetCountOfRange();
                if (rangeCount > 0)
                {
                    CellArea retrievedArea = errorCheckOption.GetRange(0);
                    Console.WriteLine($"Retrieved range: StartRow={retrievedArea.StartRow}, StartColumn={retrievedArea.StartColumn}, " +
                        $"EndRow={retrievedArea.EndRow}, EndColumn={retrievedArea.EndColumn}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRange method: {ex.Message}");
            }

            workbook.Save("ErrorCheckOptionMethodGetRangeWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


