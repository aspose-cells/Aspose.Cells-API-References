---
title: "Workbook.AcceptAllRevisions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Acepta todos los cambios rastreados en el libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbook/acceptallrevisions/
---
## Workbook.AcceptAllRevisions method

Acepta todos los cambios rastreados en el libro de trabajo.

```csharp
public void AcceptAllRevisions()
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAcceptAllRevisionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con revisiones
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunas revisiones (el seguimiento de cambios debe estar habilitado en Excel primero)
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Guardar con revisiones
            string sourcePath = "source_with_revisions.xlsx";
            workbook.Save(sourcePath, SaveFormat.Xlsx);
            
            // Reabrir el libro de trabajo
            workbook = new Workbook(sourcePath);
            
            // Verificar si tiene revisiones y aceptarlas
            if (workbook.HasRevisions)
            {
                Console.WriteLine("Workbook has revisions. Accepting all...");
                workbook.AcceptAllRevisions();
                
                // Guardar sin revisiones
                string destPath = "output_no_revisions.xlsx";
                workbook.Save(destPath, SaveFormat.Xlsx);
                Console.WriteLine("Revisions accepted and saved to: " + destPath);
            }
            else
            {
                Console.WriteLine("Workbook has no revisions.");
            }
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


