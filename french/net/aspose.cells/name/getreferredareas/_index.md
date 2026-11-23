---
title: "Name.GetReferredAreas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Name. Obtient toutes les références référencées par ce nom"
type: docs
url: /fr/net/aspose.cells/name/getreferredareas/
---
## Name.GetReferredAreas method

Obtient toutes les références référencées par ce nom.

```csharp
public ReferredArea[] GetReferredAreas(bool recalculate)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| recalculer | Boolean | si le recalcul doit être effectué si ce nom a déjà été calculé avant cet appel. |

### Valeur de retour

Toutes les plages.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetReferredAreasWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook wb = new Workbook();
            
            // Ajouter des données à la feuille de calcul
            wb.Worksheets[0].Cells[3, 3].PutValue("v03");
            
            // Créer une plage nommée avec plusieurs références
            Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")];
            n.RefersTo = "='C:\\[extlink1.xlsx]Sheet1'!$A$1:$B$2,'C:\\[extlink2.xlsx]Sheet2'!$C$3,Sheet1!$D$4,'C:\\[extlink1.xlsx]Sheet1'!E5";
            
            // Obtenir les zones référencées avec des liens externes
            ReferredArea[] ras = n.GetReferredAreas(true);
            
            // Afficher les informations sur chaque zone référencée
            Console.WriteLine("Number of referred areas: " + ras.Length);
            for (int i = 0; i < ras.Length; i++)
            {
                ReferredArea ra = ras[i];
                Console.WriteLine($"\nArea {i + 1}:");
                Console.WriteLine($"IsExternalLink: {ra.IsExternalLink}");
                if (ra.IsExternalLink)
                {
                    Console.WriteLine($"ExternalFileName: {ra.ExternalFileName}");
                }
                Console.WriteLine($"SheetName: {ra.SheetName}");
                Console.WriteLine($"IsArea: {ra.IsArea}");
                
                if (ra.IsArea)
                {
                    Console.WriteLine($"Range: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}" +
                                    $" to {CellsHelper.CellIndexToName(ra.EndRow, ra.EndColumn)}");
                }
                else
                {
                    Console.WriteLine($"Cell: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}");
                }
            }
            
            // Créer un classeur externe et mettre à jour les valeurs
            Workbook wb1 = new Workbook();
            wb1.Worksheets[0].Cells[0, 0].PutValue("v10");
            wb1.Worksheets[0].Cells[1, 1].PutValue("v11");
            wb1.Worksheets[0].Cells[4, 4].PutValue("v14");
            
            // Mettre à jour la source de données liée
            wb.UpdateLinkedDataSource(new Workbook[]{wb1});
            
            // Afficher certaines valeurs des zones référencées
            Console.WriteLine("\nValues from referred areas:");
            Console.WriteLine($"Area1[0,0]: {ras[0].GetValue(0, 0)}");
            Console.WriteLine($"Area1[1,1]: {ras[0].GetValue(1, 1)}");
            Console.WriteLine($"Area3[0,0]: {ras[2].GetValue(0, 0)}");
            Console.WriteLine($"Area4[0,0]: {ras[3].GetValue(0, 0)}");
        }
    }
}
```

### Voir aussi

* class [ReferredArea](../../referredarea/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


