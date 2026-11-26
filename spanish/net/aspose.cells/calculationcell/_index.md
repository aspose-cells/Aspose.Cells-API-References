---
title: "Clase CalculationCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CalculationCell. Representa los datos relevantes de cálculo sobre una celda que está siendo calculada"
type: docs
url: /es/net/aspose.cells/calculationcell/
---
## CalculationCell class

Representa los datos relevantes al cálculo de una celda que está siendo calculada.

```csharp
public class CalculationCell
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Cell](../../aspose.cells/calculationcell/cell/) { get; } | Obtiene el objeto Cell que está siendo calculado. |
| [CellColumn](../../aspose.cells/calculationcell/cellcolumn/) { get; } | Obtiene el índice de columna de la celda. |
| [CellRow](../../aspose.cells/calculationcell/cellrow/) { get; } | Obtiene el índice de fila de la celda. |
| [Workbook](../../aspose.cells/calculationcell/workbook/) { get; } | Obtiene el objeto Workbook. |
| [Worksheet](../../aspose.cells/calculationcell/worksheet/) { get; } | Obtiene el objeto Worksheet donde se encuentra la celda. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetCalculatedValue](../../aspose.cells/calculationcell/setcalculatedvalue/)(object) | Establece el valor calculado para la celda. |

### Observaciones

El usuario no debe cambiar ningún dato en el Workbook durante el proceso de cálculo de la fórmula, de lo contrario se pueden producir resultados inesperados o Exception. Por lo tanto, todos los objetos proporcionados por esta clase (como el objeto Cell de [`Cell`](./cell/)) son solo para propósito de "lectura".

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CellsClassCalculationCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Crear una instancia de CalculationCell usando reflexión ya que el constructor no es público
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell),
                    BindingFlags.NonPublic | BindingFlags.Instance,
                    null,
                    new object[] { workbook, worksheet, 0, 1, worksheet.Cells["B1"] },
                    null);

                // Mostrar propiedades básicas
                Console.WriteLine($"Cell Row: {calcCell.CellRow}");
                Console.WriteLine($"Cell Column: {calcCell.CellColumn}");
                Console.WriteLine($"Cell Value: {calcCell.Cell.Value}");
                Console.WriteLine($"Workbook Name: {calcCell.Workbook.FileName}");
                Console.WriteLine($"Worksheet Name: {calcCell.Worksheet.Name}");

                // Guarda el libro de trabajo
                workbook.Save("CalculationCellDemo.xlsx");
                Console.WriteLine("CalculationCell demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


