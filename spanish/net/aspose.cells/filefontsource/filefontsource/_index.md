---
title: "FileFontSource.FileFontSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de FileFontSource. Ctor"
type: docs
url: /es/net/aspose.cells/filefontsource/filefontsource/
---
## FileFontSource constructor

Ctor.

```csharp
public FileFontSource(string filePath)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | String | ruta al archivo de fuente |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFontSourceMethodCtorWithStringDemo
    {
        public static void Run()
        {
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            Console.WriteLine("Font Source Type: " + fontSource.Type);
            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Text");

            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont";
            cell.SetStyle(style);

            workbook.Save("FileFontSourceExample.xlsx");
        }
    }
}
```

### Ver también

* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


