---
title: "Classe GridTxtLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.GridTxtLoadOptions. Représente les options de chargement d’un fichier texte"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridtxtloadoptions/
---
## GridTxtLoadOptions class

Représente les options de chargement d'un fichier texte.

```csharp
[Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.TxtLoadOptions ")]
public class GridTxtLoadOptions : GridLoadOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GridTxtLoadOptions](gridtxtloadoptions/)() | Crée les options de chargement d'un fichier texte. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | Indique si le filtrage automatique des données est appliqué lors du chargement des fichiers. (Hérité de [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | Vérifie si les données sont valides dans le fichier modèle. (Hérité de [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | Indique si la restriction du fichier Excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une Exception. Si cette propriété est fausse, nous accepterons votre chaîne saisie comme valeur de la cellule afin que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une telle valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, des erreurs inattendues peuvent survenir dans le fichier Excel généré. (Hérité de [`GridLoadOptions`](../gridloadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertdatetimedata/) { get; set; } | Obtient ou définit une valeur indiquant si la chaîne du fichier texte est convertie en données de type date. |
| [ConvertNumericData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertnumericdata/) { get; set; } | Obtient ou définit une valeur indiquant si la chaîne du fichier texte est convertie en données numériques. |
| [Encoding](../../aspose.cells.gridweb.data/gridtxtloadoptions/encoding/) { get; set; } | Obtient et définit l'encodage par défaut. S'applique uniquement aux fichiers csv. |
| [ExtendToNextSheet](../../aspose.cells.gridweb.data/gridtxtloadoptions/extendtonextsheet/) { get; set; } | Indique si les données sont étendues à la feuille suivante lorsque les lignes ou colonnes dépassent la limite. Si cette propriété est vraie, les données supplémentaires seront transférées à la feuille suivante derrière la feuille actuelle (si la feuille actuelle est la dernière, une nouvelle feuille sera ajoutée au classeur). Si cette propriété est fausse, les données dépassant la limite seront ignorées. La valeur par défaut est false ; |
| [HasFormula](../../aspose.cells.gridweb.data/gridtxtloadoptions/hasformula/) { get; set; } | Indique si le texte est une formule lorsqu'il commence par "=". |
| [HasTextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/hastextqualifier/) { get; set; } | Indique s'il existe un qualificateur de texte pour la valeur de cellule. La valeur par défaut est true. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier (Hérité de [`GridLoadOptions`](../gridloadoptions/).) |
| [IsMultiEncoded](../../aspose.cells.gridweb.data/gridtxtloadoptions/ismultiencoded/) { get; set; } | True signifie que le fichier contient plusieurs encodages. |
| [KeepPrecision](../../aspose.cells.gridweb.data/gridtxtloadoptions/keepprecision/) { get; set; } | Indique s'il ne faut pas analyser une valeur de chaîne si la longueur est de 15. |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir d'un fichier modèle. La valeur par défaut est true. (Hérité de [`GridLoadOptions`](../gridloadoptions/).) |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | Indique si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées. (Hérité de [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | Indique si la formule est analysée lors de la lecture du fichier. (Hérité de [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | Indique si les enregistrements mis en cache du tableau croisé dynamique sont analysés lors du chargement du fichier. La valeur par défaut est false. (Hérité de [`GridLoadOptions`](../gridloadoptions/).) |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | Obtient et définit le mot de passe du classeur. (Hérité de [`GridLoadOptions`](../gridloadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | Indique si les espaces et sauts de ligne insérés entre les jetons de formule sont conservés lors de l'obtention et de la définition des formules. La valeur par défaut est false. (Hérité de [`GridLoadOptions`](../gridloadoptions/).) |
| [Separator](../../aspose.cells.gridweb.data/gridtxtloadoptions/separator/) { get; set; } | Obtient et définit le séparateur de caractères du fichier texte. |
| [SeparatorString](../../aspose.cells.gridweb.data/gridtxtloadoptions/separatorstring/) { get; set; } | Obtient et définit une valeur chaîne comme séparateur. |
| [TextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/textqualifier/) { get; set; } | Spécifie le qualificateur de texte pour les valeurs de cellule. Le qualificateur par défaut est '\"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | Indique si les délimiteurs consécutifs doivent être traités comme un seul. |
| [TreatQuotePrefixAsValue](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatquoteprefixasvalue/) { get; set; } | Indique si l'apostrophe simple initiale doit être considérée comme faisant partie de la valeur d'une cellule. La valeur par défaut est true. Si elle est false, l'apostrophe initiale sera supprimée de la valeur de la cellule correspondante et [`QuotePrefix`](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) sera définie sur true pour la cellule. |

### Voir aussi

* class [GridLoadOptions](../gridloadoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


