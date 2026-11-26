---
title: "CalculationCell.SetCalculatedValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CalculationCell. Establece el valor calculado para la celda"
type: docs
url: /es/net/aspose.cells/calculationcell/setcalculatedvalue/
---
## CalculationCell.SetCalculatedValue method

Establece el valor calculado para la celda.

```csharp
public void SetCalculatedValue(object v)
```

### Observaciones

El usuario puede establecer el resultado calculado mediante este método para ignorar el cálculo automático de la celda.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellMethodSetCalculatedValueWithObjectDemo
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

                // Establecer un valor calculado usando el método SetCalculatedValue
                calcCell.SetCalculatedValue(42); // Using an integer value as the Object parameter

                // Mostrar información sobre la celda
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);
                Console.WriteLine("SetCalculatedValue method called successfully with value: 42");

                // Guarda el libro de trabajo
                workbook.Save("SetCalculatedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetCalculatedValue: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


