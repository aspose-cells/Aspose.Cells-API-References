---
title: "SettableGlobalizationSettings.GetTableRowTypeOfHeaders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el nombre del tipo de filas de tabla que consisten en el encabezado de la tabla. El valor predeterminado es Headers, por lo que en la fórmula Headers representa el encabezado de la tabla"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/
---
## SettableGlobalizationSettings.GetTableRowTypeOfHeaders method

Obtiene el nombre del tipo de filas de tabla que consiste en el encabezado de la tabla. El predeterminado es "Headers", por lo que en la fórmula "#Headers" representa el encabezado de la tabla.

```csharp
public override string GetTableRowTypeOfHeaders()
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

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfHeadersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfHeaders("CustomHeaders");
            workbook.Settings.GlobalizationSettings = settings;

            // Crear datos de tabla de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);

            try
            {
                // Obtenga el tipo de fila de tabla para encabezados
                string rowType = settings.GetTableRowTypeOfHeaders();
                Console.WriteLine($"Table row type for headers: {rowType}");

                // Crear un ListObject (Tabla)
                ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "B3", true)];

                // Utilice la referencia de encabezado personalizada en una fórmula
                worksheet.Cells["C2"].Formula = "=COUNTA(Table1[#CustomHeaders])";
                Console.WriteLine("Formula using custom headers reference: " + worksheet.Cells["C2"].Formula);

                // Calcular la fórmula
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfHeaders method: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


