---
title: "Enumeración SheetType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.SheetType. Especifica el tipo de hoja de cálculo"
type: docs
url: /es/net/aspose.cells/sheettype/
---
## SheetType enumeration

Especifica el tipo de hoja de cálculo.

```csharp
public enum SheetType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| VB | `0` | Módulo Visual Basic |
| Worksheet | `1` |  |
| Chart | `2` | Gráfico |
| BIFF4Macro | `3` | Hoja de macro BIFF4 |
| InternationalMacro | `4` | Hoja macro internacional |
| Other | `5` |  |
| Dialog | `6` | Hoja de trabajo de diálogo |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSheetTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Insertar una nueva hoja de trabajo de tipo Worksheet en el índice 0
            Worksheet newWorksheet = workbook.Worksheets.Insert(0, SheetType.Worksheet);
            
            // Establecer el nombre de la nueva hoja de trabajo
            newWorksheet.Name = "InsertedSheet";
            
            // Acceder a las celdas en la nueva hoja de trabajo y agregar algunos datos
            newWorksheet.Cells["A1"].PutValue("This is a new worksheet");
            
            // Guarda el libro de trabajo
            workbook.Save("SheetTypeDemoOutput.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


