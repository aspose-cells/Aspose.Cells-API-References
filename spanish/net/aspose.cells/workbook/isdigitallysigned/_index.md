---
title: "Workbook.IsDigitallySigned"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Workbook property. Indica si esta hoja de cálculo está firmada digitalmente"
type: docs
url: /es/net/aspose.cells/workbook/isdigitallysigned/
---
## Workbook.IsDigitallySigned property

Indica si esta hoja de cálculo está firmada digitalmente.

```csharp
public bool IsDigitallySigned { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsDigitallySignedDemo
    {
        public static void Run()
        {
            // Cargar un libro de trabajo firmado digitalmente
            Workbook book = new Workbook("Test_DigiSign.xlsx");
            
            // Verificar si el libro de trabajo está firmado digitalmente
            bool isSigned = book.IsDigitallySigned;
            Console.WriteLine("Workbook is digitally signed: " + isSigned);

            if (isSigned)
            {
                // Guardar una copia (la firma se conservará)
                book.Save("SignedCopy.xlsx");
                
                // Eliminar la firma digital
                book.RemoveDigitalSignature();
                book.Save("UnsignedCopy.xlsx");
                
                // Verificar que la firma fue eliminada
                Workbook unsignedBook = new Workbook("UnsignedCopy.xlsx");
                Console.WriteLine("After removal, workbook is signed: " + unsignedBook.IsDigitallySigned);
            }
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


