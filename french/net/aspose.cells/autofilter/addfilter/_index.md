---
title: "AutoFilter.AddFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AutoFilter. Ajoute un filtre pour une colonne de filtre"
type: docs
url: /fr/net/aspose.cells/autofilter/addfilter/
---
## AutoFilter.AddFilter method

Ajoute un filtre pour une colonne de filtre.

```csharp
public void AddFilter(int fieldIndex, string criteria)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| critères | String | Le critère spécifié (une chaîne ; par exemple, "101"). Il ne peut être nul ou être l'une des valeurs des cellules de cette colonne. |

### Remarques

MS Excel 2007 prend en charge la sélection multiple dans une colonne de filtre.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["A5"].PutValue("Date");
            worksheet.Cells["A6"].PutValue("Elderberry");
            
            // Créer une plage de filtre automatique
            worksheet.AutoFilter.Range = "A1:A6";
            
            // Obtenir le filtre automatique
            AutoFilter filter = worksheet.AutoFilter;
            
            // Ajouter des filtres pour les valeurs commençant par 'A' et 'E'
            filter.AddFilter(0, "A*");
            filter.AddFilter(0, "E*");
            
            // Actualiser le filtre
            filter.Refresh();
            
            // Enregistrez le classeur
            workbook.Save("AutoFilterAddFilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


