---
title: "AutoFitterOptions.OnlyAuto"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AutoFitterOptions. Indique si seules les lignes dont la hauteur n'est pas personnalisée doivent être ajustées"
type: docs
url: /fr/net/aspose.cells/autofitteroptions/onlyauto/
---
## AutoFitterOptions.OnlyAuto property

Indique si l'ajustement ne concerne que les lignes dont la hauteur n'est pas personnalisée.

```csharp
public bool OnlyAuto { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyOnlyAutoDemo
    {
        public static void Run()
        {
            // Créer des options de chargement et définir la propriété OnlyAuto
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = new AutoFitterOptions();
            loadOptions.AutoFitterOptions.OnlyAuto = true;

            // Charger le classeur avec les options d'ajustement automatique
            Workbook workbook = new Workbook("example.xml", loadOptions);
            
            // Démontrer l'ajustement automatique en vérifiant la largeur de colonne
            Console.WriteLine("Column width after auto-fit: " + 
                workbook.Worksheets[0].Cells.GetColumnWidthPixel(0));
            
            // Enregistrer et recharger pour vérifier la persistance
            workbook.Save("example_output.xlsx");
            Workbook reloaded = new Workbook("example_output.xlsx");
            Console.WriteLine("Reloaded column width: " + 
                reloaded.Worksheets[0].Cells.GetColumnWidthPixel(0));
        }
    }
}
```

### Voir aussi

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


