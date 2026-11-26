---
title: "Clase PasteOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.PasteOptions. Representa las opciones de pegado especial"
type: docs
url: /es/net/aspose.cells/pasteoptions/
---
## PasteOptions class

Representa las opciones de pegado especial.

```csharp
public class PasteOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PasteOptions](pasteoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IgnoreLinksToOriginalFile](../../aspose.cells/pasteoptions/ignorelinkstooriginalfile/) { get; set; } | Ignorar enlaces al archivo original. |
| [KeepOldTables](../../aspose.cells/pasteoptions/keepoldtables/) { get; set; } | Mantiene las tablas en el rango de destino. |
| [OnlyVisibleCells](../../aspose.cells/pasteoptions/onlyvisiblecells/) { get; set; } | True indica que solo se copian celdas visibles. |
| [OperationType](../../aspose.cells/pasteoptions/operationtype/) { get; set; } | Obtiene y establece el tipo de operación al pegar el rango. |
| [PasteType](../../aspose.cells/pasteoptions/pastetype/) { get; set; } | El tipo de pegado especial. |
| [ShiftFormulasOfShapes](../../aspose.cells/pasteoptions/shiftformulasofshapes/) { get; set; } | Indica si se deben desplazar las fórmulas de las formas al copiar rangos. |
| [SkipBlanks](../../aspose.cells/pasteoptions/skipblanks/) { get; set; } | Indica si se omiten celdas en blanco. |
| [Transpose](../../aspose.cells/pasteoptions/transpose/) { get; set; } | True para transponer filas y columnas cuando se pega el rango. El valor predeterminado es False. |

### Ejemplos

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsDemo
    {
        public static void PasteOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos a la primera hoja de cálculo
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].PutValue(123);

            // Crear otra hoja de cálculo
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");

            // Defina el rango de origen
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1:A3");

            // Defina el rango de destino
            Aspose.Cells.Range destRange = sheet2.Cells.CreateRange("B1:B3");

            // Crear objeto PasteOptions
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                OperationType = PasteOperationType.None,
                IgnoreLinksToOriginalFile = true
            };

            // Copiar el rango con las opciones de pegado especificadas
            destRange.Copy(sourceRange, pasteOptions);

            // Guarda el libro de trabajo
            workbook.Save("PasteOptionsExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


