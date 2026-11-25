---
title: "License.License"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore License. Inizializza una nuova istanza di questa classe"
type: docs
url: /it/net/aspose.cells/license/license/
---
## License constructor

Inizializza una nuova istanza di questa classe.

```csharp
public License()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LicenseMethodCtorDemo
    {
        public static void Run()
        {
            // Crea una nuova istanza di License usando il costruttore (#ctor)
            License license = new License();
            
            // Imposta il file di licenza
            license.SetLicense("MyLicense.lic");
            
            Console.WriteLine("License set successfully.");
        }
    }
}
```

### Vedi anche

* class [License](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


