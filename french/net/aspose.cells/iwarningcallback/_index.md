---
title: "Interface IWarningCallback"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Interface Aspose.Cells.IWarningCallback. Interface de rappel d'avertissement"
type: docs
url: /fr/net/aspose.cells/iwarningcallback/
---
## IWarningCallback interface

Interface de rappel d'avertissement.

```csharp
public interface IWarningCallback
```

## Méthodes

| Nom | Description |
| --- | --- |
| [Warning](../../aspose.cells/iwarningcallback/warning/)(WarningInfo) | Notre rappel n'a besoin d'implémenter que la méthode "Warning". |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IWarningCallbackDemo : IWarningCallback
    {
        // Implémentation de la méthode Warning de l'interface IWarningCallback
        public void Warning(WarningInfo warningInfo)
        {
            // Afficher le message d'avertissement
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
        }

        public static void IWarningCallbackExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Définir le rappel d'avertissement
            workbook.Settings.WarningCallback = new IWarningCallbackDemo();

            // Charger un classeur avec des avertissements potentiels
            try
            {
                workbook = new Workbook("example.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception: " + ex.Message);
            }

            // Enregistrez le classeur
            workbook.Save("IWarningCallbackExample.xlsx");
        }
    }

}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


