---
title: "GridLoadOptions.CheckExcelRestriction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GridLoadOptions. Indique s'il faut vérifier les restrictions du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas l'entrée d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple via Cell.PutValuestring, si cette propriété est vraie vous obtiendrez une exception. Si cette propriété est fausse, nous accepterons votre chaîne d'entrée comme valeur de la cellule, de sorte que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, il peut y avoir des erreurs inattendues dans le fichier Excel généré."
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/
---
## GridLoadOptions.CheckExcelRestriction property

Indique si la restriction du fichier Excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une Exception. Si cette propriété est fausse, nous accepterons votre chaîne d'entrée comme valeur de la cellule, de sorte que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, des erreurs inattendues peuvent survenir dans le fichier Excel généré.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Voir aussi

* class [GridLoadOptions](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


