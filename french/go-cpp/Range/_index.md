---
title: "Range Classe"
linktitle: "Range"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Range classe. Encapsule l'objet qui représente range en Go."
type: docs
weight: 200
url: /fr/go-cpp/range/
---

## Range class

Encapsule l'objet qui représente une plage de cellules dans une feuille de calcul.

```go

type Range struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewRange_CellArea_Cells](./newrange_cellarea_cells/) | Constructeur de classe. |
| [NewRange_Int_Int_Int_Int_Cells](./newrange_int_int_int_int_cells/) | Constructeur de classe. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [AutoFill_Range](./autofill_range/) | Remplit automatiquement la plage cible. |
| [AutoFill_Range_AutoFillType](./autofill_range_autofilltype/) | Remplit automatiquement la plage cible. |
| [GetCurrentRegion](./getcurrentregion/) | Renvoie un objet Range qui représente la région actuelle. La région actuelle est une plage délimitée par toute combinaison de lignes vides et de colonnes vides. |
| [GetHyperlinks](./gethyperlinks/) | Obtient tous les hyperliens dans la plage. |
| [AddHyperlink](./addhyperlink/) | Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules. |
| [GetEnumerator](./getenumerator/) | Obtient l'énumérateur des cellules de cette Range. |
| [IsIntersect](./isintersect/) | Indique si la plage intersecte. |
| [Intersect](./intersect/) | Renvoie un objet Range qui représente l'intersection rectangulaire de deux plages. |
| [UnionRanges](./unionranges/) | Renvoie le résultat de l'union de deux plages. |
| [GetRowCount](./getrowcount/) | Obtient le nombre de lignes dans la plage. |
| [GetColumnCount](./getcolumncount/) | Obtient le nombre de colonnes dans la plage. |
| [GetName](./getname/) | Obtient ou définit le nom de la plage. |
| [SetName](./setname/) | Obtient ou définit le nom de la plage. |
| [GetRefersTo](./getrefersto/) | Obtient la référence de la plage. |
| [GetAddress](./getaddress/) | Obtient l'adresse de la plage. |
| [IsBlank](./isblank/) | Indique si la plage contient des valeurs. |
| [GetLeft](./getleft/) | Obtient la distance, en points, du bord gauche de la colonne A au bord gauche de la plage. |
| [GetTop](./gettop/) | Obtient la distance, en points, du bord supérieur de la ligne 1 au bord supérieur de la plage. |
| [GetWidth](./getwidth/) | Obtient la largeur d'une plage en points. |
| [GetHeight](./getheight/) | Obtient la largeur d'une plage en points. |
| [GetFirstRow](./getfirstrow/) | Obtient l'index de la première ligne de la plage. |
| [GetFirstColumn](./getfirstcolumn/) | Obtient l'index de la première colonne de la plage. |
| [Merge](./merge/) | Combine une plage de cellules en une seule cellule. |
| [UnMerge](./unmerge/) | Démarque les cellules fusionnées de cette plage. |
| [PutValue](./putvalue/) | Place une valeur dans la plage, le cas échéant la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [GetValue](./getvalue/) | Obtient et définit la valeur de la plage. |
| [SetValue](./setvalue/) | Obtient et définit la valeur de la plage. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | Applique le style de cellule. |
| [ApplyStyle](./applystyle/) | Applique des formats à l'ensemble d'une plage. |
| [SetStyle_Style](./setstyle_style/) | Définit le style de la plage. |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | Définit les bordures de contour autour d'une plage de cellules avec le même style et la même couleur de bordure. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Définit les bordures de contour autour d'une plage de cellules avec le même style et la même couleur de bordure. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Définit les bordures de contour autour d'une plage de cellules. |
| [SetOutlineBorder_BorderType_CellBorderType_CellsColor](./setoutlineborder_bordertype_cellbordertype_cellscolor/) | Définit la bordure de contour autour d'une plage de cellules. |
| [SetOutlineBorder_BorderType_CellBorderType_Color](./setoutlineborder_bordertype_cellbordertype_color/) | Définit la bordure de contour autour d'une plage de cellules. |
| [SetInsideBorders](./setinsideborders/) | Définit les bordures internes de la plage. |
| [GetColumnWidth](./getcolumnwidth/) | Définit ou obtient la largeur de colonne de cette plage |
| [SetColumnWidth](./setcolumnwidth/) | Définit ou obtient la largeur de colonne de cette plage |
| [GetRowHeight](./getrowheight/) | Définit ou obtient la hauteur des lignes dans cette plage |
| [SetRowHeight](./setrowheight/) | Définit ou obtient la hauteur des lignes dans cette plage |
| [MoveTo](./moveto/) | Déplace la plage actuelle vers la plage de destination. |
| [CopyData](./copydata/) | Copie les données de cellule (y compris les formules) d'une plage source. |
| [CopyValue](./copyvalue/) | Copie la valeur de cellule d'une plage source. |
| [CopyStyle](./copystyle/) | Copie les paramètres de style d'une plage source. |
| [Copy_Range_PasteOptions](./copy_range_pasteoptions/) | Copie la plage avec les options de collage spécial. |
| [Transpose](./transpose/) | Transpose (fait pivoter) les données des lignes vers les colonnes ou inversement. |
| [Copy_Range](./copy_range/) | Copie les données (y compris les formules), le formatage, les objets de dessin, etc. d'une plage source. |
| [Get](./get/) | Obtient l'objet Cell dans cette plage. |
| [GetCellOrNull](./getcellornull/) | Obtient l'objet Cell ou null dans cette plage. |
| [GetOffset](./getoffset/) | Obtient la plage Range par décalage. |
| [GetEntireColumn](./getentirecolumn/) | Obtient un objet Range qui représente la colonne entière (ou les colonnes) contenant la plage spécifiée. |
| [GetEntireRow](./getentirerow/) | Obtient un objet Range qui représente la ligne entière (ou les lignes) contenant la plage spécifiée. |
| [GetWorksheet](./getworksheet/) | Obtient l'objet Worksheetobject qui contient cette plage. |
| [ToString](./tostring/) | Renvoie une chaîne qui représente l'objet Range actuel. |
| [ToImage](./toimage/) | Convertit la plage en image. |
| [ToJson](./tojson/) | Convertit la plage en valeur JSON. |
| [ToHtml](./tohtml/) | Convertit la plage en HTML. |
| [Clear](./clear/) | Efface cette plage. |
| [ClearContents](./clearcontents/) | Efface le contenu de cette plage. |
| [ClearFormats](./clearformats/) | Efface les formats de cette plage. |
| [ClearComments](./clearcomments/) | Efface les commentaires de cette plage. |
| [ClearHyperlinks](./clearhyperlinks/) | Supprime uniquement les hyperliens. |
