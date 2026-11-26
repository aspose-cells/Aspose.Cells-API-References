---
title: "SettableGlobalizationSettings.SetTableRowTypeOfCurrent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el nombre de tipo de las filas de tabla que consisten en la fila actual en la tabla referenciada"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/
---
## SettableGlobalizationSettings.SetTableRowTypeOfCurrent method

Establece el nombre del tipo de filas de tabla que consiste en la fila actual de la tabla referenciada.

```csharp
public void SetTableRowTypeOfCurrent(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfCurrentWithStringDemo
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
            cells["B2"].PutValue("2.5");
            cells["A3"].PutValue("Banana");
            cells["B3"].PutValue("1.5");
            
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Crear configuraciones de globalización
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            try
            {
                // Establezca un nombre personalizado para el tipo de fila actual
                settings.SetTableRowTypeOfCurrent("CurrentItem");
                
                // Aplicar configuraciones al libro de trabajo
                workbook.Settings.GlobalizationSettings = settings;

                // Verifique la configuración obteniendo el valor de nuevo
                string currentRowType = settings.GetTableRowTypeOfCurrent();
                Console.WriteLine($"Current row type name set to: {currentRowType}");

                // Guarda el libro de trabajo
                workbook.Save("SetTableRowTypeOfCurrentDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfCurrent method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


