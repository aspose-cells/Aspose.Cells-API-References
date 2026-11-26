---
title: "Font.Charset"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Representa el conjunto de caracteres"
type: docs
url: /es/net/aspose.cells/font/charset/
---
## Font.Charset property

Representa el conjunto de caracteres.

```csharp
public int Charset { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyCharsetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo con propiedades de fuente específicas, incluido el conjunto de caracteres
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Charset = 1; // ANSI_CHARSET

            // Aplicar el estilo a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Text with ANSI charset");

            // Crear otro estilo con un conjunto de caracteres diferente
            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 12;
            style2.Font.Charset = 2; // DEFAULT_CHARSET

            // Aplicar el segundo estilo a otra celda
            Cell cell2 = worksheet.Cells["A2"];
            cell2.SetStyle(style2);
            cell2.PutValue("Text with DEFAULT charset");

            // Guarda el libro de trabajo
            workbook.Save("FontCharsetDemo.xlsx");

            // Verificar las propiedades del conjunto de caracteres
            Console.WriteLine("Cell A1 Font Charset: " + cell.GetStyle().Font.Charset);
            Console.WriteLine("Cell A2 Font Charset: " + cell2.GetStyle().Font.Charset);
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


