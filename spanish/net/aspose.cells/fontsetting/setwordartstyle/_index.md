---
title: "FontSetting.SetWordArtStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FontSetting. Establece el estilo WordArt predefinido"
type: docs
url: /es/net/aspose.cells/fontsetting/setwordartstyle/
---
## FontSetting.SetWordArtStyle method

Establece el estilo predefinido de WordArt.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | PresetWordArtStyle | El estilo WordArt predefinido. |

### Observaciones

Solo para el texto de forma/gráfico.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FontSettingMethodSetWordArtStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue texto a la celda A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text for WordArt");

            // Crear configuración de fuente para el texto en la celda A1
            FontSetting fontSetting = new FontSetting(0, cell.StringValue.Length, workbook.Worksheets);

            try
            {
                // Aplicar estilo WordArt a la configuración de fuente
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle3);

                Console.WriteLine("WordArt style applied successfully to the text.");
                
                // Mostrar el efecto guardando el libro de trabajo
                worksheet.AutoFitColumn(0);
                worksheet.AutoFitRow(0);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("FontSettingMethodSetWordArtStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


