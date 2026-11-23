---
title: "LoadFilter.StartSheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LoadFilter. Prépare les options de filtre avant de charger la feuille de calcul donnée. L'implémentation par les utilisateurs de LoadFilter peut modifier les LoadDataFilterOptions ici pour indiquer comment charger les données pour cette feuille de calcul."
type: docs
url: /fr/net/aspose.cells/loadfilter/startsheet/
---
## LoadFilter.StartSheet method

Prépare les options de filtre avant de charger la feuille de calcul donnée. L'implémentation de LoadFilter par l'utilisateur peut modifier les LoadDataFilterOptions ici pour indiquer comment charger les données pour cette feuille de calcul.

```csharp
public virtual void StartSheet(Worksheet sheet)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| feuille | Feuille de calcul | La feuille de calcul à charger. Seules quelques propriétés peuvent être utilisées pour l'objet feuille de calcul donné ici car la plupart des données et propriétés n'ont pas été chargées. Les propriétés disponibles sont : Name, Index, VisibilityType |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodStartSheetWithWorksheetDemo
    {
        // Créer une classe de filtre de chargement personnalisée qui étend LoadFilter
        class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                Console.WriteLine($"Processing sheet: {sheet.Name}");
                // Vous pouvez ajouter une logique personnalisée ici pour gérer des feuilles spécifiques
            }
        }

        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "TestSheet";

            // Créer une instance de notre filtre de chargement personnalisé
            CustomLoadFilter loadFilter = new CustomLoadFilter();

            try
            {
                // Appeler la méthode StartSheet avec le paramètre de la feuille de calcul
                loadFilter.StartSheet(worksheet);
                
                Console.WriteLine("StartSheet method executed successfully");
                
                // Ajouter des données pour démontrer que la feuille est accessible
                worksheet.Cells["A1"].PutValue("StartSheet Demo");
                worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("LoadFilterStartSheetDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../worksheet/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


