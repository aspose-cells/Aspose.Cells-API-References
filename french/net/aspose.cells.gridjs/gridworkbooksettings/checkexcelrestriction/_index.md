---
title: "GridWorkbookSettings.CheckExcelRestriction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GridWorkbookSettings. Indique si la restriction du fichier excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple via Cell.PutValuestring, si cette propriété est vraie vous obtiendrez une Exception. Si cette propriété est fausse, nous accepterons votre chaîne d'entrée comme valeur de la cellule afin que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier excel, vous ne devez pas enregistrer le classeur au format excel ultérieurement. Sinon, des erreurs inattendues peuvent survenir dans le fichier excel généré. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/
---
## GridWorkbookSettings.CheckExcelRestriction property

Indique si la restriction du fichier Excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est true, vous obtiendrez une Exception. Si cette propriété est false, nous accepterons votre chaîne d'entrée comme valeur de la cellule, ce qui vous permettra ensuite d'exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, des erreurs inattendues peuvent survenir dans le fichier Excel généré. La valeur par défaut est false.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Voir aussi

* class [GridWorkbookSettings](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


