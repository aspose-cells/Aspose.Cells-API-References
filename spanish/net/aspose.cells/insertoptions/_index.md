---
title: "Clase InsertOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.InsertOptions. Representa las opciones de inserción"
type: docs
url: /es/net/aspose.cells/insertoptions/
---
## InsertOptions class

Representa las opciones de inserción.

```csharp
public class InsertOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [InsertOptions](insertoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CopyFormatType](../../aspose.cells/insertoptions/copyformattype/) { get; set; } |  |
| [FormulaChangeMonitor](../../aspose.cells/insertoptions/formulachangemonitor/) { get; set; } | Obtiene/establece el monitor para rastrear los cambios causados por la inserción. |
| [UpdateReference](../../aspose.cells/insertoptions/updatereference/) { get; set; } | Indica si las referencias en otras hojas de cálculo se actualizarán. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InsertOptionsDemo
    {
        public static void InsertOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una instancia de InsertOptions
            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Define el área de celdas donde se insertarán filas
            CellArea cellArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };

            // Inserta filas con las opciones especificadas
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            // Guarda el libro de trabajo
            workbook.Save("InsertOptionsExample.xlsx");
            workbook.Save("InsertOptionsExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


