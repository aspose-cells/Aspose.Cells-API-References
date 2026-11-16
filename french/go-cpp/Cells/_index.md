---
title: "Classe Cells"
linktitle: "Cells"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Cells. Encapsule l'objet qui représente les cellules dans Go."
type: docs
weight: 200
url: /fr/go-cpp/cells/
---

## Cells class

Encapsule une collection d'objets pertinents pour la cellule, tels que <see cref="Cell"/>, <see cref="Row"/>, etc.

```go

type Cells struct  {
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
| [GetOdsCellFields](./getodscellfields/) | Obtient la liste des champs de ods. |
| [Dispose](./dispose/) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [GetCount](./getcount/) | Obtient le nombre total d'objets Cell instanciés. |
| [GetCountLarge](./getcountlarge/) | Obtient le nombre total d'objets Cell instanciés. |
| [GetEnumerator](./getenumerator/) | Obtient l'énumérateur des cellules. |
| [GetRows](./getrows/) | Obtient la collection d'objets Row qui représente les lignes individuelles de cette feuille de calcul. |
| [GetMergedAreas](./getmergedareas/) | Obtient toutes les cellules fusionnées. |
| [CheckCell](./checkcell/) | Obtient l'élément Cell ou null à l'index de ligne et de colonne de cellule spécifié. |
| [CheckRow](./checkrow/) | Obtient l'élément Row ou null à l'index de ligne de cellule spécifié. |
| [CheckColumn](./checkcolumn/) | Obtient l'élément Column ou null à l'index de colonne spécifié. |
| [IsRowHidden](./isrowhidden/) | Vérifie si une ligne à l'index donné est masquée. |
| [IsColumnHidden](./iscolumnhidden/) | Vérifie si une colonne à l'index donné est masquée. |
| [AddRange](./addrange/) | Ajoute une référence d'objet de plage aux cellules |
| [CreateRange_String_String](./createrange_string_string/) | Crée un objet Range à partir d'une plage de cellules. |
| [CreateRange_Int_Int_Int_Int](./createrange_int_int_int_int/) | Crée un objet Range à partir d'une plage de cellules. |
| [CreateRange_String](./createrange_string/) | Crée un objet Range à partir d'une adresse de la plage. |
| [CreateRange_Int_Int_Bool](./createrange_int_int_bool/) | Crée un objet Range à partir de lignes de cellules ou de colonnes de cellules. |
| [Get_Int_Int](./get_int_int/) | Obtient l'élément Cell à l'index de ligne de cellule et d'index de colonne spécifiés. |
| [Get_String](./get_string/) | Obtient l'élément Cell au nom de cellule spécifié. |
| [GetMultiThreadReading](./getmultithreadreading/) | Obtient ou définit si le modèle de données des cellules doit prendre en charge la lecture Multi-Thread. La valeur par défaut de cette propriété est false. |
| [SetMultiThreadReading](./setmultithreadreading/) | Obtient ou définit si le modèle de données des cellules doit prendre en charge la lecture Multi-Thread. La valeur par défaut de cette propriété est false. |
| [GetMemorySetting](./getmemorysetting/) | Obtient ou définit l'option d'utilisation de la mémoire pour ces cellules. |
| [SetMemorySetting](./setmemorysetting/) | Obtient ou définit l'option d'utilisation de la mémoire pour ces cellules. |
| [Clear](./clear/) | Efface toutes les données de la feuille de calcul. |
| [GetStyle](./getstyle/) | Obtient et définit le style par défaut de la feuille de calcul. |
| [SetStyle](./setstyle/) | Obtient et définit le style par défaut de la feuille de calcul. |
|[IsDefaultColumnHidden](./isdefaultcolumnhidden/) |  | 
|[SetIsDefaultColumnHidden](./setisdefaultcolumnhidden/) |  | 
| [GetStandardWidthInch](./getstandardwidthinch/) | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en pouces. |
| [SetStandardWidthInch](./setstandardwidthinch/) | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en pouces. |
| [GetStandardWidthPixels](./getstandardwidthpixels/) | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en pixels. |
| [SetStandardWidthPixels](./setstandardwidthpixels/) | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en pixels. |
| [GetStandardWidth](./getstandardwidth/) | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en caractères. |
| [SetStandardWidth](./setstandardwidth/) | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en caractères. |
| [GetStandardHeight](./getstandardheight/) | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en points. |
| [SetStandardHeight](./setstandardheight/) | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en points. |
| [GetStandardHeightPixels](./getstandardheightpixels/) | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en pixels. |
| [SetStandardHeightPixels](./setstandardheightpixels/) | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en pixels. |
| [GetStandardHeightInch](./getstandardheightinch/) | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en pouces. |
| [SetStandardHeightInch](./setstandardheightinch/) | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en pouces. |
| [ImportFormulaArray](./importformulaarray/) | Importe un tableau de formules dans une feuille de calcul. |
| [TextToColumns](./texttocolumns/) | Divise le contenu de la colonne spécifiée en plusieurs colonnes.. |
| [ImportCSV_String_String_Bool_Int_Int](./importcsv_string_string_bool_int_int/) | Importe un fichier CSV dans les cellules. |
| [ImportCSV_Stream_String_Bool_Int_Int](./importcsv_stream_string_bool_int_int/) | Importe un fichier CSV dans les cellules. |
| [ImportCSV_String_TxtLoadOptions_Int_Int](./importcsv_string_txtloadoptions_int_int/) | Importe un fichier CSV dans les cellules. |
| [ImportCSV_Stream_TxtLoadOptions_Int_Int](./importcsv_stream_txtloadoptions_int_int/) | Importe un fichier CSV dans les cellules. |
| [GetPreserveString](./getpreservestring/) | Obtient ou définit une valeur indiquant si toutes les valeurs de la feuille de calcul sont conservées en tant que chaînes. La valeur par défaut est false. |
| [SetPreserveString](./setpreservestring/) | Obtient ou définit une valeur indiquant si toutes les valeurs de la feuille de calcul sont conservées en tant que chaînes. La valeur par défaut est false. |
| [Merge_Int_Int_Int_Int](./merge_int_int_int_int/) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [Merge_Int_Int_Int_Int_Bool](./merge_int_int_int_int_bool/) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [Merge_Int_Int_Int_Int_Bool_Bool](./merge_int_int_int_int_bool_bool/) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [UnMerge](./unmerge/) | Annule la fusion d'une plage de cellules fusionnées spécifiée. |
| [ClearMergedCells](./clearmergedcells/) | Efface toutes les plages fusionnées. |
| [HideRow](./hiderow/) | Masque une ligne. |
| [UnhideRow](./unhiderow/) | Affiche une ligne masquée. |
| [HideRows](./hiderows/) | Masque plusieurs lignes. |
| [UnhideRows](./unhiderows/) | Démasque les lignes masquées. |
| [SetRowHeightPixel](./setrowheightpixel/) | Définit la hauteur de la ligne en pixels. |
| [SetRowHeightInch](./setrowheightinch/) | Définit la hauteur de la ligne en pouces. |
| [SetRowHeight](./setrowheight/) | Définit la hauteur de la ligne spécifiée. |
| [GetRowHeight_Int_Bool_CellsUnitType](./getrowheight_int_bool_cellsunittype/) | Obtient la hauteur de la ligne. |
| [GetColumnWidth_Int_Bool_CellsUnitType](./getcolumnwidth_int_bool_cellsunittype/) | Obtient la largeur de la colonne. |
| [HideColumn](./hidecolumn/) | Masque une colonne. |
| [UnhideColumn](./unhidecolumn/) | Démasque une colonne |
| [HideColumns](./hidecolumns/) | Masque plusieurs colonnes. |
| [UnhideColumns](./unhidecolumns/) | Démasque plusieurs colonnes. |
| [GetRowHeight_Int](./getrowheight_int/) | Obtient la hauteur d'une ligne spécifiée, en points. |
| [GetViewRowHeight](./getviewrowheight/) | Obtient la hauteur d'une ligne spécifiée. |
| [GetRowHeightInch](./getrowheightinch/) | Obtient la hauteur d'une ligne spécifiée en pouces. |
| [GetViewRowHeightInch](./getviewrowheightinch/) | Obtient la hauteur d'une ligne spécifiée en pouces. |
| [GetRowHeightPixel](./getrowheightpixel/) | Obtient la hauteur d'une ligne spécifiée en pixels. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | Définit la largeur de la colonne en pixels en vue normale. |
| [SetColumnWidthInch](./setcolumnwidthinch/) | Définit la largeur de la colonne en pouces en vue normale. |
| [SetColumnWidth](./setcolumnwidth/) | Définit la largeur de la colonne spécifiée en vue normale. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | Obtient la largeur de la colonne spécifiée en vue normale, en pixels. |
| [GetColumnWidth_Int](./getcolumnwidth_int/) | Obtient la largeur (en caractères) de la colonne spécifiée en vue normale |
| [GetViewColumnWidthPixel](./getviewcolumnwidthpixel/) | Obtenez la largeur dans un type de vue différent. |
| [SetViewColumnWidthPixel](./setviewcolumnwidthpixel/) | Définit la largeur de la colonne dans une vue différente. |
| [GetMinRow](./getminrow/) | Indice de ligne minimum de la cellule qui contient des données ou un style. |
| [GetMaxRow](./getmaxrow/) | Indice de ligne maximum de la cellule qui contient des données ou un style. |
| [GetMinColumn](./getmincolumn/) | Indice de colonne minimum de ces cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée). |
| [GetMaxColumn](./getmaxcolumn/) | Indice maximal de colonne des cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée). |
| [GetMinDataRow](./getmindatarow/) | Indice minimal de ligne de la cellule qui contient des données. |
| [GetMaxDataRow](./getmaxdatarow/) | Indice maximal de ligne de la cellule qui contient des données. |
| [GetMinDataColumn](./getmindatacolumn/) | Indice minimal de colonne de la cellule qui contient des données. |
| [GetMaxDataColumn](./getmaxdatacolumn/) | Indice maximal de colonne de la cellule qui contient des données. |
| [GetLastDataRow](./getlastdatarow/) | Obtient l'indice de la dernière ligne de la cellule qui contient des données dans la colonne spécifiée. |
| [GetFirstDataRow](./getfirstdatarow/) | Obtient l'indice de la première ligne de la cellule qui contient des données dans la colonne spécifiée. |
| [IsDefaultRowHeightMatched](./isdefaultrowheightmatched/) | Indique que la hauteur de la ligne et la hauteur de police par défaut correspondent |
| [SetIsDefaultRowHeightMatched](./setisdefaultrowheightmatched/) | Indique que la hauteur de la ligne et la hauteur de police par défaut correspondent |
| [IsDefaultRowHidden](./isdefaultrowhidden/) | Indique si la ligne est masquée par défaut. |
| [SetIsDefaultRowHidden](./setisdefaultrowhidden/) | Indique si la ligne est masquée par défaut. |
| [GetColumns](./getcolumns/) | Obtient la collection d'objets Column qui représente les colonnes individuelles dans cette feuille de calcul. |
| [ApplyColumnStyle](./applycolumnstyle/) | Applique les formats à une colonne entière. |
| [ApplyRowStyle](./applyrowstyle/) | Applique les formats à une ligne entière. |
| [ApplyStyle](./applystyle/) | Applique les formats à une feuille de calcul entière. |
| [CopyColumns_Cells_Int_Int_Int_PasteOptions](./copycolumns_cells_int_int_int_pasteoptions/) | Copie les données et les formats d'une colonne entière. |
| [CopyColumn](./copycolumn/) | Copie les données et les formats d'une colonne entière. |
| [CopyColumns_Cells_Int_Int_Int](./copycolumns_cells_int_int_int/) | Copie les données et les formats de colonnes entières. |
| [CopyColumns_Cells_Int_Int_Int_Int](./copycolumns_cells_int_int_int_int/) | Copie les données et les formats de toutes les colonnes. |
| [CopyRow](./copyrow/) | Copie les données et les formats d'une ligne entière. |
| [CopyRows_Cells_Int_Int_Int](./copyrows_cells_int_int_int/) | Copie les données et les formats de certaines lignes entières. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions](./copyrows_cells_int_int_int_copyoptions/) | Copie les données et les formats de certaines lignes entières. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions_PasteOptions](./copyrows_cells_int_int_int_copyoptions_pasteoptions/) | Copie les données et les formats de certaines lignes entières. |
| [GetGroupedRowOutlineLevel](./getgroupedrowoutlinelevel/) | Obtient le niveau de contour (à base zéro) de la ligne. |
| [GetGroupedColumnOutlineLevel](./getgroupedcolumnoutlinelevel/) | Obtient le niveau de contour (à base zéro) de la colonne. |
| [GetMaxGroupedColumnOutlineLevel](./getmaxgroupedcolumnoutlinelevel/) | Obtient le niveau de contour maximal des colonnes groupées (à base zéro). |
| [GetMaxGroupedRowOutlineLevel](./getmaxgroupedrowoutlinelevel/) | Obtient le niveau de contour maximal des lignes groupées (à base zéro). |
| [ShowGroupDetail](./showgroupdetail/) | Développe les lignes/colonnes groupées. |
| [HideGroupDetail](./hidegroupdetail/) | Réduit les lignes/colonnes groupées. |
| [UngroupColumns](./ungroupcolumns/) | Dégroupe les colonnes. |
| [GroupColumns_Int_Int](./groupcolumns_int_int/) | Regroupe les colonnes. |
| [GroupColumns_Int_Int_Bool](./groupcolumns_int_int_bool/) | Regroupe les colonnes. |
| [UngroupRows_Int_Int_Bool](./ungrouprows_int_int_bool/) | Dégroupe les lignes. |
| [UngroupRows_Int_Int](./ungrouprows_int_int/) | Dégroupe les lignes. |
| [GroupRows_Int_Int_Bool](./grouprows_int_int_bool/) | Regroupe les lignes. |
| [GroupRows_Int_Int](./grouprows_int_int/) | Regroupe les lignes. |
| [DeleteColumn_Int_Bool](./deletecolumn_int_bool/) | Supprime une colonne. |
| [DeleteColumn_Int](./deletecolumn_int/) | Supprime une colonne. |
| [DeleteColumns_Int_Int_Bool](./deletecolumns_int_int_bool/) | Supprime plusieurs colonnes. |
| [DeleteColumns_Int_Int_DeleteOptions](./deletecolumns_int_int_deleteoptions/) | Supprime plusieurs colonnes. |
| [IsDeletingRangeEnabled](./isdeletingrangeenabled/) | Vérifiez si la plage peut être supprimée. |
| [DeleteRow_Int](./deleterow_int/) | Supprime une ligne. |
| [DeleteRow_Int_Bool](./deleterow_int_bool/) | Supprime une ligne. |
| [DeleteRows_Int_Int](./deleterows_int_int/) | Supprime plusieurs lignes. |
| [DeleteRows_Int_Int_Bool](./deleterows_int_int_bool/) | Supprime plusieurs lignes dans la feuille de calcul. |
| [DeleteRows_Int_Int_DeleteOptions](./deleterows_int_int_deleteoptions/) | Supprime plusieurs lignes dans la feuille de calcul. |
| [DeleteBlankColumns](./deleteblankcolumns/) | Supprime toutes les colonnes vides qui ne contiennent aucune donnée. |
| [DeleteBlankColumns_DeleteOptions](./deleteblankcolumns_deleteoptions/) | Supprime toutes les colonnes vides qui ne contiennent aucune donnée. |
| [IsBlankColumn](./isblankcolumn/) | Vérifie si la colonne donnée est vide (ne contient aucune donnée). |
| [DeleteBlankRows](./deleteblankrows/) | Supprime toutes les lignes vides qui ne contiennent aucune donnée ou aucun autre objet. |
| [DeleteBlankRows_DeleteOptions](./deleteblankrows_deleteoptions/) | Supprime toutes les lignes vides qui ne contiennent aucune donnée ou certains objets spéciaux tels que les commentaires visibles, les tableaux croisés dynamiques. |
| [InsertColumns_Int_Int](./insertcolumns_int_int/) | Insère quelques colonnes dans la feuille de calcul. |
| [InsertColumns_Int_Int_Bool](./insertcolumns_int_int_bool/) | Insère quelques colonnes dans la feuille de calcul. |
| [InsertColumns_Int_Int_InsertOptions](./insertcolumns_int_int_insertoptions/) | Insère quelques colonnes dans la feuille de calcul. |
| [InsertColumn_Int_Bool](./insertcolumn_int_bool/) | Insère une nouvelle colonne dans la feuille de calcul. |
| [InsertColumn_Int](./insertcolumn_int/) | Insère une nouvelle colonne dans la feuille de calcul. |
| [InsertRows_Int_Int_Bool](./insertrows_int_int_bool/) | Insère plusieurs lignes dans la feuille de calcul. |
| [InsertRows_Int_Int_InsertOptions](./insertrows_int_int_insertoptions/) | Insère plusieurs lignes dans la feuille de calcul. |
| [InsertRows_Int_Int](./insertrows_int_int/) | Insère plusieurs lignes dans la feuille de calcul. |
| [InsertRow](./insertrow/) | Insère une nouvelle ligne dans la feuille de calcul. |
| [GetRanges](./getranges/) | Obtient la collection d'objets Range créés à l'exécution. |
| [ClearRange_CellArea](./clearrange_cellarea/) | Efface le contenu et le formatage d'une plage. |
| [ClearRange_Int_Int_Int_Int](./clearrange_int_int_int_int/) | Efface le contenu et le formatage d'une plage. |
| [ClearContents_CellArea](./clearcontents_cellarea/) | Efface le contenu d'une plage. |
| [ClearContents_Int_Int_Int_Int](./clearcontents_int_int_int_int/) | Efface le contenu d'une plage. |
| [ClearFormats_CellArea](./clearformats_cellarea/) | Efface le formatage d'une plage. |
| [ClearFormats_Int_Int_Int_Int](./clearformats_int_int_int_int/) | Efface le formatage d'une plage. |
| [GetLastCell](./getlastcell/) | Obtient la dernière cellule de cette feuille de calcul. |
| [LinkToXmlMap](./linktoxmlmap/) | Lien vers une carte XML. |
| [GetMaxDisplayRange](./getmaxdisplayrange/) | Obtient la plage maximale qui inclut les données, les cellules fusionnées et les formes. |
| [GetFirstCell](./getfirstcell/) | Obtient la première cellule de cette feuille de calcul. |
| [Find_Object_Cell](./find_object_cell/) | Trouve la cellule contenant l'objet d'entrée. |
| [Find_Object_Cell_FindOptions](./find_object_cell_findoptions/) | Trouve la cellule contenant l'objet d'entrée. |
| [EndCellInRow_Int](./endcellinrow_int/) | Obtient la dernière cellule de cette ligne. |
| [EndCellInColumn_Int](./endcellincolumn_int/) | Obtient la dernière cellule de cette colonne. |
| [EndCellInColumn_Int_Int_Int_Int](./endcellincolumn_int_int_int_int/) | Obtient la dernière cellule avec l'indice de colonne maximal dans cette plage. |
| [EndCellInRow_Int_Int_Int_Int](./endcellinrow_int_int_int_int/) | Obtient la dernière cellule avec l'indice de ligne maximal dans cette plage. |
| [MoveRange](./moverange/) | Déplace la plage. |
| [InsertCutCells](./insertcutcells/) | Insérer la plage découpée. |
| [InsertRange_CellArea_Int_ShiftType_Bool](./insertrange_cellarea_int_shifttype_bool/) | Insère une plage de cellules et décale les cellules selon l'option de décalage. |
| [InsertRange_CellArea_ShiftType](./insertrange_cellarea_shifttype/) | Insère une plage de cellules et décale les cellules selon l'option de décalage. |
| [InsertRange_CellArea_Int_ShiftType](./insertrange_cellarea_int_shifttype/) | Insère une plage de cellules et décale les cellules selon l'option de décalage. |
| [DeleteRange](./deleterange/) | Supprime une plage de cellules et décale les cellules selon l'option de décalage. |
| [ExportArray](./exportarray/) | Exporte les données de la collection Cells vers un objet tableau à deux dimensions. |
| [RetrieveSubtotalSetting](./retrievesubtotalsetting/) | Récupère les paramètres de sous-totaux de la plage. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array](./subtotal_cellarea_int_consolidationfunction_int32array/) | Crée des sous-totaux pour la plage. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array_Bool_Bool_Bool](./subtotal_cellarea_int_consolidationfunction_int32array_bool_bool_bool/) | Crée des sous-totaux pour la plage. |
| [RemoveFormulas](./removeformulas/) | Supprime toutes les formules et les remplace par la valeur de la formule. |
| [RemoveDuplicates](./removeduplicates/) | Supprime les lignes en double dans la feuille. |
| [RemoveDuplicates_Int_Int_Int_Int](./removeduplicates_int_int_int_int/) | Supprime les valeurs en double dans la plage. |
| [RemoveDuplicates_Int_Int_Int_Int_Bool_int32Array](./removeduplicates_int_int_int_int_bool_int32array/) | Supprime les données en double de la plage. |
| [ConvertStringToNumericValue](./convertstringtonumericvalue/) | Convertit toutes les données de type chaîne de la feuille de calcul en valeur numérique si possible. |
| [GetDependents](./getdependents/) | Obtient toutes les cellules qui font référence à la cellule spécifique. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | Obtient toutes les cellules dont le résultat calculé dépend de la cellule spécifique. |
| [GetCellsWithPlaceInCellPicture](./getcellswithplaceincellpicture/) | Obtient toutes les cellules contenant une image intégrée. |
| [GetCellStyle](./getcellstyle/) | Obtient le style de la cellule donnée. |
| [GetCellDisplayStyle_Int_Int](./getcelldisplaystyle_int_int/) | Obtient le style d'affichage de la cellule donnée. |
| [GetCellDisplayStyle_Int_Int_BorderType](./getcelldisplaystyle_int_int_bordertype/) | Obtient le style d'affichage de la cellule donnée. |
