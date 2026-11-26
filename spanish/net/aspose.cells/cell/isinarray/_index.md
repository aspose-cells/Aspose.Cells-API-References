---
title: "Cell.IsInArray"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Indica si la fórmula de la celda es una fórmula de matriz"
type: docs
url: /es/net/aspose.cells/cell/isinarray/
---
## Cell.IsInArray property

Indica si la fórmula de la celda es una fórmula de matriz.

```csharp
[Obsolete("Use IsArrayFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInArray { get; }
```

### Observaciones

NOTA: Esta clase está ahora obsoleta. En su lugar, utilice Cell.IsArrayFormula para comprobar si la fórmula de la celda es una fórmula de matriz. Esta propiedad será eliminada 12 meses después, desde mayo de 2018. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsInArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo con fórmulas de matriz
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Establecer una fórmula de matriz usando la API correcta
            worksheet.Cells["C2"].SetArrayFormula("A2:A3*B2:B3", 2, 1);

            // Comprobar la propiedad IsInArray
            Cell cellInArray = worksheet.Cells["C2"];
            Cell cellNotInArray = worksheet.Cells["A2"];

            Console.WriteLine("Cell C2 is in array: " + cellInArray.IsInArray);
            Console.WriteLine("Cell A2 is in array: " + cellNotInArray.IsInArray);

            // Demostrar la eliminación de celdas que no son de matriz
            for (int row = 1; row <= 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = worksheet.Cells[row, col];
                    if (!cell.IsInArray && !cell.IsFormula)
                    {
                        cell.PutValue("");
                    }
                }
            }

            // Guarda el libro de trabajo
            workbook.Save("IsInArrayDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


