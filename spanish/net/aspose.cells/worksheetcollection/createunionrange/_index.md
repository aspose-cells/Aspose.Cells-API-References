---
title: "WorksheetCollection.CreateUnionRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Crea un objeto Range a partir de una dirección del rango"
type: docs
url: /es/net/aspose.cells/worksheetcollection/createunionrange/
---
## WorksheetCollection.CreateUnionRange method

Crea un objeto [`Range`](../../range/) a partir de una dirección del rango.

```csharp
public UnionRange CreateUnionRange(string address, int sheetIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| address | String | La dirección del rango. |
| sheetIndex | Int32 | El índice de la hoja. |

### Valor de retorno

Un objeto [`Range`](../../range/)

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateUnionRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un rango de unión a partir de cadenas de direcciones
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Establece el valor para todo el rango de unión
            unionRange.Value = "Test";
            
            // Aplicar estilo al rango de unión
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Font.IsBold = true;
            unionRange.ApplyStyle(style, new StyleFlag { FontBold = true, FontColor = true });
            
            // Guarda el libro de trabajo
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [UnionRange](../../unionrange/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


