---
title: "FontSetting.FontSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor FontSetting."
type: docs
url: /es/net/aspose.cells/fontsetting/fontsetting/
---
## FontSetting constructor

```csharp
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | Int32 |  |
| longitud | Int32 |  |
| hojas | WorksheetCollection |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingMethodCtorWithInt32Int32WorksheetCollectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar texto de muestra a la celda
            worksheet.Cells["A1"].PutValue("Hello World");
            
            // Crear configuración de fuente para los primeros 5 caracteres (0-4) en todas las hojas de cálculo
            FontSetting fontSetting = new FontSetting(0, 5, workbook.Worksheets);
            
            // Aplicar formato
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Size = 14;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../../worksheetcollection/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


