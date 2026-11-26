---
title: "Enum OoxmlCompressionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.OoxmlCompressionType enum. El tipo de compresión Ooxml"
type: docs
url: /es/net/aspose.cells/ooxmlcompressiontype/
---
## OoxmlCompressionType enumeration

El tipo de compresión Ooxml

```csharp
public enum OoxmlCompressionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Level1 | `1` | La compresión más rápida pero menos eficaz. |
| Level2 | `2` | Un poco más lenta, pero mejor, que el nivel 1. |
| Level3 | `3` | Un poco más lenta, pero mejor, que el nivel 2. |
| Level4 | `4` | Un poco más lenta, pero mejor, que el nivel 3. |
| Level5 | `5` | Un poco más lenta que el nivel 4, pero con mejor compresión. |
| Level6 | `6` | Un buen equilibrio entre velocidad y eficiencia de compresión. |
| Level7 | `7` | ¡Compresión bastante buena! |
| Level8 | `8` | ¡Mejor compresión que Nivel7! |
| Level9 | `9` | La compresión "óptima", donde óptima significa la mayor reducción del tamaño del flujo de datos de entrada. Esta también es la compresión más lenta. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlCompressionTypeDemo
    {
        public static void OoxmlCompressionTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Crea OoxmlSaveOptions y establece el tipo de compresión
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6; // A good balance of speed and compression efficiency

            // Guarda el libro de trabajo con el tipo de compresión especificado
            workbook.Save("OoxmlCompressionTypeExample.xlsx", saveOptions);

            Console.WriteLine("Workbook saved with OoxmlCompressionType.Level6 compression.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


