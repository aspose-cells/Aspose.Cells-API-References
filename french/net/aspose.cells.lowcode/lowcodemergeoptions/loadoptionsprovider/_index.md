---
title: "LowCodeMergeOptions.LoadOptionsProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeMergeOptions. Fournisseur d'options d'enregistrement pour enregistrer les parties découpées"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/
---
## LowCodeMergeOptions.LoadOptionsProvider property

Fournisseur d'options d'enregistrement pour enregistrer les parties découpées.

```csharp
public AbstractLowCodeLoadOptionsProvider LoadOptionsProvider { get; set; }
```

### Remarques

Si cette propriété est spécifiée, [`LoadOptions`](../../../aspose.cells/loadoptions/) n'a aucun effet car la sortie de chaque partie découpée sera spécifiée par le fournisseur.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeMergeOptionsPropertyLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();

            // Afficher la valeur actuelle de LoadOptionsProvider (devrait être null initialement)
            Console.WriteLine("Current LoadOptionsProvider value: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Créer une implémentation personnalisée de LoadOptionsProvider
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();

            // Démontrer la définition de la propriété
            Console.WriteLine("After setting LoadOptionsProvider: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Utiliser les options de fusion avec le fournisseur
            // Cela serait généralement utilisé avec des méthodes qui traitent plusieurs fichiers
            // À des fins de démonstration, nous vérifierons simplement si le fournisseur peut passer au suivant
            bool hasNext = mergeOptions.LoadOptionsProvider.MoveNext();
            Console.WriteLine("LoadOptionsProvider MoveNext result: " + hasNext);

            // Enregistrez le classeur
            workbook.Save("PropertyLoadOptionsProviderDemo.xlsx");
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int counter = 0;
            private readonly LowCodeLoadOptions options = new LowCodeLoadOptions();

            public override LowCodeLoadOptions Current => options;

            public override bool MoveNext()
            {
                // Simuler la présence de 3 fichiers à traiter
                if (counter < 3)
                {
                    counter++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // La logique de nettoyage ou de finalisation irait ici
            }
        }
    }
}
```

### Voir aussi

* class [AbstractLowCodeLoadOptionsProvider](../../abstractlowcodeloadoptionsprovider/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


