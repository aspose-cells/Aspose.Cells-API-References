---
title: "Classe Cell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Cell. Encapsule l'objet qui représente une seule cellule de classeur."
type: docs
url: /fr/net/aspose.cells/cell/
---
## Cell class

Encapsule l'objet qui représente une seule cellule de Workbook.

```csharp
public class Cell
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue/) { get; } | Obtient la valeur booléenne contenue dans la cellule. |
| [Column](../../aspose.cells/cell/column/) { get; } | Obtient le numéro de colonne (à partir de zéro) de la cellule. |
| [Comment](../../aspose.cells/cell/comment/) { get; } | Obtient le commentaire de cette cellule. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink/) { get; } | Indique si cette cellule contient un lien externe. S'applique uniquement lorsque la cellule est une cellule de formule. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue/) { get; } | Obtient la valeur DateTime contenue dans la cellule. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue/) { get; } | Obtient la valeur chaîne formatée de cette cellule selon le style d'affichage de la cellule. |
| [DoubleValue](../../aspose.cells/cell/doublevalue/) { get; } | Obtient la valeur double contenue dans la cellule. |
| [EmbeddedImage](../../aspose.cells/cell/embeddedimage/) { get; set; } | Obtient et définit l'image intégrée dans la cellule. |
| [FloatValue](../../aspose.cells/cell/floatvalue/) { get; } | Obtient la valeur flottante contenue dans la cellule. |
| [Formula](../../aspose.cells/cell/formula/) { get; set; } | Obtient ou définit une formule de la `Cell`. |
| [FormulaLocal](../../aspose.cells/cell/formulalocal/) { get; set; } | Obtenez la formule formatée selon la locale de la cellule. |
| [HasCustomFunction](../../aspose.cells/cell/hascustomfunction/) { get; } | Vérifie s'il existe une fonction personnalisée (fonction non prise en charge) dans la formule de cette cellule. |
| [HasCustomStyle](../../aspose.cells/cell/hascustomstyle/) { get; } | Indique si cette cellule possède des paramètres de style personnalisés (différents de ceux par défaut hérités de la ligne, de la colonne ou du classeur correspondants). |
| [HtmlString](../../aspose.cells/cell/htmlstring/) { get; set; } | Obtient et définit la chaîne HTML qui contient des données et certains formats dans cette cellule. |
| [IntValue](../../aspose.cells/cell/intvalue/) { get; } | Obtient la valeur entière contenue dans la cellule. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula/) { get; } | Indique si la formule de la cellule est une formule matricielle. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader/) { get; } | Indique que la formule de la cellule est une formule de tableau et qu'elle est la première cellule du tableau. |
| [IsCheckBoxStyle](../../aspose.cells/cell/ischeckboxstyle/) { get; set; } | Indique si la cellule est définie comme case à cocher. |
| [IsDynamicArrayFormula](../../aspose.cells/cell/isdynamicarrayformula/) { get; } | Indique si la formule de la cellule est une formule de tableau dynamique (true) ou une formule de tableau héritée (false). |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue/) { get; } | Vérifie si la valeur de cette cellule est une erreur. |
| [IsFormula](../../aspose.cells/cell/isformula/) { get; } | Indique si la cellule spécifiée contient une formule. |
| [IsInArray](../../aspose.cells/cell/isinarray/) { get; } | (**Obsolete.**) Indique si la formule de la cellule est une formule de tableau. |
| [IsInTable](../../aspose.cells/cell/isintable/) { get; } | (**Obsolete.**) Indique si cette cellule fait partie d'une formule de tableau. |
| [IsMerged](../../aspose.cells/cell/ismerged/) { get; } | Vérifie si une cellule fait partie d'une plage fusionnée ou non. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue/) { get; } | Indique si la valeur de cette cellule est numérique (int, double et datetime). |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula/) { get; } | Indique si la formule de la cellule fait partie d'une formule partagée. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset/) { get; } | Indique si le style de la cellule est défini. Si la valeur retournée est false, cela signifie que cette cellule utilise le format de cellule par défaut. |
| [IsTableFormula](../../aspose.cells/cell/istableformula/) { get; } | Indique si cette cellule fait partie d'une formule de tableau. |
| [Name](../../aspose.cells/cell/name/) { get; } | Obtient le nom de la cellule. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype/) { get; } | Représente le type de catégorie du format numérique de cette cellule. |
| [Picture](../../aspose.cells/cell/picture/) { get; } | Obtient une instance de [`Picture`](../../aspose.cells.drawing/picture/) pour représenter l'image intégrée dans cette cellule ou null s'il n'y a aucune image intégrée pour cette cellule. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula/) { get; set; } | Obtient ou définit une formule R1C1 de la `Cell`. |
| [Row](../../aspose.cells/cell/row/) { get; } | Obtient le numéro de ligne (à partir de zéro) de la cellule. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex/) { get; } | Obtient l'index du style partagé de la cellule dans le pool de styles. |
| [StringValue](../../aspose.cells/cell/stringvalue/) { get; } | Obtient la valeur chaîne contenue dans la cellule. Si le type de cette cellule est chaîne, la valeur chaîne elle‑même est retournée. Pour les autres types de cellules, la valeur chaîne formatée (formatée avec le style spécifié de cette cellule) est retournée. La valeur de cellule formatée est identique à ce que vous pouvez obtenir depuis Excel en copiant une cellule en tant que texte (par exemple en copiant la cellule dans un éditeur de texte ou en l'exportant vers CSV). |
| [StringValueWithoutFormat](../../aspose.cells/cell/stringvaluewithoutformat/) { get; } | (**Obsolete.**) Obtient la valeur de la cellule sous forme de chaîne sans aucun format. |
| [Type](../../aspose.cells/cell/type/) { get; } | Représente le type de valeur de la cellule. |
| [Value](../../aspose.cells/cell/value/) { get; set; } | Obtient/definit la valeur contenue dans cette cellule. |
| [Worksheet](../../aspose.cells/cell/worksheet/) { get; } | Obtient la feuille de calcul parente. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate/)(CalculationOptions) | Calcule la formule de la cellule. |
| [Characters](../../aspose.cells/cell/characters/)(int, int) | Renvoie un objet Characters qui représente une plage de caractères dans le texte de la cellule. |
| [Copy](../../aspose.cells/cell/copy/)(Cell) | Copie les données d'une cellule source. |
| [Equals](../../aspose.cells/cell/equals/#equals)(Cell) | Vérifie si cet objet fait référence à la même cellule qu'un autre objet cellule. |
| override [Equals](../../aspose.cells/cell/equals/#equals_1)(object) | Vérifie si cet objet fait référence à la même cellule qu'un autre. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange/)() | Obtient la plage de tableau si la formule de la cellule est une formule matricielle. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters)() | Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte de la cellule. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters_1)(bool) | Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte de la cellule. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult/)() | Obtenir le résultat du formatage conditionnel. |
| [GetDependents](../../aspose.cells/cell/getdependents/)(bool) | Obtenir toutes les cellules dont la formule fait référence directement à cette cellule. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation/)(bool) | Obtient toutes les cellules dont le résultat calculé dépend de cette cellule. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle)() | Obtient le style d'affichage de cette cellule. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_2)(bool) | Obtient le style d'affichage de cette cellule. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_1)(BorderType) | Obtient le style d'affichage de cette cellule. |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions/)() | Obtient les conditions de format qui s'appliquent à cette cellule. |
| [GetFormula](../../aspose.cells/cell/getformula/)(bool, bool) | Obtenir la formule de cette cellule. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode/)() | Fonctionne comme une fonction de hachage pour un type particulier. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue/)() | Obtient la hauteur de la valeur en pixels. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring/)(bool) | Obtient la chaîne html qui contient des données et certains formats dans cette cellule. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs)() | (**Obsolete.**) Obtenir toutes les cellules qui font référence directement à cette cellule et qui doivent être mises à jour lorsque cette cellule est modifiée. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs_1)(bool) | (**Obsolete.**) Obtenir toutes les cellules qui seront mises à jour lorsque cette cellule sera modifiée. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange/)() | Renvoie un objet [`Range`](../range/) qui représente une plage fusionnée. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents/)() | Obtient toutes les références apparaissant dans la formule de cette cellule. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation/)() | Obtient tous les antécédents (référence aux cellules du classeur actuel) utilisés par la formule de cette cellule lors de son calcul. |
| [GetRichValue](../../aspose.cells/cell/getrichvalue/)() | Obtient la valeur enrichie de la cellule. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue/)(CellValueFormatStrategy) | Obtient la valeur chaîne selon une stratégie de formatage spécifique. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle)() | Obtient le style de la cellule. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle_1)(bool) | Si checkBorders est vrai, vérifie si les bordures des autres cellules affecteront le style de cette cellule. |
| [GetTable](../../aspose.cells/cell/gettable/)() | Obtient le tableau qui contient cette cellule. |
| [GetValidation](../../aspose.cells/cell/getvalidation/)() | Obtient la validation appliquée à cette cellule. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue/)() | Obtient la valeur de validation appliquée à cette cellule. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue/)() | Obtient la largeur de la valeur en pixels. |
| [InsertText](../../aspose.cells/cell/inserttext/)(int, string) | Insère des caractères dans la cellule. Si la cellule est formatée richement, cette méthode peut conserver le formatage original. |
| [IsRichText](../../aspose.cells/cell/isrichtext/)() | Indique si la valeur chaîne de cette cellule est un texte formaté richement. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue)(bool) | Place une valeur booléenne dans la cellule. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_3)(DateTime) | Place une valeur DateTime dans la cellule. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_1)(double) | Place une valeur double dans la cellule. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_2)(int) | Place une valeur entière dans la cellule. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_4)(object) | Place une valeur d'objet dans la cellule. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_5)(string) | Place une valeur chaîne dans la cellule. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_6)(string, bool) | Place une valeur chaîne dans la cellule et convertit la valeur en un autre type de données si approprié. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_7)(string, bool, bool) | Place une valeur dans la cellule ; si approprié, la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula/)(bool) | Supprime la formule de tableau. |
| [Replace](../../aspose.cells/cell/replace/)(string, string, ReplaceOptions) | Remplace le texte de la cellule avec des options. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula)(string, int, int) | Définit une formule de tableau(formule de tableau héritée saisie via CTRL+SHIFT+ENTER dans MS Excel) pour une plage de cellules. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_1)(string, int, int, FormulaParseOptions) | Définit une formule de tableau pour une plage de cellules. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Définit une formule de tableau pour une plage de cellules. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Définit une formule de tableau pour une plage de cellules. |
| [SetCharacters](../../aspose.cells/cell/setcharacters/)(FontSetting[]) | Définit le format de texte riche de la cellule. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Définit une formule de tableau dynamique et fait déborder la formule dans les cellules voisines si possible. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Définit une formule de tableau dynamique et fait déborder la formule dans les cellules voisines si possible. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_2)(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) | Définit une formule de tableau dynamique et fait déborder la formule dans les cellules voisines si possible. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula)(string, FormulaParseOptions) | Définit la formule et la valeur(résultat calculé) de la formule. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_3)(string, object) | Définit la formule et la valeur(résultat calculé) de la formule. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_1)(string, FormulaParseOptions, object) | Définit la formule et la valeur(résultat calculé) de la formule. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_2)(string, bool, bool, object) | (**Obsolete.**) Définit la formule et la valeur de la formule. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula)(string, int, int) | Définit des formules partagées pour une plage de cellules. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_1)(string, int, int, FormulaParseOptions) | Définit des formules partagées pour une plage de cellules. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Définit une formule pour une plage de cellules. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Définit des formules partagées pour une plage de cellules. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle)(Style) | Définit le style de la cellule. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_2)(Style, bool) | Applique la propriété modifiée du style à la cellule. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_1)(Style, StyleFlag) | Appliquer le style de la cellule en fonction des indicateurs. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_2)(int, int, string, bool, object[][]) | Créer un tableau de données à une variable pour la plage donnée en commençant à partir de cette cellule. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_3)(int, int, string, string, object[][]) | Créer un tableau de données à deux variables pour la plage donnée en commençant à partir de cette cellule. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula)(int, int, int, int, bool, object[][]) | Créer un tableau de données à une variable pour la plage donnée en commençant à partir de cette cellule. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_1)(int, int, int, int, int, int, object[][]) | Créer un tableau de données à deux variables pour la plage donnée en commençant à partir de cette cellule. |
| [ToJson](../../aspose.cells/cell/tojson/)() | Convertir `Cell` en données struct JSON. |
| override [ToString](../../aspose.cells/cell/tostring/)() | Renvoie une chaîne qui représente l'objet Cell actuel. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellDemo
    {
        public static void CellExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            // Accéder à la collection de cellules
            Cells cells = worksheet.Cells;

            // Insérer une chaîne dans une cellule
            Cell cell = cells[0, 0];
            cell.PutValue("Hello");

            // Insérer un entier dans une cellule
            cell = cells["B1"];
            cell.PutValue(12);

            // Insérer un double dans une cellule
            cell = cells[0, 2];
            cell.PutValue(-1.234);

            // Insérer une formule dans une cellule
            cell = cells["D1"];
            cell.Formula = "=B1 + C1";

            // Insérer une formule combinée : "sum(average(b1,c1), b1)" dans la cellule b2
            cell = cells["B2"];
            cell.Formula = "=sum(average(b1,c1), b1)";

            // Définir le style d'une cellule
            Style style = cell.GetStyle();
            // Définir la couleur d'arrière-plan
            style.BackgroundColor = System.Drawing.Color.Yellow;
            // Définir la police d'une cellule
            style.Font.Name = "Courier New";
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("CellExample.xlsx");
            workbook.Save("CellExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


