---
title: "AutoFilter.ShowAll"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AutoFilter. Affiche toutes les lignes"
type: docs
url: /fr/net/aspose.cells/autofilter/showall/
---
## AutoFilter.ShowAll method

Afficher toutes les lignes.

```csharp
public void ShowAll()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodShowAllDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            
            // Appliquer le filtre automatique
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Filtrer pour n'afficher que "Apple"
            worksheet.AutoFilter.Filter(0, "Apple");
            
            // Afficher à nouveau toutes les données
            worksheet.AutoFilter.ShowAll();
            
            // Enregistrez le classeur
            workbook.Save("ShowAllDemoOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


