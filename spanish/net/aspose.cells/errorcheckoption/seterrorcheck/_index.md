---
title: "ErrorCheckOption.SetErrorCheck"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ErrorCheckOption. Establece si el tipo de error dado será verificado"
type: docs
url: /es/net/aspose.cells/errorcheckoption/seterrorcheck/
---
## ErrorCheckOption.SetErrorCheck method

Establece si el tipo de error dado será verificado.

```csharp
public void SetErrorCheck(ErrorCheckType errorCheckType, bool isCheck)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | el tipo de error puede ser verificado. |
| isCheck | Booleano | true si el tipo de error dado necesita ser verificado (se mostrará un triángulo verde en la celda si la verificación falla). |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodSetErrorCheckWithErrorCheckTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("Sample text for error checking");
            
            // Configurar opciones de verificación de errores
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];
            
            // Demostrar SetErrorCheck con diferentes valores de ErrorCheckType
            errorCheckOption.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, true);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            
            // Aplicar a toda la hoja de cálculo
            errorCheckOption.AddRange(CellArea.CreateCellArea(0, 0, worksheet.Cells.MaxRow, worksheet.Cells.MaxDataColumn));
            
            workbook.Save("ErrorCheckExample.xlsx");
        }
    }
}
```

### Ver también

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


