---
title: "Enumeración PaneStateType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.PaneStateType enum. Representa el estado del panel de las hojas"
type: docs
url: /es/net/aspose.cells/panestatetype/
---
## PaneStateType enumeration

Representa el estado del panel de la hoja.

```csharp
public enum PaneStateType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Frozen | `0` | Los paneles están congelados, pero no lo estaban antes de congelarse. |
| FrozenSplit | `1` | Los paneles están congelados y se dividieron antes de congelarse. |
| Split | `2` | Los paneles están divididos, pero no congelados. |
| Normal | `3` | Los paneles no están congelados ni divididos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PaneStateTypeDemo
    {
        public static void PaneStateTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer algunos datos de ejemplo en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Data 1");
            worksheet.Cells["A2"].PutValue("Data 2");
            worksheet.Cells["A3"].PutValue("Data 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Congelar paneles en la celda B2
            worksheet.FreezePanes(1, 0, 1, 1); // Freeze the first row and first column

            // Verificar el estado del panel
            PaneStateType paneState = worksheet.PaneState;

            // Mostrar el estado del panel
            Console.WriteLine("Current Pane State: " + paneState);

            // Guarda el libro de trabajo
            workbook.Save("PaneStateTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


