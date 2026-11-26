---
title: "FontSetting.TextOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontSetting. Devuelve las opciones de texto"
type: docs
url: /es/net/aspose.cells/fontsetting/textoptions/
---
## FontSetting.TextOptions property

Devuelve las opciones de texto.

```csharp
public TextOptions TextOptions { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyTextOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear texto de ejemplo con diferentes secciones de formato
            string part1 = "This is normal text. ";
            string part2 = "This is bold and italic text. ";
            string part3 = "This is normal again. ";
            string part4 = "This is bold text.";
            
            // Combinar todas las partes en una sola celda
            Cell cell = worksheet.Cells["A1"];
            cell.Value = part1 + part2 + part3 + part4;
            
            // Aplicar formato a partes específicas del texto
            int startPos1 = part1.Length;
            int length1 = part2.Length;
            cell.Characters(startPos1, length1).TextOptions.IsBold = true;
            cell.Characters(startPos1, length1).TextOptions.IsItalic = true;
            
            int startPos2 = part1.Length + part2.Length + part3.Length;
            int length2 = part4.Length;
            cell.Characters(startPos2, length2).TextOptions.IsBold = true;
            
            // Guarda el libro de trabajo
            workbook.Save("TextOptionsDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("TextOptions demo completed. File saved.");
        }
    }
}
```

### Ver también

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


