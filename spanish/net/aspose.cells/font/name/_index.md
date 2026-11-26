---
title: "Font.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene o establece el nombre de la Font"
type: docs
url: /es/net/aspose.cells/font/name/
---
## Font.Name property

Obtiene o establece el nombre del [`Font`](../).

```csharp
public virtual string Name { get; set; }
```

### Observaciones

Si esta propiedad se usa para establecer el nombre de la fuente, el [`SchemeType`](../schemetype/) se actualizará a None

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la hoja de cálculo y celdas predeterminadas
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Crear y modificar un estilo con propiedades de fuente
            Style style = workbook.CreateStyle();
            Font font = style.Font;
            
            // Demostrar el uso de la propiedad Name
            font.Name = "Arial";  // Changed from FontNameConstants.Arial to string literal
            font.Size = 14;
            font.IsBold = true;
            
            // Aplicar el estilo a una celda
            cells["A1"].PutValue("Font Property Name Demo");
            cells["A1"].SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("FontPropertyNameDemo.xlsx");
            
            Console.WriteLine("Demo completed. File saved as FontPropertyNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


