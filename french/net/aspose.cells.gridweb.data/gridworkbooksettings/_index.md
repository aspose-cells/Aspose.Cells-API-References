---
title: "Classe GridWorkbookSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.GridWorkbookSettings. Représente les paramètres du classeur"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridworkbooksettings/
---
## GridWorkbookSettings class

Représente les paramètres du classeur.

```csharp
public class GridWorkbookSettings : ISerializable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | constructeur par défaut |

## Propriétés

| Nom | Description |
| --- | --- |
| [Author](../../aspose.cells.gridweb.data/gridworkbooksettings/author/) { get; set; } | Obtient et définit l'auteur du fichier. |
| [CheckCustomNumberFormat](../../aspose.cells.gridweb.data/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Obtient ou définit si la vérification du format de nombre personnalisé est effectuée lors du réglage de Style.Custom. |
| [CreateCalcChain](../../aspose.cells.gridweb.data/gridworkbooksettings/createcalcchain/) { get; set; } | Obtient ou définit si une chaîne de formules calculées est créée. La valeur par défaut est false. |
| [Date1904](../../aspose.cells.gridweb.data/gridworkbooksettings/date1904/) { get; set; } | Obtient ou définit la valeur qui indique si le classeur utilise le système de dates 1904. |
| [EnableMacros](../../aspose.cells.gridweb.data/gridworkbooksettings/enablemacros/) { get; set; } | Obtient ou définit si les macros sont activées ; maintenant cela ne fonctionne que lors de la copie d’une feuille de calcul vers une autre feuille dans un classeur. |
| [ForceFullCalculate](../../aspose.cells.gridweb.data/gridworkbooksettings/forcefullcalculate/) { get; set; } | Obtient ou définit si le calcul est effectué complètement à chaque déclenchement d’un calcul. |
| [Iteration](../../aspose.cells.gridweb.data/gridworkbooksettings/iteration/) { get; set; } | Obtient ou définit si l’itération est utilisée pour résoudre les références circulaires. |
| [MaxIteration](../../aspose.cells.gridweb.data/gridworkbooksettings/maxiteration/) { get; set; } | Obtient ou définit le nombre maximal d’itérations pour résoudre une référence circulaire, la valeur par défaut est 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridweb.data/gridworkbooksettings/precisionasdisplayed/) { get; set; } | Vrai si les calculs dans ce classeur sont effectués en utilisant uniquement la précision des nombres tels qu’ils sont affichés |
| [PreservePaddingSpaces](../../aspose.cells.gridweb.data/gridworkbooksettings/preservepaddingspaces/) { get; set; } | Indique s'il faut conserver les espaces et les sauts de ligne qui sont insérés entre les jetons de formule lors de l'obtention et de la définition des formules. La valeur par défaut est false. |
| [ReCalculateOnOpen](../../aspose.cells.gridweb.data/gridworkbooksettings/recalculateonopen/) { get; set; } | Obtient ou définit si toutes les formules sont recalculées à l’ouverture du fichier. |

### Exemples

```csharp
[C#]

 
GridWeb gridweb = new GridWeb();
GridWorkbookSettings gsettings = new GridWorkbookSettings();
gridweb.Settings=gsettings;

//faites votre travail

[Visual Basic]


Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 gridweb.Settings=gsettings;
 
'do your business
```

### Voir aussi

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


