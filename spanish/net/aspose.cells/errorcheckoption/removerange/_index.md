---
title: "ErrorCheckOption.RemoveRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ErrorCheckOption. Elimina un rango dado su índice"
type: docs
url: /es/net/aspose.cells/errorcheckoption/removerange/
---
## ErrorCheckOption.RemoveRange method

Elimina un rango por el índice dado.

```csharp
public void RemoveRange(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | el índice del rango a eliminar. |

### Ejemplos

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

            // Crea una nueva ErrorCheckOption y habilita la verificación EmptyCellRef
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

### Ver también

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


