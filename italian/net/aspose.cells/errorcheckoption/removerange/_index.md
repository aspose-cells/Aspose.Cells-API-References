---
title: "ErrorCheckOption.RemoveRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ErrorCheckOption. Rimuove un intervallo dato l'indice specificato"
type: docs
url: /it/net/aspose.cells/errorcheckoption/removerange/
---
## ErrorCheckOption.RemoveRange method

Rimuove un intervallo per l'indice fornito.

```csharp
public void RemoveRange(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | l'indice dell'intervallo da rimuovere. |

### Esempi

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

            // Crea un nuovo ErrorCheckOption e abilita il controllo EmptyCellRef
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

### Vedi anche

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


