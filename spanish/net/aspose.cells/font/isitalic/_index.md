---
title: "Font.IsItalic"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene o establece un valor que indica si la fuente está en cursiva"
type: docs
url: /es/net/aspose.cells/font/isitalic/
---
## Font.IsItalic property

Obtiene o establece un valor que indica si la fuente está en cursiva.

```csharp
public bool IsItalic { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsItalicDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder al estilo predeterminado
            Style style = workbook.DefaultStyle;
            
            // Establecer propiedades de la fuente incluyendo IsItalic
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.Font.IsItalic = true;
            
            // Aplicar el estilo a la celda A1
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Italic Text Example");
            
            // Guarda el libro de trabajo
            workbook.Save("FontPropertyIsItalicDemo.xlsx");
            
            // Verificar la propiedad cursiva
            Console.WriteLine("Font is italic: " + cell.GetStyle().Font.IsItalic);
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


