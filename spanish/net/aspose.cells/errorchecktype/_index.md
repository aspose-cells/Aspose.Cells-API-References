---
title: "Enum ErrorCheckType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.ErrorCheckType. Representa todos los tipos de verificación de errores"
type: docs
url: /es/net/aspose.cells/errorchecktype/
---
## ErrorCheckType enumeration

Representa todos los tipos de comprobación de errores.

```csharp
public enum ErrorCheckType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| EvaluationError | `1` | Ignora los errores cuando las celdas contienen fórmulas que producen un error. |
| Calc | `1` |  |
| EmptyCellRef | `2` | Ignorar errores cuando las fórmulas hacen referencia a celdas vacías. |
| NumberStoredAsText | `4` | Ignorar errores cuando los números están formateados como texto o van precedidos por un apóstrofe |
| TextNumber | `4` | Ignorar errores cuando los números están formateados como texto o van precedidos por un apóstrofe |
| InconsistRange | `8` | Ignorar errores cuando las fórmulas omiten ciertas celdas en una región. |
| InconsistFormula | `16` | Ignorar errores cuando una fórmula en una región de su hoja de cálculo difiere de otras fórmulas en la misma región. |
| TwoDigitTextYear | `32` | Ignorar errores cuando las fórmulas contienen celdas con formato de texto y años representados con 2 dígitos. |
| TextDate | `32` | Ignorar errores cuando las fórmulas contienen celdas con formato de texto y años representados con 2 dígitos. |
| UnlockedFormula | `64` | Ignorar errores cuando las celdas desbloqueadas contienen fórmulas. |
| UnproctedFormula | `64` | Ignorar errores cuando las celdas desbloqueadas contienen fórmulas. |
| TableDataValidation | `128` | Ignorar errores cuando el valor de una celda en una Tabla no cumple con las reglas de Validación de Datos especificadas. |
| Validation | `128` | Ignorar errores cuando el valor de una celda en una Tabla no cumple con las reglas de Validación de Datos especificadas. |
| CalculatedColumn | `129` | Ignorar errores cuando las celdas contienen un valor diferente de una fórmula de columna calculada. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckTypeDemo
    {
        public static void ErrorCheckTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la ErrorCheckOptionCollection
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;

            // Agregar una nueva ErrorCheckOption
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];

            // Establecer varios tipos de verificación de errores en false
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.Validation, false);

            // Definir un área de celdas para la opción de verificación de errores
            CellArea cellArea = CellArea.CreateCellArea("A1", "B10");
            errorCheckOption.AddRange(cellArea);

            // Guarda el libro de trabajo
            workbook.Save("ErrorCheckTypeExample.xlsx");
            workbook.Save("ErrorCheckTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


