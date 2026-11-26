---
title: "VbaProject.IsSigned"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProject. Indica si el código VBA está firmado o no"
type: docs
url: /es/net/aspose.cells.vba/vbaproject/issigned/
---
## VbaProject.IsSigned property

Indica si VBAcode está firmado o no.

```csharp
public bool IsSigned { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsSignedDemo
    {
        public static void Run()
        {
            // Cargar un archivo de Excel de ejemplo con proyecto VBA
            Workbook workbook = new Workbook("example.xlsm");
            
            // Verificar si el proyecto VBA está firmado
            if (workbook.VbaProject.IsSigned)
            {
                Console.WriteLine("VBA project is signed.");
                Console.WriteLine("Signature is valid: " + workbook.VbaProject.IsValidSigned);
            }
            else
            {
                Console.WriteLine("VBA project is not signed.");
            }
        }
    }
}
```

### Ver también

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


