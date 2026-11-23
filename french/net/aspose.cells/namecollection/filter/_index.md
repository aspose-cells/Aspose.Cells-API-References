---
title: "NameCollection.Filter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode NameCollection. Obtient tous les noms définis par portée"
type: docs
url: /fr/net/aspose.cells/namecollection/filter/
---
## NameCollection.Filter method

Obtient tous les noms définis par portée.

```csharp
public Name[] Filter(NameScopeType type, int sheetIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | NameScopeType | Le type de portée. |
| sheetIndex | Int32 | L'index de la feuille. N'affecte que lorsque le type de portée est Worksheet |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodFilterWithNameScopeTypeInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez quelques noms au classeur et aux feuilles de calcul
            workbook.Worksheets.Names.Add("GlobalName");
            Worksheet worksheet1 = workbook.Worksheets[0];
            workbook.Worksheets.Names.Add("Sheet1Name");
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Names.Add("Sheet2Name");

            // Filtrez les noms par type de portée et index de feuille
            Name[] workbookScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Workbook, -1);
            Name[] worksheetScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1);
            Name[] sheet1Names = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 0);

            // Afficher les résultats
            Console.WriteLine($"Workbook-scoped names count: {workbookScopeNames.Length}");
            Console.WriteLine($"Worksheet-scoped names count: {worksheetScopeNames.Length}");
            Console.WriteLine($"Sheet1 names count: {sheet1Names.Length}");
        }
    }
}
```

### Voir aussi

* class [Name](../../name/)
* enum [NameScopeType](../../namescopetype/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


