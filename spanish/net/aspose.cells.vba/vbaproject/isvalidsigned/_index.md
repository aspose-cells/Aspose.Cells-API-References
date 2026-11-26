---
title: "VbaProject.IsValidSigned"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProject. Indica si la firma del proyecto VBA es válida o no"
type: docs
url: /es/net/aspose.cells.vba/vbaproject/isvalidsigned/
---
## VbaProject.IsValidSigned property

Indica si la firma del proyecto VBA es válida o no.

```csharp
public bool IsValidSigned { get; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsValidSignedDemo
    {
        public static void Run()
        {
            // Cargar un libro de trabajo de ejemplo con proyecto VBA firmado
            Workbook wb = new Workbook("example.xlsm");
            
            // Verificar si el proyecto VBA está firmado y la firma es válida
            Console.WriteLine("Is VBA Project Signed: " + wb.VbaProject.IsSigned);
            Console.WriteLine("Is Signature Valid: " + wb.VbaProject.IsValidSigned);

            // Guardar y recargar para verificar que la firma persista
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Excel97To2003);
            
            Workbook validateWb = new Workbook(ms);
            Console.WriteLine("After Reload - Is VBA Project Signed: " + validateWb.VbaProject.IsSigned);
            Console.WriteLine("After Reload - Is Signature Valid: " + validateWb.VbaProject.IsValidSigned);
        }
    }
}
```

### Ver también

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


