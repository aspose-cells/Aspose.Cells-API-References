---
title: "WorksheetCollection.GetSheetByCodeName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorksheetCollection. Obtient la feuille de calcul par le nom de code"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/getsheetbycodename/
---
## WorksheetCollection.GetSheetByCodeName method

Obtient la feuille de calcul par son nom de code.

```csharp
public Worksheet GetSheetByCodeName(string codeName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| codeName | String | Nom de code de la feuille de calcul. |

### Valeur de retour

L'élément avec le nom de code spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetSheetByCodeNameWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter des feuilles de calcul et définir leurs noms de code
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            sheet1.CodeName = "MainSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.CodeName = "DataSheet";

            // Obtenir la feuille de calcul par le nom de code
            Worksheet mainSheet = workbook.Worksheets.GetSheetByCodeName("MainSheet");
            Worksheet dataSheet = workbook.Worksheets.GetSheetByCodeName("DataSheet");

            // Démontrer l'utilisation en écrivant dans les cellules
            mainSheet.Cells["A1"].PutValue("This is Main Sheet");
            dataSheet.Cells["A1"].PutValue("This is Data Sheet");

            // Enregistrez le classeur
            workbook.Save("GetSheetByCodeNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


