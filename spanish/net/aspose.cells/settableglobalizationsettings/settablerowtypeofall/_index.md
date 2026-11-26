---
title: "SettableGlobalizationSettings.SetTableRowTypeOfAll"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el nombre de tipo de las filas de tabla que consisten en todas las filas en la tabla referenciada"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/settablerowtypeofall/
---
## SettableGlobalizationSettings.SetTableRowTypeOfAll method

Establece el nombre del tipo de filas de tabla que consiste en todas las filas de la tabla referenciada.

```csharp
public void SetTableRowTypeOfAll(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfAllWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree datos de muestra para una tabla
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);

            // Crear una tabla
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Llame a SetTableRowTypeOfAll con un nombre personalizado
                settings.SetTableRowTypeOfAll("CompleteTable");

                // Aplicar configuraciones al libro de trabajo
                workbook.Settings.GlobalizationSettings = settings;

                // Verifique la configuración obteniendo el valor de nuevo
                string rowType = settings.GetTableRowTypeOfAll();
                Console.WriteLine($"Table row type for all rows set to: {rowType}");

                // Agregar una fórmula que haga referencia a todas las filas usando el nombre personalizado
                cells["C2"].Formula = "=SUM(#CompleteTable[Price])";
                Console.WriteLine($"Formula using custom row type: {cells["C2"].Formula}");

                // Calcular fórmulas
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result: {cells["C2"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfAll method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("MethodSetTableRowTypeOfAllWithStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


