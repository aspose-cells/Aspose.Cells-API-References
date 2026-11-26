---
title: "SettableGlobalizationSettings.SetTableRowTypeOfHeaders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el nombre de tipo de las filas de tabla que consisten en el encabezado de la tabla"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/
---
## SettableGlobalizationSettings.SetTableRowTypeOfHeaders method

Establece el nombre del tipo de filas de tabla que consiste en el encabezado de la tabla.

```csharp
public void SetTableRowTypeOfHeaders(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfHeadersWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una tabla y agregar algunos datos
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");
            
            // Crear un ListObject (Tabla)
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Crear una instancia de SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Llamar a SetTableRowTypeOfHeaders con un nombre de tipo de encabezado personalizado
                settings.SetTableRowTypeOfHeaders("CustomHeaders");

                // Aplicar la configuración al workbook
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table header type name set to: CustomHeaders");
                Console.WriteLine("In formulas, '#CustomHeaders' will now represent the table header");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfHeaders method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("SetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


