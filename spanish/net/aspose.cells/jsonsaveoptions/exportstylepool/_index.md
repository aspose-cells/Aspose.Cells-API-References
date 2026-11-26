---
title: "JsonSaveOptions.ExportStylePool"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonSaveOptions. Indica si se exportan los estilos de forma colectiva o individualmente a cada celda"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/exportstylepool/
---
## JsonSaveOptions.ExportStylePool property

Indica si exportar estilos de forma colectiva o individual a cada celda.

```csharp
public bool ExportStylePool { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonSaveOptionsPropertyExportStylePoolDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra con diferentes estilos
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);

            // Aplique diferentes estilos a las celdas
            Aspose.Cells.Style style1 = workbook.CreateStyle();
            style1.Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["A1"].SetStyle(style1);

            Aspose.Cells.Style style2 = workbook.CreateStyle();
            style2.Font.Color = System.Drawing.Color.Blue;
            worksheet.Cells["B1"].SetStyle(style2);

            try
            {
                // Crear JsonSaveOptions con ExportStylePool = true (exportación colectiva)
                JsonSaveOptions options1 = new JsonSaveOptions();
                options1.ExportStylePool = true;
                Console.WriteLine("ExportStylePool (collective): " + options1.ExportStylePool);

                // Guardar con exportación de estilo colectiva
                workbook.Save("output_collective_styles.json", options1);

                // Crear JsonSaveOptions con ExportStylePool = false (exportación individual)
                JsonSaveOptions options2 = new JsonSaveOptions();
                options2.ExportStylePool = false;
                Console.WriteLine("ExportStylePool (individual): " + options2.ExportStylePool);

                // Guardar con exportación de estilo individual
                workbook.Save("output_individual_styles.json", options2);

                Console.WriteLine("ExportStylePool demonstration completed successfully.");
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

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


