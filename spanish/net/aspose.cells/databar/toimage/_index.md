---
title: "DataBar.ToImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DataBar. Renderizar la barra de datos en la celda a una matriz de bytes de imagen"
type: docs
url: /es/net/aspose.cells/databar/toimage/
---
## DataBar.ToImage method

Renderizar la barra de datos en la celda a una matriz de bytes de imagen.

```csharp
public byte[] ToImage(Cell cell, ImageOrPrintOptions imgOpts)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| celda | Celda | Indicar la barra de datos en qué celda se debe renderizar |
| imgOpts | ImageOrPrintOptions | ImageOrPrintOptions contiene algunas propiedades de la imagen de salida |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class DataBarMethodToImageWithCellImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo y formato condicional
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            
            // Agregar formato condicional de barra de datos
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);
            
            idx = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcc[idx];
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            
            // Obtener la celda con formato condicional
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            
            if (result != null && result.ConditionalFormattingDataBar != null)
            {
                DataBar bar = result.ConditionalFormattingDataBar;
                ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
                
                // Convertir la barra de datos a imagen
                byte[] img = bar.ToImage(cell, imgOpts);
                
                // Guardar la imagen
                string outputPath = "DataBarImage.png";
                File.WriteAllBytes(outputPath, img);
                
                // Para la verificación de la imagen, necesitará agregar el paquete System.Drawing.Common
                // y usar System.Drawing.Image si es necesario
                Console.WriteLine($"Data bar image saved to {outputPath}");
            }
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


