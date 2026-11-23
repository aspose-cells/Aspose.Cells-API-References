---
title: "LoadOptions.CheckExcelRestriction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Indique si la restriction du fichier Excel doit être vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple via Cell.PutValuestring, si cette propriété est vraie vous obtiendrez une exception. Si cette propriété est fausse, nous accepterons votre chaîne d'entrée comme valeur de la cellule, de sorte que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, il peut y avoir des erreurs inattendues dans le fichier Excel généré."
type: docs
url: /fr/net/aspose.cells/loadoptions/checkexcelrestriction/
---
## LoadOptions.CheckExcelRestriction property

Indique si la restriction du fichier Excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une Exception. Si cette propriété est fausse, nous accepterons votre chaîne d'entrée comme valeur de la cellule, de sorte que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, des erreurs inattendues peuvent survenir dans le fichier Excel généré.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Désactiver la vérification des restrictions Excel
            workbook.Settings.CheckExcelRestriction = false;

            // Accéder à la première feuille de calcul et aux cellules
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Créer une chaîne plus longue que la limite normale d'Excel (32767 caractères)
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // Placer la chaîne longue dans la cellule A1
            cells["A1"].PutValue(longString);
            
            // Enregistrer avec la vérification des restrictions désactivée
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;
            workbook.Save("output.xlsx", saveOptions);
            
            // Charger avec la vérification des restrictions désactivée
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output.xlsx", loadOptions);
            
            // Vérifier que la chaîne longue a été conservée
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("String length: " + loadedValue.Length);
            Console.WriteLine("String matches: " + loadedValue.Equals(longString));
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


