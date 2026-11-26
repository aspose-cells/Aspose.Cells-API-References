---
title: "FontSetting.Length"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontSetting. Obtiene la longitud de los caracteres"
type: docs
url: /es/net/aspose.cells/fontsetting/length/
---
## FontSetting.Length property

Obtiene la longitud de los caracteres.

```csharp
public int Length { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyLengthDemo
    {
        public static void Run()
        {
            // Crea un libro de trabajo y accede a su primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue texto a la celda A1
            worksheet.Cells["A1"].PutValue("Hello World");

            // Crea la configuración de fuente para el texto en la celda A1
            FontSetting fontSetting = worksheet.Cells["A1"].Characters(0, 5);
            
            // Demuestra el uso de la propiedad Length
            Console.WriteLine("Original Length: " + fontSetting.Length);
            
            // Modifica la longitud de la configuración de fuente
            fontSetting = worksheet.Cells["A1"].Characters(0, 11);
            Console.WriteLine("Modified Length: " + fontSetting.Length);
            
            // Aplica formato a la configuración de fuente
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Guarda el libro de trabajo
            workbook.Save("FontSettingLengthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


