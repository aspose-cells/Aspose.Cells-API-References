---
title: "FindOptions.SetRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FindOptions. Establece el rango buscado"
type: docs
url: /es/net/aspose.cells/findoptions/setrange/
---
## FindOptions.SetRange method

Establece el rango buscado.

```csharp
public void SetRange(CellArea ca)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | CellArea | el rango buscado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsMethodSetRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar algunos datos
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("def");
            worksheet.Cells["C3"].PutValue("abc");
            
            // Crear FindOptions y establecer el rango de búsqueda
            FindOptions rangeOptions = new FindOptions();
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 1;
            cellarea.StartColumn = 1;
            cellarea.EndRow = 3;
            cellarea.EndColumn = 3;
            rangeOptions.SetRange(cellarea);
            
            // Buscar dentro del rango especificado
            rangeOptions.SearchBackward = false;
            Cell foundCell = worksheet.Cells.Find("abc", null, rangeOptions);
            
            Console.WriteLine("Found 'abc' at row: " + foundCell.Row + ", column: " + foundCell.Column);
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


