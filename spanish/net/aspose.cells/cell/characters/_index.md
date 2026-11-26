---
title: "Cell.Characters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Devuelve un objeto Characters que representa un rango de caracteres dentro del texto de la celda"
type: docs
url: /es/net/aspose.cells/cell/characters/
---
## Cell.Characters method

Devuelve un objeto Characters que representa un rango de caracteres dentro del texto de la celda.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | Int32 | El índice del inicio del carácter. |
| longitud | Int32 | El número de caracteres. |

### Valor de retorno

Objeto Characters.

### Observaciones

Este método solo funciona en celdas con valor de cadena.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].PutValue("Helloworld");
            cells["A1"].Characters(5, 5).Font.IsBold = true;
            cells["A1"].Characters(5, 5).Font.Color = Color.Blue;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


