---
title: GridCell
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente un objet cellule.
type: docs
weight: 150
url: /fr/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

Représente un objet cellule.

```csharp
public class GridCell
```

## Propriétés

| Nom | La description |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue) { get; } | Obtient la valeur booléenne contenue dans la cellule. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column) { get; } | Obtient le numéro de colonne (base zéro) de la cellule. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue) { get; } | Obtient la valeur DateTime contenue dans la cellule. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue) { get; } | Obtient la valeur de chaîne formatée de cette cellule. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue) { get; } | Obtient la valeur double contenue dans la cellule. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue) { get; } | Obtient la valeur flottante contenue dans la cellule. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula) { get; set; } | Obtient ou définit une formule duCell . |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring) { get; set; } | Obtient et définit la chaîne html qui contient des données et certaines mises en forme dans cette cellule. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue) { get; } | Obtient la valeur entière contenue dans la cellule. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset) { get; } | Indique si le style de la cellule est défini. Si le retour est faux, cela signifie que cette cellule a un format de cellule par défaut. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name) { get; } | Obtient le nom de la cellule. Par exemple : A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row) { get; } | Obtient le numéro de ligne (base zéro) de la cellule. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue) { get; } | Obtient la valeur de chaîne contenue dans la cellule. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style) { get; set; } | Obtient la copie du style de cellule. définir le style de la cellule. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type) { get; } | renvoie le type de valeur de cellule, la signification peut voir GridCellValueType.java |
| [Value](../../aspose.cells.gridweb.data/gridcell/value) { get; set; } | Obtient la valeur contenue dans cette cellule. |

## Méthodes

| Nom | La description |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink)() | Indique si cette cellule contient un lien externe. S'applique uniquement lorsque la cellule est une cellule de formule. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy)(GridCell) | Copie les données d'une cellule source. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle)(GridTableItemStyle) | copiez le style et définissez le style de la cellule |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment)(string, string, bool) | Crée un objet de commentaire pour une cellule. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation)(GridValidationType, bool) | Crée un objet de validation pour une cellule. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.gridweb.data/gridcell/getcellarea)() |  |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment)() | Obtenir un objet de commentaire sur cette cellule |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode)() |  |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue)() | Obtient la largeur de la valeur en unité de pixels. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue)() | Vérifie si une formule peut évaluer correctement un résultat. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula)() | Indique si la cellule spécifiée contient une formule. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue)(bool) | Place une valeur booléenne dans la cellule. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_3)(DateTime) | Place une valeur DateTime dans la cellule. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_1)(double) | Met une valeur double dans la cellule. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_2)(int) | Met une valeur int dans la cellule. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_4)(object) | Place une valeur d'objet dans la cellule.identique à setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_5)(string) | Place une valeur de chaîne dans la cellule. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_6)(string, bool) | Insère une valeur de chaîne dans la cellule et convertit la valeur en un autre type de données, le cas échéant. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | Met une valeur dans la cellule, le cas échéant, la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue)(string) | Définit la valeur de la cellule avec une valeur de chaîne et définit le format de cellule par cette valeur. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment)() | Supprime l'objet commentaire de la cellule. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation)() | Supprime l'objet de validation de la cellule. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder)(WebBorderStyle) | Définit les bordures (haut, bas, gauche et droite) pour une cellule, toutes les bordures ont le même style de bordure. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom)(string) | définit le format personnalisé, une chaîne nulle ou vide signifie qu'il n'y a pas de format personnalisé. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula)(string, object) | Définissez la formule et la valeur de la formule. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype)(int) | définir le format d'affichage des nombres et des dates |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring#tostring)() | Renvoie une chaîne représentant l'objet Cell actuel. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality) |  |

### Voir également

* espace de noms [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* Assemblée [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
