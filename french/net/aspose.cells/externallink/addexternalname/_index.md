---
title: "ExternalLink.AddExternalName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ExternalLink. Ajoute un nom externe"
type: docs
url: /fr/net/aspose.cells/externallink/addexternalname/
---
## ExternalLink.AddExternalName method

Ajoute un nom externe.

```csharp
public void AddExternalName(string text, string referTo)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| texte | String | Le texte du nom externe. Si le nom externe appartient à une feuille de calcul, le texte doit être sous la forme Sheet1!Text. |
| referTo | String | Le referTo du nom externe. Il doit s'agir d'une cellule ou d'une plage. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkMethodAddExternalNameWithStringStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créer un classeur externe d'exemple
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["B2"].PutValue(67);
            
            // Ajouter un lien externe au classeur principal
            string[] sheetNames = new string[] { externalSheet.Name };
            int index = workbook.Worksheets.ExternalLinks.Add("ExternalWorkbook.xlsx", sheetNames);
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[index];
            
            // Ajouter un nom externe
            externalLink.AddExternalName("Test", "=Sheet1!$B$2");
            
            // Utiliser le nom externe dans une formule
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]!Test";
            
            // Calculer la formule
            workbook.CalculateFormula();
            
            // Afficher le résultat
            Console.WriteLine("Value from external reference: " + sheet.Cells["A1"].DoubleValue);
        }
    }
}
```

### Voir aussi

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


