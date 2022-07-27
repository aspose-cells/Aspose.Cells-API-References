---
title: GridCell
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente un objet cellule.
type: docs
weight: 370
url: /fr/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

Représente un objet cellule.

```csharp
public class GridCell
```

## Propriétés

| Nom | La description |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue) { get; } | Obtient la valeur booléenne contenue dans la cellule. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column) { get; } | Obtient le numéro de colonne (base zéro) de la cellule. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue) { get; } | Obtient la valeur DateTime contenue dans la cellule. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue) { get; } | Obtient la valeur de chaîne formatée de cette cellule. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue) { get; } | Obtient la valeur double contenue dans la cellule. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue) { get; } | Obtient la valeur flottante contenue dans la cellule. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula) { get; set; } | Obtient ou définit une formule duCell . |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring) { get; set; } | Obtient et définit la chaîne html qui contient des données et certaines mises en forme dans cette cellule. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue) { get; } | Obtient la valeur entière contenue dans la cellule. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset) { get; } | Indique si le style de la cellule est défini. Si le retour est faux, cela signifie que cette cellule a un format de cellule par défaut. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name) { get; } | Obtient le nom de la cellule. Par exemple : A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected) { get; set; } | Indique si la cellule est protégée. Si la valeur est "true", l'utilisateur ne peut pas modifier la cellule via l'interface utilisateur. Cet attribut n'a rien à voir avec la propriété Style.CellLocked et ne sera pas enregistré dans le fichier lorsque données de grille exportées. La valeur par défaut est "false". |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row) { get; } | Obtient le numéro de ligne (base zéro) de la cellule. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue) { get; } | Obtient la valeur de chaîne contenue dans la cellule. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style) { get; set; } | Obtient la copie du style de cellule. définir le style de la cellule. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type) { get; } | renvoie le type de valeur de cellule, la signification peut voir GridCellValueType.java |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value) { get; set; } | Obtient la valeur contenue dans cette cellule. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet) { get; } | Obtient l'objet feuille de calcul. |

## Méthodes

| Nom | La description |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink)() | Indique si cette cellule contient un lien externe. S'applique uniquement lorsque la cellule est une cellule de formule. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy)(GridCell) | Copie les données d'une cellule source. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle)(Style) | copiez le style et définissez le style de la cellule |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont)() | Obtient la police de la cellule. Lorsque vous modifiez la police, vous devez appeler la méthode "SetFont", pour définir la police sur la cellule. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor)() | Obtient la couleur de la police de la cellule. Lorsque vous modifiez la couleur, vous devez appeler la méthode "SetFontColor", pour définir la couleur de la police sur la cellule. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle)() | Obtient le style de cellule. Lorsque vous modifiez le style, vous devez appeler la méthode "SetStyle", pour définir le style sur la cellule. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation)() | Obtient la validation qui s'applique à cette cellule. Si elle n'est pas définie, retourne null. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue)() | Obtient la largeur de la valeur en unité de pixels. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet)() | Obtient la feuille de calcul parente. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue)() | Vérifie si une formule peut évaluer correctement un résultat. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula)() | Indique si la cellule spécifiée contient une formule. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue)(bool) | Place une valeur booléenne dans la cellule. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_3)(DateTime) | Place une valeur DateTime dans la cellule. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_1)(double) | Met une valeur double dans la cellule. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_2)(int) | Met une valeur int dans la cellule. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_4)(object) | Place une valeur d'objet dans la cellule.identique à setValue(Object param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_5)(string) | Place une valeur de chaîne dans la cellule. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_6)(string, bool) | Insère une valeur de chaîne dans la cellule et convertit la valeur en un autre type de données, le cas échéant. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | Met une valeur dans la cellule, le cas échéant, la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue)(string) | Définit la valeur de la cellule avec une valeur de chaîne et définit le format de cellule par cette valeur. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue)(object) | Si la valeur est une formule, cette méthode définit la valeur de la cellule comme FormulaType, |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom)(string) | définit le format personnalisé, une chaîne nulle ou vide signifie qu'il n'y a pas de format personnalisé. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont)(Font) | Définit la police sur la cellule. Pour améliorer les performances, implémentez la méthode "SetFont", n'implémentez pas la propriété "Font". |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor)(Color) | Définit la couleur de la police sur la cellule. Pour améliorer les performances, implémentez la méthode "SetFontColor", n'implémentez pas la propriété "FontColor". |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula)(string, object) | Définissez la formule et la valeur de la formule. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype)(int) | définir le format d'affichage des nombres et des dates |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle)(Style) | Définit le style sur la cellule. Pour améliorer les performances, implémentez la méthode "SetStyle", n'implémentez pas la propriété "Style". |
| [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring#tostring)() | Renvoie une chaîne représentant l'objet Cell actuel. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality) |  |

### Voir également

* espace de noms [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* Assemblée [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
