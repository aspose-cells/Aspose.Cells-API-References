---
title: "Classe Cell"
linktitle: "Cell"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Cell. Encapsule l'objet qui représente cell en Go."
type: docs
weight: 200
url: /fr/go-cpp/cell/
---

## Cell class

Encapsule l'objet qui représente une cellule unique du classeur.

```go

type Cell struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [Calculate](./calculate/) | Calcule la formule de la cellule. |
| [GetWorksheet](./getworksheet/) | Obtient la feuille de calcul parente. |
| [PutValue_Bool](./putvalue_bool/) | Place une valeur booléenne dans la cellule. |
| [PutValue_Int](./putvalue_int/) | Place une valeur entière dans la cellule. |
| [PutValue_Double](./putvalue_double/) | Place une valeur double dans la cellule. |
| [PutValue_String_Bool_Bool](./putvalue_string_bool_bool/) | Place une valeur dans la cellule, le cas échéant la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [PutValue_String_Bool](./putvalue_string_bool/) | Place une valeur chaîne dans la cellule et convertit la valeur en un autre type de données si nécessaire. |
| [PutValue_String](./putvalue_string/) | Place une valeur chaîne dans la cellule. |
| [PutValue_Date](./putvalue_date/) | Place une valeur DateTime dans la cellule. |
| [PutValue_Object](./putvalue_object/) | Place une valeur d'objet dans la cellule. |
| [GetRow](./getrow/) | Obtient le numéro de ligne (à partir de zéro) de la cellule. |
| [GetColumn](./getcolumn/) | Obtient le numéro de colonne (à partir de zéro) de la cellule. |
| [IsFormula](./isformula/) | Représente si la cellule spécifiée contient une formule. |
| [GetHasCustomFunction](./gethascustomfunction/) | Vérifie s'il y a une fonction personnalisée (fonction non prise en charge) dans la formule de cette cellule. |
| [GetType](./gettype/) | Représente le type de valeur de la cellule. |
| [GetName](./getname/) | Obtient le nom de la cellule. |
| [IsErrorValue](./iserrorvalue/) | Vérifie si la valeur de cette cellule est une erreur. |
| [IsNumericValue](./isnumericvalue/) | Indique si la valeur de cette cellule est numérique (int, double et datetime). |
| [GetStringValue_CellValueFormatStrategy](./getstringvalue_cellvalueformatstrategy/) | Obtient la valeur chaîne selon une stratégie de formatage spécifique. |
| [GetStringValue](./getstringvalue/) | Obtient la valeur chaîne contenue dans la cellule. Si le type de cette cellule est une chaîne, alors la valeur chaîne elle‑même est renvoyée. Pour les autres types de cellules, la valeur chaîne formatée (formatée avec le style spécifié de cette cellule) sera renvoyée. La valeur de cellule formatée est identique à ce que vous pouvez obtenir depuis Excel en copiant une cellule en tant que texte (par exemple en copiant la cellule vers un éditeur de texte ou en l'exportant vers CSV). |
| [GetNumberCategoryType](./getnumbercategorytype/) | Représente le type de catégorie du format numérique de cette cellule. |
| [GetDisplayStringValue](./getdisplaystringvalue/) | Obtient la valeur chaîne formatée de cette cellule selon le style d'affichage de la cellule. |
| [GetIntValue](./getintvalue/) | Obtient la valeur entière contenue dans la cellule. |
| [GetDoubleValue](./getdoublevalue/) | Obtient la valeur double contenue dans la cellule. |
| [GetFloatValue](./getfloatvalue/) | Obtient la valeur flottante contenue dans la cellule. |
| [GetDateTimeValue](./getdatetimevalue/) | Obtient la valeur DateTime contenue dans la cellule. |
| [GetBoolValue](./getboolvalue/) | Obtient la valeur booléenne contenue dans la cellule. |
| [GetWidthOfValue](./getwidthofvalue/) | Obtient la largeur de la valeur en pixels. |
| [GetHeightOfValue](./getheightofvalue/) | Obtient la hauteur de la valeur en pixels. |
| [GetDisplayStyle](./getdisplaystyle/) | Obtient le style d'affichage de cette cellule. |
| [GetDisplayStyle_Bool](./getdisplaystyle_bool/) | Obtient le style d'affichage de cette cellule. |
| [GetDisplayStyle_BorderType](./getdisplaystyle_bordertype/) | Obtient le style d'affichage de cette cellule. |
| [GetFormatConditions](./getformatconditions/) | Obtient les conditions de format qui s'appliquent à cette cellule. |
| [GetStyle](./getstyle/) | Obtient le style de la cellule. |
| [GetStyle_Bool](./getstyle_bool/) | Si checkBorders est vrai, vérifie si les bordures des autres cellules affecteront le style de cette cellule. |
| [SetStyle_Style](./setstyle_style/) | Définit le style de la cellule. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | Applique la propriété modifiée du style à la cellule. |
| [SetStyle_Style_StyleFlag](./setstyle_style_styleflag/) | Applique le style de la cellule en fonction des indicateurs. |
| [GetHasCustomStyle](./gethascustomstyle/) | Indique si cette cellule possède des paramètres de style personnalisés (différents du style par défaut hérité de la ligne, de la colonne ou du classeur correspondant). |
| [GetSharedStyleIndex](./getsharedstyleindex/) | Obtient l'index du style partagé de la cellule dans le pool de styles. |
| [GetFormula](./getformula/) | Obtient ou définit une formule de la cellule. |
| [SetFormula_String](./setformula_string/) | Obtient ou définit une formule de la cellule. |
| [GetFormulaLocal](./getformulalocal/) | Obtient la formule formatée selon la locale de la cellule. |
| [SetFormulaLocal](./setformulalocal/) | Obtient la formule formatée selon la locale de la cellule. |
| [GetR1C1Formula](./getr1c1formula/) | Obtient ou définit une formule R1C1 de la cellule. |
| [SetR1C1Formula](./setr1c1formula/) | Obtient ou définit une formule R1C1 de la cellule. |
| [SetFormula_String_Object](./setformula_string_object/) | Définit la formule et la valeur (résultat calculé) de la formule. |
| [SetFormula_String_FormulaParseOptions](./setformula_string_formulaparseoptions/) | Définit la formule et la valeur (résultat calculé) de la formule. |
| [GetFormula_Bool_Bool](./getformula_bool_bool/) | Obtient la formule de cette cellule. |
| [SetFormula_String_FormulaParseOptions_Object](./setformula_string_formulaparseoptions_object/) | Définit la formule et la valeur (résultat calculé) de la formule. |
| [SetArrayFormula_String_Int_Int](./setarrayformula_string_int_int/) | Définit une formule matricielle (formule matricielle héritée saisie via CTRL+MAJ+ENTRÉE dans MS Excel) sur une plage de cellules. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions](./setarrayformula_string_int_int_formulaparseoptions/) | Définit une formule matricielle sur une plage de cellules. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setarrayformula_string_int_int_formulaparseoptions_object2array/) | Définit une formule matricielle sur une plage de cellules. |
| [SetSharedFormula_String_Int_Int](./setsharedformula_string_int_int/) | Définit des formules partagées sur une plage de cellules. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions](./setsharedformula_string_int_int_formulaparseoptions/) | Définit des formules partagées sur une plage de cellules. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setsharedformula_string_int_int_formulaparseoptions_object2array/) | Définit des formules partagées sur une plage de cellules. |
| [GetContainsExternalLink](./getcontainsexternallink/) | Indique si cette cellule contient un lien externe. S'applique uniquement lorsque la cellule est une cellule de formule. |
| [GetPrecedents](./getprecedents/) | Obtient toutes les références apparaissant dans la formule de cette cellule. |
| [GetDependents](./getdependents/) | Obtient toutes les cellules dont la formule fait directement référence à cette cellule. |
| [GetPrecedentsInCalculation](./getprecedentsincalculation/) | Obtient tous les antécédents (références aux cellules du classeur actuel) utilisés par la formule de cette cellule lors de son calcul. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | Obtient toutes les cellules dont le résultat calculé dépend de cette cellule. |
| [IsArrayHeader](./isarrayheader/) | Indique que la formule de la cellule est une formule matricielle et qu'elle est la première cellule du tableau. |
| [IsDynamicArrayFormula](./isdynamicarrayformula/) | Indique si la formule de la cellule est une formule matricielle dynamique (true) ou une formule matricielle héritée (false). |
| [GetArrayRange](./getarrayrange/) | Obtient la plage matricielle si la formule de la cellule est une formule matricielle. |
| [IsArrayFormula](./isarrayformula/) | Indique si la formule de la cellule est une formule matricielle. |
| [IsSharedFormula](./issharedformula/) | Indique si la formule de la cellule fait partie d'une formule partagée. |
| [IsTableFormula](./istableformula/) | Indique si cette cellule fait partie d'une formule de tableau. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Bool](./setdynamicarrayformula_string_formulaparseoptions_bool/) | Définit une formule matricielle dynamique et fait déborder la formule dans les cellules voisines si possible. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool/) | Définit une formule matricielle dynamique et fait déborder la formule dans les cellules voisines si possible. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool_CalculationOptions](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool_calculationoptions/) | Définit une formule matricielle dynamique et fait déborder la formule dans les cellules voisines si possible. |
| [SetTableFormula_Int_Int_String_String_Object2Array](./settableformula_int_int_string_string_object2array/) | Crée un tableau de données à deux variables pour la plage donnée à partir de cette cellule. |
| [SetTableFormula_Int_Int_String_Bool_Object2Array](./settableformula_int_int_string_bool_object2array/) | Crée un tableau de données à une variable pour la plage donnée à partir de cette cellule. |
| [SetTableFormula_Int_Int_Int_Int_Int_Int_Object2Array](./settableformula_int_int_int_int_int_int_object2array/) | Crée un tableau de données à deux variables pour la plage donnée à partir de cette cellule. |
| [SetTableFormula_Int_Int_Int_Int_Bool_Object2Array](./settableformula_int_int_int_int_bool_object2array/) | Crée un tableau de données à une variable pour la plage donnée à partir de cette cellule. |
| [RemoveArrayFormula](./removearrayformula/) | Supprime la formule matricielle. |
| [Copy](./copy/) | Copie les données d'une cellule source. |
| [GetValue](./getvalue/) | Obtient/définit la valeur contenue dans cette cellule. |
| [SetValue](./setvalue/) | Obtient/définit la valeur contenue dans cette cellule. |
| [IsStyleSet](./isstyleset/) | Indique si le style de la cellule est défini. Si la valeur retournée est false, cela signifie que cette cellule a un format de cellule par défaut. |
| [Characters](./characters/) | Renvoie un objet **Characters** qui représente une plage de caractères dans le texte de la cellule. |
| [Replace](./replace/) | Remplace le texte de la cellule avec des options. |
| [InsertText](./inserttext/) | Insère des caractères dans la cellule. Si la cellule est formatée en riche, cette méthode peut conserver le formatage original. |
| [IsRichText](./isrichtext/) | Indique si la valeur chaîne de cette cellule est un texte formaté en riche. |
| [GetCharacters](./getcharacters/) | Renvoie tous les objets **Characters** qui représentent une plage de caractères dans le texte de la cellule. |
| [GetCharacters_Bool](./getcharacters_bool/) | Renvoie tous les objets **Characters** qui représentent une plage de caractères dans le texte de la cellule. |
| [SetCharacters](./setcharacters/) | Définit le format de texte riche de la cellule. |
| [IsMerged](./ismerged/) | Vérifie si une cellule fait partie d'une plage fusionnée ou non. |
| [GetMergedRange](./getmergedrange/) | Renvoie un objet **Range** qui représente une plage fusionnée. |
| [GetComment](./getcomment/) | Obtient le commentaire de cette cellule. |
| [GetHtmlString](./gethtmlstring/) | Obtient et définit la chaîne HTML qui contient des données et certains formats dans cette cellule. |
| [SetHtmlString](./sethtmlstring/) | Obtient et définit la chaîne HTML qui contient des données et certains formats dans cette cellule. |
| [GetHtmlString_Bool](./gethtmlstring_bool/) | Obtient la chaîne HTML qui contient des données et certains formats dans cette cellule. |
| [ToString](./tostring/) | Renvoie une chaîne qui représente l'objet Cell actuel. |
| [ToJson](./tojson/) | Convertit la cellule en données de structure JSON. |
| [Equals_Object](./equals_object/) | Vérifie si cet objet fait référence à la même cellule qu'un autre. |
| [GetHashCode](./gethashcode/) | Servir de fonction de hachage pour un type particulier. |
| [Equals_Cell](./equals_cell/) | Vérifie si cet objet fait référence à la même cellule qu'un autre objet cellule. |
| [GetConditionalFormattingResult](./getconditionalformattingresult/) | Obtenez le résultat du formatage conditionnel. |
| [GetValidation](./getvalidation/) | Obtient la validation appliquée à cette cellule. |
| [GetValidationValue](./getvalidationvalue/) | Obtient la valeur de validation qui est appliquée à cette cellule. |
| [GetTable](./gettable/) | Obtient le tableau qui contient cette cellule. |
| [IsCheckBoxStyle](./ischeckboxstyle/) | Indique si la cellule est définie comme case à cocher. |
| [SetIsCheckBoxStyle](./setischeckboxstyle/) | Indique si la cellule est définie comme case à cocher. |
| [GetRichValue](./getrichvalue/) | Obtient la valeur riche de la cellule. |
| [GetEmbeddedImage](./getembeddedimage/) | Obtient et définit l'image intégrée dans la cellule. |
| [SetEmbeddedImage](./setembeddedimage/) | Obtient et définit l'image intégrée dans la cellule. |
| [GetPicture](./getpicture/) | Obtient une instance Aspose.Cells.Drawing.Picture pour représenter l'image incorporée dans cette cellule ou null s'il n'y a aucune image incorporée pour cette cellule. |
|[Dispose](./dispose/) |  | 
