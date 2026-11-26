---
title: "SettableGlobalizationSettings.GetTableRowTypeOfCurrent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el nombre del tipo de filas de tabla que consiste en la fila actual en la tabla referenciada"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/
---
## SettableGlobalizationSettings.GetTableRowTypeOfCurrent method

Obtiene el nombre del tipo de filas de tabla que consiste en la fila actual de la tabla referenciada.

```csharp
public override string GetTableRowTypeOfCurrent()
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

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una tabla
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfCurrent("CurrentRow");

            // Aplicar configuraciones al libro de trabajo
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Obtener el nombre del tipo de fila actual
                string currentRowType = settings.GetTableRowTypeOfCurrent();
                Console.WriteLine("Current row type name: " + currentRowType);

                // Agregar una fórmula que haga referencia a la fila actual
                cells["C2"].Formula = "=SUM(#CurrentRow)";
                Console.WriteLine("Formula set to: " + cells["C2"].Formula);

                // Calcular fórmulas
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


