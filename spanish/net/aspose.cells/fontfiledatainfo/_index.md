---
title: "Clase FontFileDataInfo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.FontFileDataInfo. Representa la información de datos del archivo de fuente"
type: docs
url: /es/net/aspose.cells/fontfiledatainfo/
---
## FontFileDataInfo class

Representa la información de datos del archivo de fuente.

```csharp
public class FontFileDataInfo
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Data](../../aspose.cells/fontfiledatainfo/data/) { get; } | Obtiene los datos binarios del archivo de fuente. |
| [FormatType](../../aspose.cells/fontfiledatainfo/formattype/) { get; } | Obtiene el tipo de formato de fuente del archivo de fuente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassFontFileDataInfoDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ejemplo: Cargando datos del archivo de fuente
            string fontFilePath = "arial.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Nota: FontFileDataInfo no puede instanciarse directamente ya que no tiene un constructor público
            // y sus propiedades son de solo lectura. En un escenario real, obtendrías una instancia
            // de otro método de API (como FontConfigs.GetFontFileDataInfo())
            FontFileDataInfo fontInfo = null; // Would be populated by API call in real scenario

            // Demostrar cómo se usarían las propiedades si tuviéramos una instancia
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
                Console.WriteLine("Font data length: " + (fontInfo.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            }

            // Demostrar la integración con Workbook
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Guarda el libro de trabajo
            workbook.Save("FontFileDataInfoDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


