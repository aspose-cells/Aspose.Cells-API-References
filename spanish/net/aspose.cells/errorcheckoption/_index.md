---
title: "Clase ErrorCheckOption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ErrorCheckOption. Configuración de verificación de errores aplicada a ciertos rangos"
type: docs
url: /es/net/aspose.cells/errorcheckoption/
---
## ErrorCheckOption class

Configuración de verificación de errores aplicada a ciertos rangos.

```csharp
public class ErrorCheckOption
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddRange](../../aspose.cells/errorcheckoption/addrange/)(CellArea) | Añade un rango influenciado por esta configuración. |
| [GetCountOfRange](../../aspose.cells/errorcheckoption/getcountofrange/)() | Obtiene el recuento de rangos influenciados por esta configuración. |
| [GetRange](../../aspose.cells/errorcheckoption/getrange/)(int) | Obtiene el rango influenciado de esta configuración por el índice dado. |
| [IsErrorCheck](../../aspose.cells/errorcheckoption/iserrorcheck/)(ErrorCheckType) | Comprueba si el tipo de error dado será verificado. |
| [RemoveRange](../../aspose.cells/errorcheckoption/removerange/)(int) | Elimina un rango por el índice dado. |
| [SetErrorCheck](../../aspose.cells/errorcheckoption/seterrorcheck/)(ErrorCheckType, bool) | Establece si el tipo de error dado será verificado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionDemo
    {
        public static void ErrorCheckOptionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la ErrorCheckOptionCollection de la hoja de cálculo
            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;

            // Agregar una nueva ErrorCheckOption a la colección
            int optionIdx = opts.Add();
            ErrorCheckOption opt = opts[optionIdx];

            // Establecer opciones de comprobación de errores
            opt.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            opt.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            opt.SetErrorCheck(ErrorCheckType.TextDate, false);
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.SetErrorCheck(ErrorCheckType.Validation, false);

            // Definir un área de celdas y agregarla a la ErrorCheckOption
            CellArea ca = CellArea.CreateCellArea("A1", "B10");
            opt.AddRange(ca);

            // Guarda el libro de trabajo
            workbook.Save("ErrorCheckOptionExample.xlsx");
            workbook.Save("ErrorCheckOptionExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


