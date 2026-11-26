---
title: "Cell.IsRichText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Indica si el valor de cadena de esta celda es un texto con formato enriquecido"
type: docs
url: /es/net/aspose.cells/cell/isrichtext/
---
## Cell.IsRichText method

Indica si el valor de cadena de esta celda es un texto con formato enriquecido.

```csharp
public bool IsRichText()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodIsRichTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear una celda con formato de texto enriquecido
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello World");
            
            // Aplicar formato de texto enriquecido
            FontSetting boldFont = cell.GetCharacters()[0];
            boldFont.Font.IsBold = true;
            
            FontSetting normalFont = cell.GetCharacters()[6];
            normalFont.Font.IsBold = false;
            
            // Comprobar si la celda contiene texto enriquecido
            bool isRichText = cell.IsRichText();
            Console.WriteLine("Is cell A1 rich text? " + isRichText);
            
            // Guarda el libro de trabajo
            workbook.Save("RichTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


