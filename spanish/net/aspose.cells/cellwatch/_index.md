---
title: "Clase CellWatch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.CellWatch clase. Representa el elemento de vigilancia de celda en la ventana de observación"
type: docs
url: /es/net/aspose.cells/cellwatch/
---
## CellWatch class

Representa el elemento de observación de celda en la 'ventana de observación'.

```csharp
public class CellWatch
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CellWatch](cellwatch/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CellName](../../aspose.cells/cellwatch/cellname/) { get; set; } | Obtiene y establece el nombre de la celda. |
| [Column](../../aspose.cells/cellwatch/column/) { get; set; } | Obtiene y establece la columna de la celda. |
| [Row](../../aspose.cells/cellwatch/row/) { get; set; } | Obtiene y establece la fila de la celda. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchDemo
    {
        public static void CellWatchExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            // Obtenga la primera hoja de cálculo.
            Worksheet sheet = workbook.Worksheets[0];

            // Añadir elemento de vigilancia de celda a la ventana de observación
            int watchIndex = sheet.CellWatches.Add("B2");

            // Recuperar el objeto CellWatch
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Estableciendo propiedades
            cellWatch.Row = 1; // B2 corresponds to row 1 (0-based index)
            cellWatch.Column = 1; // B2 corresponds to column 1 (0-based index)
            cellWatch.CellName = "B2";

            // Guarda el libro de trabajo
            workbook.Save("CellWatchExample.xlsx");
            workbook.Save("CellWatchExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


