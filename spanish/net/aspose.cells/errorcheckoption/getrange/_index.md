---
title: "ErrorCheckOption.GetRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ErrorCheckOption method. Obtiene el rango influenciado de esta configuración por el índice dado"
type: docs
url: /es/net/aspose.cells/errorcheckoption/getrange/
---
## ErrorCheckOption.GetRange method

Obtiene el rango influenciado de esta configuración por el índice dado.

```csharp
public CellArea GetRange(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | el índice del rango |

### Valor de retorno

devuelve el rango influenciado en el índice dado.

### Ejemplos

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

            // Crear un ErrorCheckOption usando la colección ErrorCheckOptions de la hoja de cálculo
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

### Ver también

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


