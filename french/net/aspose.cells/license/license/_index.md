---
title: "License.License"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur License. Initialise une nouvelle instance de cette classe"
type: docs
url: /fr/net/aspose.cells/license/license/
---
## License constructor

Initialise une nouvelle instance de cette classe.

```csharp
public License()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LicenseMethodCtorDemo
    {
        public static void Run()
        {
            // Créer une nouvelle instance de License en utilisant le constructeur (#ctor)
            License license = new License();
            
            // Définir le fichier de licence
            license.SetLicense("MyLicense.lic");
            
            Console.WriteLine("License set successfully.");
        }
    }
}
```

### Voir aussi

* class [License](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


