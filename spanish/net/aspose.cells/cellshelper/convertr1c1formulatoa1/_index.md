---
title: "CellsHelper.ConvertR1C1FormulaToA1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Convierte la fórmula r1c1 de la celda a fórmula A1"
type: docs
url: /es/net/aspose.cells/cellshelper/convertr1c1formulatoa1/
---
## CellsHelper.ConvertR1C1FormulaToA1 method

Convierte la fórmula r1c1 de la celda a fórmula A1.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertR1C1FormulaToA1(string r1c1Formula, int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| r1c1Formula | String | La fórmula r1c1. |
| fila | Int32 | El índice de fila de la celda. |
| columna | Int32 | El índice de columna de la celda. |

### Valor de retorno

La fórmula A1.

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método Worksheet.ConvertFormulaReferenceStyle(). Esta propiedad será eliminada 12 meses después, a partir de agosto de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodConvertR1C1FormulaToA1WithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer fórmulas R1C1 en celdas
            worksheet.Cells["A1"].R1C1Formula = "=R[1]C";
            worksheet.Cells["B1"].R1C1Formula = "=RC[1]";
            worksheet.Cells["A2"].R1C1Formula = "=R2C3";
            worksheet.Cells["B2"].R1C1Formula = "=R[-1]C[-1]";

            // Convertir fórmulas R1C0 al estilo A1
            string a1Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["A1"].R1C1Formula, 0, 0);
            string b1Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["B1"].R1C1Formula, 0, 0);
            string a2Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["A2"].R1C1Formula, 1, 2);
            string b2Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["B2"].R1C1Formula, 1, 1);

            // Genere la salida de los resultados
            Console.WriteLine("A1 R1C1: {0} -> A1: {1}", worksheet.Cells["A1"].R1C1Formula, a1Converted);
            Console.WriteLine("B1 R1C1: {0} -> A1: {1}", worksheet.Cells["B1"].R1C1Formula, b1Converted);
            Console.WriteLine("A2 R1C1: {0} -> A1: {1}", worksheet.Cells["A2"].R1C1Formula, a2Converted);
            Console.WriteLine("B2 R1C1: {0} -> A1: {1}", worksheet.Cells["B2"].R1C1Formula, b2Converted);
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


