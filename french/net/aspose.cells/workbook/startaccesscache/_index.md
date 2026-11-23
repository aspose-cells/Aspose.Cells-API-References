---
title: "Workbook.StartAccessCache"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Démarre la session qui utilise des caches pour accéder aux données"
type: docs
url: /fr/net/aspose.cells/workbook/startaccesscache/
---
## Workbook.StartAccessCache method

Démarre la session qui utilise des caches pour accéder aux données.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| opts | AccessCacheOptions | options d'accès aux données |

### Remarques

Si le cache d'accès aux données spécifiées nécessite que certains modèles de données dans la feuille de calcul soient en \"lecture seule\", alors les modèles de données correspondants dans chaque feuille de calcul de ce classeur seront considérés comme en \"lecture seule\" et l'utilisateur ne doit en modifier aucun. Après avoir terminé l'accès aux données, [`CloseAccessCache`](../closeaccesscache/) doit être invoqué avec les mêmes options pour effacer tous les caches et rétablir le mode d'accès normal.

### Exemples

```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ajouter une mise en forme conditionnelle
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            int index = cfc.Add();
            cfc[index].Add(CellArea.CreateCellArea(0, 0, 5, 0),
                FormatConditionType.DuplicateValues, OperatorType.None, null, null);
            
            // Définir le style pour le formatage conditionnel
            Style style = cfc[0][0].Style;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            
            // Ajoutez quelques images intégrées
            Cells cells = sheet.Cells;
            byte[] img1 = File.ReadAllBytes("1.png");
            byte[] img2 = File.ReadAllBytes("2.png");
            cells[0, 0].EmbeddedImage = img1;
            cells[2, 0].EmbeddedImage = img2;
            cells[4, 0].EmbeddedImage = img1;

            // Démarrer le cache d'accès pour de meilleures performances
            wb.StartAccessCache(AccessCacheOptions.All);
            
            // Accédez aux styles de cellules (sera plus rapide grâce au cache)
            Console.WriteLine("A1 Pattern: " + cells[0, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A3 Pattern: " + cells[2, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A5 Pattern: " + cells[4, 0].GetDisplayStyle().Pattern);
            
            // Fermez le cache une fois terminé
            wb.CloseAccessCache(AccessCacheOptions.All);
        }
    }
}
```

### Voir aussi

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


