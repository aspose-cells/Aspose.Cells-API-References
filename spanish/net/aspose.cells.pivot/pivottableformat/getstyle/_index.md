---
title: "PivotTableFormat.GetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTableFormat. Obtiene el estilo formateado"
type: docs
url: /es/net/aspose.cells.pivot/pivottableformat/getstyle/
---
## PivotTableFormat.GetStyle method

Obtiene el estilo formateado.

```csharp
public Style GetStyle()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableFormatMethodGetStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Obtenga el formato de tabla dinámica
            PivotTableFormatCollection formats = pivotTable.PivotFormats;
            PivotTableFormat format = formats[0];

            try
            {
                // Llame al método GetStyle
                Style style = format.GetStyle();

                // Propiedades del estilo de visualización
                Console.WriteLine("Style properties:");
                Console.WriteLine($"Font Name: {style.Font.Name}");
                Console.WriteLine($"Font Size: {style.Font.Size}");
                Console.WriteLine($"Background Color: {style.BackgroundColor}");

                // Modificar el estilo
                style.Font.Name = "Arial";
                style.Font.Size = 12;
                style.BackgroundColor = System.Drawing.Color.LightBlue;

                // Aplique el estilo modificado de nuevo al formato
                format.SetStyle(style);

                Console.WriteLine("GetStyle method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStyle method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("PivotTableFormatMethodGetStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


