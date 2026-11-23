---
title: "LoadOptions.MemorySetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Obtient ou définit le mode mémoire pour le classeur chargé"
type: docs
url: /fr/net/aspose.cells/loadoptions/memorysetting/
---
## LoadOptions.MemorySetting property

Obtient ou définit le mode mémoire pour le classeur chargé.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Remarques

Pour plus de détails sur le mode mémoire, veuillez consulter [`MemorySetting`](../../cells/memorysetting/).

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Créer des options de chargement avec le paramètre de préférence mémoire
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;

            // Charger le classeur avec des paramètres optimisés pour la mémoire
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // Accéder à la feuille de calcul et ajouter des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Memory Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Enregistrez le classeur
            workbook.Save("MemorySettingDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with MemoryPreference setting.");
        }
    }
}
```

### Voir aussi

* enum [MemorySetting](../../memorysetting/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


