---
title: "Metered.Metered"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur Metered. Initialise une nouvelle instance de cette classe"
type: docs
url: /fr/net/aspose.cells/metered/metered/
---
## Metered constructor

Initialise une nouvelle instance de cette classe.

```csharp
public Metered()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodCtorDemo
    {
        public static void Run()
        {
            // Créez une instance en utilisant le constructeur
            Metered metered = new Metered();

            // Définir la licence metered
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // Créer un classeur simple pour démontrer la fonctionnalité
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Metered License Demo");
            
            // Enregistrez le classeur
            workbook.Save("MeteredDemoOutput.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### Voir aussi

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


