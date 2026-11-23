---
title: "Classe GridWorkbookSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridJs.GridWorkbookSettings. Représente les paramètres du classeur"
type: docs
url: /fr/net/aspose.cells.gridjs/gridworkbooksettings/
---
## GridWorkbookSettings class

Représente les paramètres du classeur.

```csharp
public class GridWorkbookSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Author](../../aspose.cells.gridjs/gridworkbooksettings/author/) { get; set; } | Obtient/definit l'auteur du fichier. |
| [CheckCustomNumberFormat](../../aspose.cells.gridjs/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Indique si la vérification du format numérique personnalisé lors du réglage de Style.Custom est activée, la valeur par défaut est false. |
| [CheckExcelRestriction](../../aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/) { get; set; } | Indique si la restriction du fichier Excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est true, vous obtiendrez une Exception. Si cette propriété est false, nous accepterons votre chaîne d'entrée comme valeur de la cellule, ce qui vous permettra ensuite d'exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, des erreurs inattendues peuvent survenir dans le fichier Excel généré. La valeur par défaut est false. |
| [CreateCalcChain](../../aspose.cells.gridjs/gridworkbooksettings/createcalcchain/) { get; set; } | Indique si la chaîne de formules calculées est créée. La valeur par défaut est false. |
| [Date1904](../../aspose.cells.gridjs/gridworkbooksettings/date1904/) { get; set; } | Obtient ou définit une valeur indiquant si le workbook utilise le système de dates 1904. |
| [EnableMacros](../../aspose.cells.gridjs/gridworkbooksettings/enablemacros/) { get; set; } | Active les macros ; actuellement cela ne fonctionne que lors de la copie d'une feuille de calcul vers une autre feuille dans un classeur. |
| [ForceFullCalculate](../../aspose.cells.gridjs/gridworkbooksettings/forcefullcalculate/) { get; set; } | Indique si le calcul est effectué complètement à chaque déclenchement d'un calcul. |
| [Iteration](../../aspose.cells.gridjs/gridworkbooksettings/iteration/) { get; set; } | Indique si l'itération est utilisée pour résoudre les références circulaires. |
| [MaxIteration](../../aspose.cells.gridjs/gridworkbooksettings/maxiteration/) { get; set; } | Renvoie ou définit le nombre maximal d'itérations pour résoudre une référence circulaire, la valeur par défaut est 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridjs/gridworkbooksettings/precisionasdisplayed/) { get; set; } | Vrai si les calculs dans ce classeur sont effectués en utilisant uniquement la précision des nombres tels qu’ils sont affichés |
| [ReCalculateOnOpen](../../aspose.cells.gridjs/gridworkbooksettings/recalculateonopen/) { get; set; } | Indique si toutes les formules sont recalculées à l'ouverture du fichier. La valeur par défaut est true. |

### Exemples

```csharp
[C#]

GridJsWorkbook g = new GridJsWorkbook();

GridWorkbookSettings gsettings = new GridWorkbookSettings();
g.Settings=gsettings;

//faites votre travail

[Visual Basic]
Dim g as GridJsWorkbook = new GridJsWorkbook()

Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 g.Settings=gsettings;
 
'do your business
```

### Voir aussi

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


