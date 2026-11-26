---
title: "ErrorCheckOption.IsErrorCheck"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ErrorCheckOption. Verifica si el tipo de error dado será verificado"
type: docs
url: /es/net/aspose.cells/errorcheckoption/iserrorcheck/
---
## ErrorCheckOption.IsErrorCheck method

Comprueba si el tipo de error dado será verificado.

```csharp
public bool IsErrorCheck(ErrorCheckType errorCheckType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | el tipo de error puede ser verificado |

### Valor de retorno

devuelve true si el tipo de error dado será verificado (se mostrará un triángulo verde en la celda si la verificación falla).

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodIsErrorCheckWithErrorCheckTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            int index = options.Add();
            ErrorCheckOption option = options[index];

            // Configurar ajustes de verificación de errores
            option.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            option.SetErrorCheck(ErrorCheckType.EvaluationError, true);
            option.SetErrorCheck(ErrorCheckType.InconsistRange, false);

            // Agregar rango para aplicar estas configuraciones
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 10;
            area.StartColumn = 0;
            area.EndColumn = 5;
            option.AddRange(area);

            // Verificar y mostrar la configuración
            Console.WriteLine("NumberStoredAsText check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.NumberStoredAsText));
            Console.WriteLine("EvaluationError check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.EvaluationError));
            Console.WriteLine("InconsistRange check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.InconsistRange));
        }
    }
}
```

### Ver también

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


