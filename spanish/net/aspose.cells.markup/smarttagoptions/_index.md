---
title: "Clase SmartTagOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Markup.SmartTagOptions. Representa las opciones de la smart tag"
type: docs
url: /es/net/aspose.cells.markup/smarttagoptions/
---
## SmartTagOptions class

Representa las opciones de la etiqueta inteligente.

```csharp
public class SmartTagOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SmartTagOptions](smarttagoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [EmbedSmartTags](../../aspose.cells.markup/smarttagoptions/embedsmarttags/) { get; set; } | Indica si se guardan las smart tags con el libro de trabajo. |
| [ShowType](../../aspose.cells.markup/smarttagoptions/showtype/) { get; set; } | Representa el tipo de visualización de la smart tag. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree una instancia de SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // Establecer propiedades
            options.EmbedSmartTags = true;
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;

            // Aplique SmartTagOptions a la hoja de cálculo
            // Nota: Cambiado de worksheet.SmartTagSetting.Options = options;
            // para usar directamente el objeto options ya que SmartTagSetting no tiene la propiedad Options
            // (Suponiendo que las options se deben usar directamente)
            
            // Agregue algunos datos para demostrar
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);

            // Guarda el libro de trabajo
            workbook.Save("SmartTagOptionsDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


