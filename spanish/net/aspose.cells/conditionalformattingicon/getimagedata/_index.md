---
title: "ConditionalFormattingIcon.GetImageData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ConditionalFormattingIcon. Obtiene los datos de la imagen con la configuración de la celda"
type: docs
url: /es/net/aspose.cells/conditionalformattingicon/getimagedata/
---
## ConditionalFormattingIcon.GetImageData method

Obtiene los datos de la imagen con la configuración de la celda.

```csharp
public byte[] GetImageData(Cell cell)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| celda | Celda | La configuración de la celda. |

### Valor de retorno

Devuelve los datos de la imagen del icono.

### Ejemplos

```csharp
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconMethodGetImageDataWithCellDemo
    {
        public static void Run()
        {
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            Workbook workbook = new Workbook("example.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            
            ConditionalFormattingIcon icon = worksheet.ConditionalFormattings[0][0].IconSet.CfIcons[0];
            
            Cell targetCell = worksheet.Cells["E1"];
            byte[] imageData = icon.GetImageData(targetCell);
            File.WriteAllBytes(Path.Combine(outputDir, "E1_icon.png"), imageData);
            
            targetCell = worksheet.Cells["G1"];
            imageData = icon.GetImageData(targetCell);
            File.WriteAllBytes(Path.Combine(outputDir, "G1_icon.png"), imageData);
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


