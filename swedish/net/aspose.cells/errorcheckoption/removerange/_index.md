---
title: "ErrorCheckOption.RemoveRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ErrorCheckOption‑metod. Tar bort ett intervall enligt angivet index"
type: docs
url: /sv/net/aspose.cells/errorcheckoption/removerange/
---
## ErrorCheckOption.RemoveRange method

Tar bort ett område med angivet index.

```csharp
public void RemoveRange(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | index för det intervall som ska tas bort. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionMethodRemoveRangeWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;

            // Skapa ett nytt ErrorCheckOption och aktivera EmptyCellRef‑kontrollen
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];
            errorCheckOption.SetErrorCheck(ErrorCheckType.EmptyCellRef, true);

            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 1;
            area.EndColumn = 1;

            int rangeIndex = errorCheckOption.AddRange(area);
            int initialCount = errorCheckOption.GetCountOfRange();

            try
            {
                errorCheckOption.RemoveRange(rangeIndex);
                int finalCount = errorCheckOption.GetCountOfRange();
                Console.WriteLine($"Ranges before removal: {initialCount}, after removal: {finalCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveRange: {ex.Message}");
            }

            workbook.Save("ErrorCheckOptionRemoveRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


