---
title: "Classe AbstractLowCodeLoadOptionsProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.AbstractLowCodeLoadOptionsProvider. Implémentation pour fournir plusieurs options de chargement pour les processus qui utilisent plusieurs entrées telles que les fichiers modèle"
type: docs
url: /fr/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/
---
## AbstractLowCodeLoadOptionsProvider class

Implémentation pour fournir plusieurs options de chargement pour les processus qui utilisent plusieurs entrées (comme les fichiers de modèle).

```csharp
public abstract class AbstractLowCodeLoadOptionsProvider
```

## Propriétés

| Nom | Description |
| --- | --- |
| abstract [Current](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/) { get; } | Obtient les options de chargement à partir desquelles charger les données de la partie actuellement traitée. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/)(LowCodeLoadOptions) | Libère les ressources après le traitement de la partie actuelle de l'entrée. |
| abstract [MoveNext](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/)() | Vérifie s'il y a plus d'entrée. |

### Remarques

Par exemple, la fonctionnalité [`SpreadsheetMerger`](../spreadsheetmerger/) nécessite plusieurs fichiers modèle à fusionner.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // Créer une implémentation personnalisée de AbstractLowCodeLoadOptionsProvider
            var provider = new CustomLoadOptionsProvider();

            // Traiter plusieurs entrées en utilisant le fournisseur
            while (provider.MoveNext())
            {
                // Obtenir les options de chargement actuelles
                LowCodeLoadOptions currentOptions = provider.Current;
                Console.WriteLine($"Processing with load options: {currentOptions}");

                // Créer un classeur avec les options actuelles
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                Worksheet worksheet = workbook.Worksheets[0];

                // Démontrer l'utilisation avec le classeur
                worksheet.Cells["A1"].PutValue("Processed with custom provider");
                
                // Terminer le traitement de cette partie
                provider.Finish(currentOptions);
            }
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int currentIndex = 0;
            private readonly LowCodeLoadOptions[] optionsList = new LowCodeLoadOptions[]
            {
                new LowCodeLoadOptions(),
                new LowCodeLoadOptions { InputFile = "protected.xlsx" }, // Password would be handled separately
                new LowCodeLoadOptions() // MemorySetting would be handled separately
            };

            public override LowCodeLoadOptions Current => optionsList[currentIndex];

            public override bool MoveNext()
            {
                if (currentIndex < optionsList.Length - 1)
                {
                    currentIndex++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // Logique de nettoyage ou de finalisation pour chaque partie
                Console.WriteLine($"Finished processing part {currentIndex}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


