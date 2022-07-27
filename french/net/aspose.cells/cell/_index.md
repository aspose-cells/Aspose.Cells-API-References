---
title: Cell
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule lobjet qui représente une seule cellule de classeur.
type: docs
weight: 230
url: /fr/net/aspose.cells/cell/
---
## Cell class

Encapsule l'objet qui représente une seule cellule de classeur.

```csharp
public class Cell
```

## Propriétés

| Nom | La description |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue) { get; } | Obtient la valeur booléenne contenue dans la cellule. |
| [Column](../../aspose.cells/cell/column) { get; } | Obtient le numéro de colonne (base zéro) de la cellule. |
| [Comment](../../aspose.cells/cell/comment) { get; } | Obtient le commentaire de cette cellule. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink) { get; } | Indique si cette cellule contient un lien externe. S'applique uniquement lorsque la cellule est une cellule de formule. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue) { get; } | Obtient la valeur DateTime contenue dans la cellule. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue) { get; } | Obtient la valeur de chaîne formatée de cette cellule par le style d'affichage de la cellule. |
| [DoubleValue](../../aspose.cells/cell/doublevalue) { get; } | Obtient la valeur double contenue dans la cellule. |
| [FloatValue](../../aspose.cells/cell/floatvalue) { get; } | Obtient la valeur flottante contenue dans la cellule. |
| [Formula](../../aspose.cells/cell/formula) { get; set; } | Obtient ou définit une formule du[`Cell`](../cell) . |
| [FormulaLocal](../../aspose.cells/cell/formulalocal) { get; set; } | Obtenir la formule formatée locale de la cellule. |
| [HtmlString](../../aspose.cells/cell/htmlstring) { get; set; } | Obtient et définit la chaîne html qui contient des données et certains formats dans cette cellule. |
| [IntValue](../../aspose.cells/cell/intvalue) { get; } | Obtient la valeur entière contenue dans la cellule. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula) { get; } | Indique si la formule de la cellule est une formule matricielle. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader) { get; } | Indique que la formule de la cellule est une formule matricielle et qu'il s'agit de la première cellule du tableau. |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue) { get; } | Vérifie si la valeur de cette cellule est une erreur. |
| [IsFormula](../../aspose.cells/cell/isformula) { get; } | Indique si la cellule spécifiée contient une formule. |
| [IsMerged](../../aspose.cells/cell/ismerged) { get; } | Vérifie si une cellule fait partie d'une plage fusionnée ou non. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue) { get; } | Indique si la valeur interne de cette cellule est numérique (int, double et datetime) |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula) { get; } | Indique si la formule de la cellule fait partie de la formule partagée. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset) { get; } | Indique si le style de la cellule est défini. Si le retour est faux, cela signifie que cette cellule a un format de cellule par défaut. |
| [IsTableFormula](../../aspose.cells/cell/istableformula) { get; } | Indique si cette cellule fait partie de la formule du tableau. |
| [Name](../../aspose.cells/cell/name) { get; } | Obtient le nom de la cellule. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype) { get; } | Représente le type de catégorie du formatage des nombres de cette cellule. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula) { get; set; } | Obtient ou définit une formule R1C1 du[`Cell`](../cell) . |
| [Row](../../aspose.cells/cell/row) { get; } | Obtient le numéro de ligne (base zéro) de la cellule. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex) { get; } | Obtient l'index de style partagé de la cellule dans le pool de styles. |
| [StringValue](../../aspose.cells/cell/stringvalue) { get; } | Obtient la valeur de chaîne contenue dans la cellule. Si le type de cette cellule est une chaîne, renvoyez la valeur de chaîne elle-même. Pour les autres types de cellules, la valeur de chaîne formatée (formatée avec le style spécifié de cette cellule) sera renvoyée. La valeur de cellule formatée est identique à ce que vous peut obtenir d'Excel lors de la copie d'une cellule sous forme de texte (comme copier une cellule dans un éditeur de texte ou exporter vers csv). |
| [Type](../../aspose.cells/cell/type) { get; } | Représente le type de valeur de cellule. |
| [Value](../../aspose.cells/cell/value) { get; set; } | Obtient la valeur contenue dans cette cellule. |
| [Worksheet](../../aspose.cells/cell/worksheet) { get; } | Obtient la feuille de calcul parente. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate#calculate)(CalculationOptions) | Calcule la formule de la cellule. |
| [Characters](../../aspose.cells/cell/characters)(int, int) | Renvoie un objet Characters qui représente une plage de caractères dans le texte de la cellule. |
| [Copy](../../aspose.cells/cell/copy)(Cell) | Copie les données d'une cellule source. |
| [Equals](../../aspose.cells/cell/equals#equals)(Cell) | Vérifie si cet objet fait référence à la même cellule avec un autre objet de cellule. |
| override [Equals](../../aspose.cells/cell/equals#equals_1)(object) | Vérifie si cet objet fait référence à la même cellule avec un autre. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange)() | Obtient la plage du tableau si la formule de la cellule est une formule matricielle. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters)() | Renvoie tous les objets Caractères qui représentent une plage de caractères dans le texte de la cellule. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters_1)(bool) | Renvoie tous les objets Caractères qui représentent une plage de caractères dans le texte de la cellule. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult)() | Obtenez le résultat de la mise en forme conditionnelle. |
| [GetDependents](../../aspose.cells/cell/getdependents)(bool) | Obtenir toutes les cellules dont la formule fait directement référence à cette cellule. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation)(bool) | Obtient toutes les cellules dont le résultat calculé dépend de cette cellule. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle)() | Obtient le style d'affichage de la cellule. Si cette cellule est également affectée par d'autres paramètres tels que la mise en forme conditionnelle, les objets de liste, etc., , le style d'affichage peut être différent de cell.GetStyle(). |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle_1)(bool) | Obtient le style d'affichage de la cellule. Si la cellule est formatée de manière conditionnelle, le style d'affichage n'est pas le même que celui de la cellule.GetStyle(). |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions)() | Obtient les conditions de format qui s'appliquent à cette cellule. |
| [GetFormula](../../aspose.cells/cell/getformula)(bool, bool) | Obtenir la formule de cette cellule. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode)() | Sert de fonction de hachage pour un type particulier. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue)() | Obtient la hauteur de la valeur en unité de pixels. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring)(bool) | Obtient la chaîne html qui contient des données et certains formats dans cette cellule. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange)() | Renvoie un[`Range`](../range) objet qui représente une plage fusionnée. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents)() | Obtient toutes les références apparaissant dans la formule de cette cellule. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation)() | Obtient tous les précédents (référence aux cellules du classeur actuel) utilisés par la formule de cette cellule lors de son calcul. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue)(CellValueFormatStrategy) | Obtient la valeur de chaîne par une stratégie formatée spécifique. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle)() | Obtient le style de cellule. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle_1)(bool) | Si checkBorders est vrai, vérifie si les bordures des autres cellules affecteront le style de cette cellule. |
| [GetTable](../../aspose.cells/cell/gettable)() | Obtient la table qui contient cette cellule. |
| [GetValidation](../../aspose.cells/cell/getvalidation)() | Obtient la validation appliquée à cette cellule. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue)() | Obtient la valeur de validation appliquée à cette cellule. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue)() | Obtient la largeur de la valeur en unité de pixels. |
| [IsRichText](../../aspose.cells/cell/isrichtext)() | Indique si la valeur de la chaîne de cellule est un texte enrichi. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue)(bool) | Place une valeur booléenne dans la cellule. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_3)(DateTime) | Place une valeur DateTime dans la cellule. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_1)(double) | Met une valeur double dans la cellule. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_2)(int) | Insère une valeur entière dans la cellule. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_4)(object) | Place une valeur d'objet dans la cellule. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_5)(string) | Place une valeur de chaîne dans la cellule. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_6)(string, bool) | Insère une valeur de chaîne dans la cellule et convertit la valeur en un autre type de données, le cas échéant. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_7)(string, bool, bool) | Met une valeur dans la cellule, le cas échéant, la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula)(bool) | Supprimer la formule matricielle. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula)(string, int, int) | Définit une formule matricielle (formule matricielle héritée saisie via CTRL + MAJ + ENTRÉE dans ms excel) sur une plage de cellules. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_1)(string, int, int, FormulaParseOptions) | Définit une formule matricielle sur une plage de cellules. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Définit une formule matricielle sur une plage de cellules. |
| [SetCharacters](../../aspose.cells/cell/setcharacters)(FontSetting[]) | Définit le format de texte enrichi de la cellule. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Définit la formule de tableau dynamique et fait en sorte que la formule se répande dans les cellules voisines si possible. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Définit la formule de tableau dynamique et fait en sorte que la formule se répande dans les cellules voisines si possible. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula_2)(string, object) | Définissez la formule et la valeur de la formule. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula)(string, FormulaParseOptions, object) | Définissez la formule et la valeur de la formule. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula)(string, int, int) | Définit une formule sur une plage de cellules. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_1)(string, int, int, FormulaParseOptions) | Définit une formule sur une plage de cellules. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Définit une formule sur une plage de cellules. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle)(Style) | Définit le style de cellule. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_2)(Style, bool) | Appliquer le style de cellule. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_1)(Style, StyleFlag) | Appliquer le style de cellule. |
| override [ToString](../../aspose.cells/cell/tostring)() | Renvoie une chaîne représentant l'objet Cell actuel. |

### Exemples

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

// Met une chaîne dans une cellule
Cell cell = cells[0, 0];
cell.PutValue("Hello");

string first = cell.StringValue;
	
// Met un entier dans une cellule
cell = cells["B1"];
cell.PutValue(12);

int second = cell.IntValue;

//Mettre un double dans une cellule
cell = cells[0, 2];
cell.PutValue(-1.234);

double third = cell.DoubleValue;

//Insérer une formule dans une cellule
cell = cells["D1"];
cell.Formula = "=B1 + C1";

//Mettez une formule combinée : "somme(moyenne(b1,c1), b1)" dans la cellule en b2
cell = cells["b2"];
cell.Formula = "=sum(average(b1,c1), b1)";

//Définir le style d'une cellule
Style style = cell.GetStyle();
//Définir la couleur de fond
style.BackgroundColor = Color.Yellow;
//Définir le format d'une cellule
style.Font.Name = "Courier New";
style.VerticalAlignment = TextAlignmentType.Top;
cell.SetStyle(style);



[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = exce.Worksheets(0).Cells

'Mettre une chaîne dans une cellule
Dim cell as Cell = cells(0, 0)
cell.PutValue("Hello")

Dim first as String = cell.StringValue
	
// Met un entier dans une cellule
cell = cells("B1")
cell.PutValue(12)

Dim second as Integer = cell.IntValue

//Mettre un double dans une cellule
cell = cells(0, 2)
cell.PutValue(-1.234)

Dim third as Double = cell.DoubleValue

//Insérer une formule dans une cellule
cell = cells("D1")
cell.Formula = "=B1 + C1"

//Mettez une formule combinée : "somme(moyenne(b1,c1), b1)" dans la cellule en b2
cell = cells("b2")
cell.Formula = "=sum(average(b1,c1), b1)"
	
//Définir le style d'une cellule
Dim style as Style = cell.GetStyle()

//Définir la couleur de fond
style.BackgroundColor = Color.Yellow
//Définir la police d'une cellule
style.Font.Name = "Courier New"
style.VerticalAlignment = TextAlignmentType.Top
cell.SetStyle(style)
```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
