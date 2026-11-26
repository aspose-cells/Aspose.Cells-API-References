---
title: "CopyOptions.CopyInvalidFormulasAsValues"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CopyOptions. Si la fórmula no es válida para el destino, solo copie los valores"
type: docs
url: /es/net/aspose.cells/copyoptions/copyinvalidformulasasvalues/
---
## CopyOptions.CopyInvalidFormulasAsValues property

Si la fórmula no es válida para el destino, solo copiar valores.

```csharp
public bool CopyInvalidFormulasAsValues { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyInvalidFormulasAsValuesDemo
    {
        public static void Run()
        {
            // Cree un libro de origen con una hoja de cálculo de ejemplo
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Agregue una fórmula que podría ser inválida en algunos contextos
            srcSheet.Cells["A1"].Formula = "=1/0"; // Division by zero - invalid formula
            srcSheet.Cells["A2"].Value = "Valid Data";

            // Cree un libro de trabajo de destino
            Workbook destWorkbook = new Workbook();
            
            // Establezca las opciones de copia para convertir fórmulas inválidas en valores
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.CopyInvalidFormulasAsValues = true;

            // Copie la hoja de cálculo con las opciones
            destWorkbook.Worksheets[0].Copy(srcSheet, copyOptions);

            // Verifique los resultados
            Console.WriteLine("A1 (invalid formula copied as value): " + 
                destWorkbook.Worksheets[0].Cells["A1"].Value); // Should show #DIV/0! as value
            Console.WriteLine("A2 (valid data): " + 
                destWorkbook.Worksheets[0].Cells["A2"].Value); // Should show "Valid Data"
        }
    }
}
```

### Ver también

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


