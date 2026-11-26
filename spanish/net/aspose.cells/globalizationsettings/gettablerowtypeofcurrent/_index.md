---
title: "GlobalizationSettings.GetTableRowTypeOfCurrent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre del tipo de filas de tabla que consiste en la fila actual en la tabla referenciada. El valor predeterminado es This Row, por lo que en la fórmula This Row representa la fila actual en la tabla referenciada"
type: docs
url: /es/net/aspose.cells/globalizationsettings/gettablerowtypeofcurrent/
---
## GlobalizationSettings.GetTableRowTypeOfCurrent method

Obtiene el nombre del tipo de filas de tabla que consiste en la fila actual de la tabla referenciada. El valor predeterminado es "This Row", por lo que en la fórmula "#This Row" representa la fila actual de la tabla referenciada.

```csharp
public virtual string GetTableRowTypeOfCurrent()
```

### Valor de retorno

el nombre de tipo de las filas de tabla

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class GlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer configuraciones de globalización personalizadas
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Cree datos de ejemplo y tabla
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(2.5);
                worksheet.Cells["A3"].PutValue("Orange");
                worksheet.Cells["B3"].PutValue(1.8);

                // Crear tabla
                int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.DisplayName = "PriceTable"; // Fixed property name

                // Agregar fórmula usando la referencia de fila actual
                Cell formulaCell = worksheet.Cells["C2"];
                formulaCell.Formula = "=PriceTable[@Price] * 1.2";

                // Demostrar el efecto de GetTableRowTypeOfCurrent
                Console.WriteLine("Generated formula: " + formulaCell.Formula);
                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTableRowTypeOfCurrent()
        {
            return "CurrentItem"; // Custom current row identifier
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


