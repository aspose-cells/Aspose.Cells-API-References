---
title: "ErrorCheckOption.RemoveRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ErrorCheckOption-Methode. Entfernt einen Bereich anhand des angegebenen Indexes"
type: docs
url: /de/net/aspose.cells/errorcheckoption/removerange/
---
## ErrorCheckOption.RemoveRange method

Entfernt einen Bereich anhand des angegebenen Index.

```csharp
public void RemoveRange(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index des zu entfernenden Bereichs. |

### Beispiele

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

            // Erstelle ein neues ErrorCheckOption und aktiviere die EmptyCellRef-Prüfung
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

### Siehe auch

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


