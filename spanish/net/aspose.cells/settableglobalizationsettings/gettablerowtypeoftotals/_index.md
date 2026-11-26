---
title: "SettableGlobalizationSettings.GetTableRowTypeOfTotals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el nombre de tipo de las filas de tabla que consisten en la fila total de la tabla referenciada"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/
---
## SettableGlobalizationSettings.GetTableRowTypeOfTotals method

Obtiene el nombre del tipo de filas de tabla que consiste en la fila total de la tabla referenciada.

```csharp
public override string GetTableRowTypeOfTotals()
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

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfTotalsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de tabla de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Total");
            worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");

            // Crear un ListObject (Tabla)
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfTotals("CustomTotals");

            try
            {
                // Obtener el tipo de fila de tabla para totales
                string rowType = settings.GetTableRowTypeOfTotals();
                Console.WriteLine($"Table row type for totals: {rowType}");

                // Aplicar configuraciones al libro de trabajo
                workbook.Settings.GlobalizationSettings = settings;

                // Verificar el efecto en una fórmula
                worksheet.Cells["C2"].Formula = "=SUM(#CustomTotals[B])";
                Console.WriteLine("Formula using custom totals reference: " + worksheet.Cells["C2"].Formula);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfTotals method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("MethodGetTableRowTypeOfTotalsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


