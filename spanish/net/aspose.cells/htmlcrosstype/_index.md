---
title: "Enum HtmlCrossType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.HtmlCrossType enum. Representa cinco tipos de cadena cruzada html"
type: docs
url: /es/net/aspose.cells/htmlcrosstype/
---
## HtmlCrossType enumeration

Representa cinco tipos de cadena cruzada HTML.

```csharp
public enum HtmlCrossType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Default | `0` | Mostrar como MS Excel, depende de la celda siguiente. Si la celda siguiente es nula, la cadena se cruzará, o será truncada |
| MSExport | `1` | Mostrar la cadena como MS Excel al exportar html. |
| Cross | `2` | Mostrar cadena cruzada HTML, este rendimiento para crear archivos html grandes será más de diez veces más rápido que establecer el valor a Default o FitToCell. |
| CrossHideRight | `3` | Mostrar cadena cruzada HTML y ocultar la cadena derecha cuando los textos se superponen. |
| FitToCell | `4` | Mostrar solo la cadena dentro del ancho de la celda. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHtmlCrossTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);
            
            // Crear opciones de guardado HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Establecer el tipo de cruce a MSExport
            options.HtmlCrossStringType = HtmlCrossType.MSExport;
            
            // Guardar libro con opciones HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with HtmlCrossType.MSExport");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


