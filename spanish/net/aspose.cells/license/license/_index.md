---
title: "License.License"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor License. Inicializa una nueva instancia de esta clase"
type: docs
url: /es/net/aspose.cells/license/license/
---
## License constructor

Inicializa una nueva instancia de esta clase.

```csharp
public License()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LicenseMethodCtorDemo
    {
        public static void Run()
        {
            // Crear una nueva instancia de License usando el constructor (#ctor)
            License license = new License();
            
            // Establecer el archivo de licencia
            license.SetLicense("MyLicense.lic");
            
            Console.WriteLine("License set successfully.");
        }
    }
}
```

### Ver también

* class [License](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


