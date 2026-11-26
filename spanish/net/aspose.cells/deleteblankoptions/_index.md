---
title: "Clase DeleteBlankOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.DeleteBlankOptions class. Representa la configuración para eliminar celdas/filas/columnas en blanco."
type: docs
url: /es/net/aspose.cells/deleteblankoptions/
---
## DeleteBlankOptions class

Representa la configuración para eliminar celdas/filas/columnas en blanco.

```csharp
public class DeleteBlankOptions : DeleteOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [DeleteBlankOptions](deleteblankoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DrawingsAsBlank](../../aspose.cells/deleteblankoptions/drawingsasblank/) { get; set; } | Indica si los objetos relacionados con dibujos, como imágenes, formas, gráficos..., se considerarán en blanco. El valor predeterminado es true. |
| [EmptyFormulaValueAsBlank](../../aspose.cells/deleteblankoptions/emptyformulavalueasblank/) { get; set; } | Si una celda se considerará en blanco cuando es una fórmula y el resultado calculado es nulo o cadena vacía. El valor predeterminado es false. |
| [EmptyStringAsBlank](../../aspose.cells/deleteblankoptions/emptystringasblank/) { get; set; } | Indica si una celda se considerará en blanco cuando su valor es una cadena vacía. El valor predeterminado es true. |
| [EndIndex](../../aspose.cells/deleteblankoptions/endindex/) { get; set; } | Especifica el índice final de fila/columna (inclusive) del rango a comprobar y eliminar filas/columnas en blanco. El valor predeterminado es -1 y -1 significa el rango máximo de todos los objetos (celdas, dibujos, ...) que deben verificarse. |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Obtiene/establece el monitor para rastrear cambios causados por la eliminación.(Heredado de [`DeleteOptions`](../deleteoptions/).) |
| [MergedCellsShrinkType](../../aspose.cells/deleteblankoptions/mergedcellsshrinktype/) { get; set; } | Indica cómo procesar celdas combinadas al eliminar filas/columnas en blanco. |
| [StartIndex](../../aspose.cells/deleteblankoptions/startindex/) { get; set; } | Especifica el índice inicial de fila/columna del rango a comprobar y eliminar fila/columna en blanco. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Indica si actualizar referencias en otras hojas de cálculo.(Heredado de [`DeleteOptions`](../deleteoptions/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteBlankOptionsDemo
    {
        public static void DeleteBlankOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar la hoja de cálculo con algunos datos
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // Crear una instancia de DeleteBlankOptions
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true,
                EmptyFormulaValueAsBlank = false,
                UpdateReference = true
            };

            // Eliminar filas en blanco según las opciones
            worksheet.Cells.DeleteBlankRows(options);

            // Guarda el libro de trabajo
            workbook.Save("DeleteBlankOptionsExample.xlsx");
            workbook.Save("DeleteBlankOptionsExample.pdf");
            return;
        }
    }
}
```

### Ver también

* class [DeleteOptions](../deleteoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


