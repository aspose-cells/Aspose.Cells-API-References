---
title: "FileFontSource.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FileFontSource. Devuelve el tipo de la fuente"
type: docs
url: /es/net/aspose.cells/filefontsource/type/
---
## FileFontSource.Type property

Devuelve el tipo del origen de la fuente.

```csharp
public override FontSourceType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            string fontFilePath = "CustomFont.ttf";
            
            // Crear una instancia de FileFontSource
            FileFontSource fontSource = new FileFontSource(fontFilePath);
            
            // Demostrar el uso de la propiedad Type
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            
            // Crear libro de trabajo y aplicar fuente
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Text with custom font");
            
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont";
            cell.SetStyle(style);
            
            workbook.Save("FontSourceDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FontSourceType](../../fontsourcetype/)
* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


