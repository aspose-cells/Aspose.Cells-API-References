---
title: "SettableGlobalizationSettings.SetTableRowTypeOfTotals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el nombre de tipo de las filas de tabla que consisten en la fila de total de la tabla referenciada"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/
---
## SettableGlobalizationSettings.SetTableRowTypeOfTotals method

Establece el nombre del tipo de filas de tabla que consiste en la fila total de la tabla referenciada.

```csharp
public void SetTableRowTypeOfTotals(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | el nombre de tipo de las filas de tabla |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfTotalsWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una tabla
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(10);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(15);
            cells["A4"].PutValue("Total");
            cells["B4"].PutValue("=SUM(B2:B3)");

            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;

            // Crear configuraciones de globalización
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Llamar a SetTableRowTypeOfTotals con un nombre personalizado
                settings.SetTableRowTypeOfTotals("CustomTotals");

                // Aplicar configuraciones al libro de trabajo
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetTableRowTypeOfTotals executed successfully with parameter: CustomTotals");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfTotals method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("SetTableRowTypeOfTotalsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


