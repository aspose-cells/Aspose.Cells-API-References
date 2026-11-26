---
title: "Comment.Characters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Comment. Devuelve un objeto Characters que representa un rango de caracteres dentro del texto del comentario"
type: docs
url: /es/net/aspose.cells/comment/characters/
---
## Comment.Characters method

Devuelve un objeto Characters que representa un rango de caracteres dentro del texto del comentario.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | Int32 | El índice del inicio del carácter. |
| longitud | Int32 | El número de caracteres. |

### Valor de retorno

Objeto Characters.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";
            
            // Obtener la configuración de fuente para los primeros 4 caracteres
            FontSetting fontSetting = comment1.Characters(0, 4);
            
            // Modificar la configuración de fuente
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Guarda el libro de trabajo
            workbook.Save("CommentFontSettingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


