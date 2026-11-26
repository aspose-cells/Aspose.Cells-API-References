---
title: "Clase DeleteOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.DeleteOptions. Representa la configuración de eliminación de filas/columnas"
type: docs
url: /es/net/aspose.cells/deleteoptions/
---
## DeleteOptions class

Representa la configuración para eliminar filas/columnas.

```csharp
public class DeleteOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [DeleteOptions](deleteoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Obtiene/establece el monitor para rastrear los cambios causados por la eliminación. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Indica si actualizar referencias en otras hojas de cálculo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteOptionsDemo
    {
        public static void DeleteOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            // Mostrar los datos originales
            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Crear DeleteOptions
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Set to true to update references in other worksheets
            };

            // Eliminar la segunda fila (Banana)
            sheet.Cells.DeleteRow(2, options.UpdateReference);

            // Mostrar los datos después de la eliminación
            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Guarda el libro de trabajo
            workbook.Save("DeleteOptionsExample.xlsx");
            workbook.Save("DeleteOptionsExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


