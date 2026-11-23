---
title: "Classe GridCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.GridCell. Représente un objet cellule."
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

Représente un objet cellule.

```csharp
public class GridCell
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue/) { get; } | Obtient la valeur booléenne contenue dans la cellule. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column/) { get; } | Obtient le numéro de colonne (à partir de zéro) de la cellule. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue/) { get; } | Obtient la valeur DateTime contenue dans la cellule. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue/) { get; } | Obtient la valeur de chaîne formatée de cette cellule. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue/) { get; } | Obtient la valeur double contenue dans la cellule. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue/) { get; } | Obtient la valeur flottante contenue dans la cellule. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula/) { get; set; } | Obtient ou définit une formule du `GridCell`. |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring/) { get; set; } | Obtient et définit la chaîne HTML qui contient des données et certains formats dans cette cellule. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue/) { get; } | Obtient la valeur entière contenue dans la cellule. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset/) { get; } | Indique si le style de la cellule est défini. Si la valeur retournée est false, cela signifie que cette cellule utilise le format de cellule par défaut. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name/) { get; } | Obtient le nom de la cellule. Par exemple : A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row/) { get; } | Obtient le numéro de ligne (à partir de zéro) de la cellule. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue/) { get; } | Obtient la valeur de chaîne contenue dans la cellule. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style/) { get; set; } | Obtient la copie du style de la cellule. définit le style pour la cellule. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type/) { get; } | renvoie le type de valeur de la cellule, la signification peut être consultée dans GridCellValueType.java |
| [Value](../../aspose.cells.gridweb.data/gridcell/value/) { get; set; } | Obtient la valeur contenue dans cette cellule. |

## Méthodes

| Nom | Description |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink/)() | Indique si cette cellule contient un lien externe. S'applique uniquement lorsque la cellule est une cellule de formule. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy/)(GridCell) | Copie les données d'une cellule source. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle/)(GridTableItemStyle) | copie le style et définit le style pour la cellule |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment/)(string, string, bool) | Crée un objet commentaire pour une cellule. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation/)(GridValidationType, bool) | Crée un objet de validation pour une cellule. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals/)(object) | Vérifie si cet objet fait référence à la même cellule qu'un autre objet cellule. |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment/)() | Obtenir l'objet commentaire sur cette cellule |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode/)() | Fonctionne comme une fonction de hachage pour un type particulier. |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue/)() | Obtient la largeur de la valeur en pixels. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue/)() | Vérifie si une formule peut correctement évaluer un résultat. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula/)() | Indique si la cellule spécifiée contient une formule. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue)(bool) | Place une valeur booléenne dans la cellule. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_3)(DateTime) | Place une valeur DateTime dans la cellule. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_1)(double) | Place une valeur double dans la cellule. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_2)(int) | Insère une valeur int dans la cellule. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_4)(object) | Insère une valeur d'objet dans la cellule. identique à setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_5)(string) | Insère une valeur String dans la cellule. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_6)(string, bool) | Place une valeur chaîne dans la cellule et convertit la valeur en un autre type de données si approprié. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Place une valeur dans la cellule ; si approprié, la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue/)(string) | Définit la valeur de la cellule avec une valeur chaîne et définit le format de la cellule selon cette valeur. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment/)() | Supprime l'objet commentaire de la cellule. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation/)() | Supprime l'objet de validation de la cellule. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder/)(WebBorderStyle) | Définit les bordures (haut, bas, gauche et droite) d'une cellule, toutes les bordures ayant le même style de bordure. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom/)(string) | définit le format personnalisé, null ou chaîne vide signifie aucun format personnalisé. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula/)(string, object) | Définissez la formule et la valeur de la formule. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype/)(int) | définissez le format d'affichage des nombres et des dates |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring/#tostring)() | Renvoie une chaîne qui représente l'objet Cell actuel. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality/) |  |

### Voir aussi

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


