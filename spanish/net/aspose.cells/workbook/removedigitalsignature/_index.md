---
title: "Workbook.RemoveDigitalSignature"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Elimina la firma digital de esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/workbook/removedigitalsignature/
---
## Workbook.RemoveDigitalSignature method

Elimina la firma digital de esta hoja de cálculo.

```csharp
public void RemoveDigitalSignature()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveDigitalSignatureDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con firma digital
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // Guardar con firma digital (en un escenario real esto se firmaría externamente)
            string signedPath = "SignedWorkbook.xlsx";
            book.Save(signedPath, SaveFormat.Xlsx);

            // Cargar el libro de trabajo firmado
            Workbook signedBook = new Workbook(signedPath);
            Console.WriteLine("Workbook is digitally signed: " + signedBook.IsDigitallySigned);

            // Eliminar firma digital
            signedBook.RemoveDigitalSignature();
            string unsignedPath = "UnsignedWorkbook.xlsx";
            signedBook.Save(unsignedPath);

            // Verificar que la firma fue eliminada
            Workbook unsignedBook = new Workbook(unsignedPath);
            Console.WriteLine("After removal, workbook is digitally signed: " + unsignedBook.IsDigitallySigned);
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


