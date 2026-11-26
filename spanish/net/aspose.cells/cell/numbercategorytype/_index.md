---
title: "Cell.NumberCategoryType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Representa el tipo de categoría del formato numérico de esta celda"
type: docs
url: /es/net/aspose.cells/cell/numbercategorytype/
---
## Cell.NumberCategoryType property

Representa el tipo de categoría del formato numérico de esta celda.

```csharp
public NumberCategoryType NumberCategoryType { get; }
```

### Observaciones

Cuando el patrón de formato de la celda se combina con patrones de formato condicional, el tipo devuelto corresponde a la parte que se utiliza para el valor actual de esta celda. Por ejemplo, si el patrón de formato para esta celda es "#,##0;(#,##0);"-";@", entonces cuando el valor de la celda es numérico y distinto de 0, el tipo devuelto es Number; cuando el valor de la celda es 0 o no es un valor numérico, el tipo devuelto es Text.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyNumberCategoryTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un valor de fecha a la celda A1
            Cell dateCell = worksheet.Cells["A1"];
            dateCell.PutValue(DateTime.Now);
            
            // Establecer formato de fecha
            Style dateStyle = dateCell.GetStyle();
            dateStyle.Custom = "yyyy-mm-dd";
            dateCell.SetStyle(dateStyle);
            
            // Agregar un valor numérico a la celda A2
            Cell numberCell = worksheet.Cells["A2"];
            numberCell.PutValue(1234.56);
            
            // Agregar un valor de texto a la celda A3
            Cell textCell = worksheet.Cells["A3"];
            textCell.PutValue("Sample Text");
            
            // Mostrar NumberCategoryType para cada celda
            Console.WriteLine("A1 (Date) NumberCategoryType: " + dateCell.NumberCategoryType);
            Console.WriteLine("A2 (Number) NumberCategoryType: " + numberCell.NumberCategoryType);
            Console.WriteLine("A3 (Text) NumberCategoryType: " + textCell.NumberCategoryType);
            
            // Cambiar A2 a formato de moneda y verificar NumberCategoryType
            Style currencyStyle = numberCell.GetStyle();
            currencyStyle.Custom = "$#,##0.00";
            numberCell.SetStyle(currencyStyle);
            Console.WriteLine("A2 (Currency) NumberCategoryType: " + numberCell.NumberCategoryType);
        }
    }
}
```

### Ver también

* enum [NumberCategoryType](../../numbercategorytype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


