---
title: "Font.Color"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene o establece el Color de la fuente"
type: docs
url: /es/net/aspose.cells/font/color/
---
## Font.Color property

Obtiene o establece el Color de la fuente.

```csharp
public Color Color { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FontPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer HTML con diferentes colores y estilos de fuente
            Cell cell = worksheet.Cells["A1"];
            cell.HtmlString = "<font color='Red'>Red Text</font> <font color='#0000FF'>Blue Text</font><font style='color:#00FF00;text-decoration: underline;'>Green Underlined</font>";
            
            // Obtener formato de texto enriquecido
            FontSetting[] richText = cell.GetCharacters();
            
            // Verificar y demostrar las propiedades de color
            Console.WriteLine("First segment color: " + richText[0].Font.Color);
            Console.WriteLine("Second segment color: " + richText[1].Font.Color);
            Console.WriteLine("Third segment underline: " + richText[2].Font.Underline);
            
            // Guarda el libro de trabajo
            workbook.Save("FontColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


