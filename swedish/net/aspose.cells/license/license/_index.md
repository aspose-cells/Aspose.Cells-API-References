---
title: "License.License"
second_title: "Aspose.Cells för .NET API‑referens"
description: "License‑konstruktor. Initierar en ny instans av denna klass"
type: docs
url: /sv/net/aspose.cells/license/license/
---
## License constructor

Initierar en ny instans av denna klass.

```csharp
public License()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LicenseMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny instans av License med hjälp av konstruktorn (#ctor)
            License license = new License();
            
            // Ange licensfilen
            license.SetLicense("MyLicense.lic");
            
            Console.WriteLine("License set successfully.");
        }
    }
}
```

### Se även

* class [License](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


