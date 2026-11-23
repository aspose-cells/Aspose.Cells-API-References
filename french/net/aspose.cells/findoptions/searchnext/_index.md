---
title: "FindOptions.SearchNext"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FindOptions. Ordre de recherche. True recherche suivante. False recherche précédente"
type: docs
url: /fr/net/aspose.cells/findoptions/searchnext/
---
## FindOptions.SearchNext property

Ordre de recherche. True : recherche suivante. False : recherche précédente.

```csharp
[Obsolete("Use FindOptions.SearchBackward property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SearchNext { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété FindOptions.SearchBackward. Cette propriété sera supprimée 12 mois plus tard à compter de novembre 2018. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertySearchNextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données d'exemple
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("apple");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("apple pie");

            // Créer des options de recherche
            FindOptions findOptions = new FindOptions();
            findOptions.CaseSensitive = false;
            findOptions.LookAtType = LookAtType.Contains;

            // Démontrer la propriété SearchNext (obsolète, mais présentée à titre d'exemple)
            Console.WriteLine("Initial SearchNext value: " + findOptions.SearchNext);
            
            // Rechercher en avant (comportement par défaut)
            findOptions.SearchNext = true;
            Cell firstForward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First forward search result: " + (firstForward != null ? firstForward.Name + " - " + firstForward.StringValue : "Not found"));

            // Rechercher en arrière
            findOptions.SearchNext = false;
            Cell firstBackward = worksheet.Cells.Find("apple", null, findOptions);
            Console.WriteLine("First backward search result: " + (firstBackward != null ? firstBackward.Name + " - " + firstBackward.StringValue : "Not found"));

            // Enregistrez le classeur
            workbook.Save("PropertySearchNextDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


