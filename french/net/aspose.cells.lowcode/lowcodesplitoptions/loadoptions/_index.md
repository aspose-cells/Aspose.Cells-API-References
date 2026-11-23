---
title: "LowCodeSplitOptions.LoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSplitOptions. Options de chargement pour charger la feuille de calcul qui sera divisée"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesplitoptions/loadoptions/
---
## LowCodeSplitOptions.LoadOptions property

Options de chargement pour charger le tableur qui sera divisé.

```csharp
public LowCodeLoadOptions LoadOptions { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertyLoadOptionsDemo
    {
        public static void Run()
        {
            // Créez une instance d'options de division
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Initialiser les options de chargement
            splitOptions.LoadOptions = new LowCodeLoadOptions();

            // Créez de nouvelles options de chargement avec des paramètres différents (en utilisant les propriétés disponibles)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Démontrez la configuration finale
            Console.WriteLine("LoadOptions configured with InputFile: " + splitOptions.LoadOptions.InputFile);
        }
    }
}
```

### Voir aussi

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


