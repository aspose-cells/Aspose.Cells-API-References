---
title: "Classe GridLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridWeb.Data.GridLoadOptions classe. Représente les options de chargement du fichier. Obsolète : cette classe sera obsolète après l'utilisation autonome du DLL de l'API publique des cellules ; à la place, vous pouvez utiliser Aspose.Cells.LodOptions"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridloadoptions/
---
## GridLoadOptions class

Représente les options de chargement du fichier. [Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.LodOptions ")]

```csharp
public class GridLoadOptions : ISerializable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GridLoadOptions](gridloadoptions/)() | Crée une option de chargement du fichier. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | Indique si le filtrage automatique des données est appliqué lors du chargement des fichiers. |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | Vérifier si les données sont valides dans le fichier modèle. |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | Indique si la restriction du fichier Excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une Exception. Si cette propriété est fausse, nous accepterons votre chaîne d'entrée comme valeur de la cellule, de sorte que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, des erreurs inattendues peuvent survenir dans le fichier Excel généré. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | Indique s'il faut conserver les données non analysées en mémoire pour le Workbook lorsqu'il est chargé à partir d'un fichier modèle. La valeur par défaut est vraie. |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | Indique si l'ajustement ne concerne que les lignes dont la hauteur n'est pas personnalisée. |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | Indique s'il faut analyser la formule lors de la lecture du fichier. |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | Indique s'il faut analyser les enregistrements mis en cache du tableau croisé dynamique lors du chargement du fichier. La valeur par défaut est false. |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | Obtient et définit le mot de passe du classeur. |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | Indique s'il faut conserver les espaces et les sauts de ligne qui sont insérés entre les jetons de formule lors de l'obtention et de la définition des formules. La valeur par défaut est false. |

### Voir aussi

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


