---
title: "Classe GridCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridDesktop.Data.GridCell. Représente un objet cellule"
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

Représente un objet cellule.

```csharp
public class GridCell
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue/) { get; } | Obtient la valeur booléenne contenue dans la cellule. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column/) { get; } | Obtient le numéro de colonne (à partir de zéro) de la cellule. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue/) { get; } | Obtient la valeur DateTime contenue dans la cellule. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue/) { get; } | Obtient la valeur de chaîne formatée de cette cellule. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue/) { get; } | Obtient la valeur double contenue dans la cellule. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue/) { get; } | Obtient la valeur flottante contenue dans la cellule. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula/) { get; set; } | Obtient ou définit une formule de la cellule. |
| [HasCustomStyle](../../aspose.cells.griddesktop.data/gridcell/hascustomstyle/) { get; } | Indique si cette cellule possède des paramètres de style personnalisés (différents de ceux par défaut hérités de la ligne, de la colonne ou du classeur correspondants). |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring/) { get; set; } | Obtient et définit la chaîne HTML qui contient des données et certains formats dans cette cellule. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue/) { get; } | Obtient la valeur entière contenue dans la cellule. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset/) { get; } | Indique si le style de la cellule est défini. Si la valeur retournée est false, cela signifie que cette cellule utilise le format de cellule par défaut. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location/) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name/) { get; } | Obtient le nom de la cellule. Par exemple : A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected/) { get; set; } | Indique si la cellule est protégée. Si la valeur est "true", l'utilisateur ne peut pas modifier la cellule via l'interface utilisateur. Cet attribut n'a aucun rapport avec la propriété Style.CellLocked et ne sera pas enregistré dans le fichier lors de l'exportation des données de la grille. La valeur par défaut est "false". |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row/) { get; } | Obtient le numéro de ligne (à partir de zéro) de la cellule. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue/) { get; } | Obtient la valeur de chaîne contenue dans la cellule. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style/) { get; set; } | Obtient la copie du style de la cellule. définit le style pour la cellule. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type/) { get; } | renvoie le type de valeur de la cellule, la signification peut être consultée dans GridCellValueType.java |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value/) { get; set; } | Obtient la valeur contenue dans cette cellule. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet/) { get; } | Obtient l'objet feuille de calcul. |

## Méthodes

| Nom | Description |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink/)() | Indique si cette cellule contient un lien externe. S'applique uniquement lorsque la cellule est une cellule de formule. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy/)(GridCell) | Copie les données d'une cellule source. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle/)(Style) | copie le style et définit le style pour la cellule |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals/)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea/)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont/)() | Obtient la police de la cellule. Lors du changement de la police, vous devez appeler la méthode "SetFont" pour appliquer la police à la cellule. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor/)() | Obtient la couleur de police de la cellule. Lors du changement de la couleur, vous devez appeler la méthode "SetFontColor" pour appliquer la couleur de police à la cellule. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode/)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle/)() | Obtient le style de la cellule. Lors du changement du style, vous devez appeler la méthode "SetStyle" pour appliquer le style à la cellule. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation/)() | Obtient la validation appliquée à cette cellule. Si non définie, renvoie null. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue/)() | Obtient la largeur de la valeur en pixels. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet/)() | Obtient la feuille de calcul parente. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue/)() | Vérifie si une formule peut correctement évaluer un résultat. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula/)() | Indique si la cellule spécifiée contient une formule. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue)(bool) | Place une valeur booléenne dans la cellule. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_3)(DateTime) | Place une valeur DateTime dans la cellule. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_1)(double) | Place une valeur double dans la cellule. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_2)(int) | Insère une valeur int dans la cellule. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_4)(object) | Insère une valeur d'objet dans la cellule. identique à setValue(Object param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_5)(string) | Insère une valeur String dans la cellule. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_6)(string, bool) | Place une valeur chaîne dans la cellule et convertit la valeur en un autre type de données si approprié. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Place une valeur dans la cellule ; si approprié, la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue/)(string) | Définit la valeur de la cellule avec une valeur chaîne et définit le format de la cellule selon cette valeur. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue/)(object) | Si la valeur est une formule, cette méthode définit la valeur de la cellule comme FormulaType, |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom/)(string) | définit le format personnalisé, null ou chaîne vide signifie aucun format personnalisé. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont/)(Font) | Définit la police de la cellule. Pour améliorer les performances, implémentez la méthode "SetFont", n'implémentez pas la propriété "Font". |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor/)(Color) | Définit la couleur de police de la cellule. Pour améliorer les performances, implémentez la méthode "SetFontColor", n'implémentez pas la propriété "FontColor". |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula/)(string, object) | Définissez la formule et la valeur de la formule. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype/)(int) | définissez le format d'affichage des nombres et des dates |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle/)(Style) | Définit le style de la cellule. Pour améliorer les performances, implémentez la méthode "SetStyle", n'implémentez pas la propriété "Style". |
| override [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring/)() | Renvoie une chaîne qui représente l'objet Cell actuel. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality/) |  |

### Voir aussi

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


