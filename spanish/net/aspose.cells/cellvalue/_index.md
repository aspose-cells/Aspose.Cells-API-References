---
title: "Clase CellValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CellValue. Representa el valor de la celda y su tipo correspondiente"
type: docs
url: /es/net/aspose.cells/cellvalue/
---
## CellValue class

Representa el valor de la celda y su tipo correspondiente.

```csharp
public class CellValue
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CellValue](cellvalue/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Type](../../aspose.cells/cellvalue/type/) { get; set; } | Obtiene o establece el tipo de valor de celda. |
| [Value](../../aspose.cells/cellvalue/value/) { get; set; } | Obtiene o establece el valor de la celda. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueDemo
    {
        public static void CellValueExample()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de CellValue
            CellValue cellValue = new CellValue();

            // Establecer el tipo y el valor de la celda
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            // Asignar el CellValue a una celda en la hoja de cálculo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(cellValue.Value);

            // Guarda el libro de trabajo
            workbook.Save("CellValueExample.xlsx");
            workbook.Save("CellValueExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


