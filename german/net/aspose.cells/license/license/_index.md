---
title: "License.License"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "License‑Konstruktor. Initialisiert eine neue Instanz dieser Klasse"
type: docs
url: /de/net/aspose.cells/license/license/
---
## License constructor

Initialisiert eine neue Instanz dieser Klasse.

```csharp
public License()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LicenseMethodCtorDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Instanz von License mithilfe des Konstruktors (#ctor)
            License license = new License();
            
            // Legen Sie die Lizenzdatei fest
            license.SetLicense("MyLicense.lic");
            
            Console.WriteLine("License set successfully.");
        }
    }
}
```

### Siehe auch

* class [License](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


