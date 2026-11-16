---
title: "PivotTable Classe"
linktitle: "PivotTable"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "PivotTable classe. Encapsule l'objet qui représente pivottable en Go."
type: docs
weight: 200
url: /fr/go-cpp/pivottable/
---

## PivotTable class

Description résumée pour le tableau croisé dynamique.

```go

type PivotTable struct  {
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
| [Dispose](./dispose/) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [GetPivotCache](./getpivotcache/) | Obtient la source de données. |
| [IsExcel2003Compatible](./isexcel2003compatible/) | Spécifie si le PivotTable est compatible avec Excel2003 lors du rafraîchissement du PivotTable, si vrai, une chaîne doit contenir au maximum 255 caractères, donc si la chaîne dépasse 255 caractères, elle sera tronquée. si faux, une chaîne n'aura pas la restriction susmentionnée. La valeur par défaut est vraie. |
| [SetIsExcel2003Compatible](./setisexcel2003compatible/) | Spécifie si le PivotTable est compatible avec Excel2003 lors du rafraîchissement du PivotTable, si vrai, une chaîne doit contenir au maximum 255 caractères, donc si la chaîne dépasse 255 caractères, elle sera tronquée. si faux, une chaîne n'aura pas la restriction susmentionnée. La valeur par défaut est vraie. |
| [GetRefreshedByWho](./getrefreshedbywho/) | Obtient le nom du dernier utilisateur qui a rafraîchi ce PivotTable |
| [GetRefreshDate](./getrefreshdate/) | Obtient la dernière date et heure à laquelle le PivotTable a été actualisé. |
| [GetPivotTableStyle](./getpivottablestyle/) | Obtient les paramètres TableStyle de ce pivot table. |
| [SetPivotTableStyle](./setpivottablestyle/) | Obtient les paramètres TableStyle de ce pivot table. |
| [GetPivotTableStyleName](./getpivottablestylename/) | Obtient ou définit le nom du style du pivot table. |
| [SetPivotTableStyleName](./setpivottablestylename/) | Obtient ou définit le nom du style du pivot table. |
| [GetPivotTableStyleType](./getpivottablestyletype/) | Obtient et définit le style intégré du pivot table. |
| [SetPivotTableStyleType](./setpivottablestyletype/) | Obtient et définit le style intégré du pivot table. |
| [CopyStyle](./copystyle/) | Copie le style nommé d'un autre pivot table. |
| [ShowReportFilterPage](./showreportfilterpage/) | Affiche toutes les pages de filtre de rapport selon le PivotField, le PivotField doit être situé dans les PageFields. |
| [ShowReportFilterPageByName](./showreportfilterpagebyname/) | Affiche toutes les pages de filtre de rapport selon le nom du PivotField, le PivotField doit être situé dans les PageFields. |
| [ShowReportFilterPageByIndex](./showreportfilterpagebyindex/) | Affiche toutes les pages de filtre de rapport selon l'index de position dans les PageFields. |
| [RemoveField_PivotFieldType_String](./removefield_pivotfieldtype_string/) | Supprime un champ d'une zone de champ spécifique. |
| [RemoveField_PivotFieldType_Int](./removefield_pivotfieldtype_int/) | Supprime un champ d'une région pivot spécifique. |
| [RemoveField_PivotFieldType_PivotField](./removefield_pivotfieldtype_pivotfield/) | Supprime le champ d'une zone de champ spécifique. |
| [AddFieldToArea_PivotFieldType_String](./addfieldtoarea_pivotfieldtype_string/) | Ajoute le champ à la zone spécifique. |
| [AddFieldToArea_PivotFieldType_Int](./addfieldtoarea_pivotfieldtype_int/) | Ajoute le champ à la zone spécifique. |
| [AddFieldToArea_PivotFieldType_PivotField](./addfieldtoarea_pivotfieldtype_pivotfield/) | Ajoute le champ à la zone spécifique. |
| [AddCalculatedField_String_String_Bool](./addcalculatedfield_string_string_bool/) | Ajoute un champ calculé au champ pivot. |
| [AddCalculatedField_String_String](./addcalculatedfield_string_string/) | Ajoute un champ calculé au champ pivot et le fait glisser vers la zone de données. |
| [GetFields](./getfields/) | Obtient la liste de champs pivot spécifique par région. |
| [GetColumnFields](./getcolumnfields/) | Renvoie un objet PivotFields qui est actuellement affiché comme champs de colonne. |
| [GetRowFields](./getrowfields/) | Renvoie un objet PivotFields qui est actuellement affiché comme champs de ligne. |
| [GetPageFields](./getpagefields/) | Renvoie un objet PivotFields qui est actuellement affiché comme champs de page. |
| [GetDataFields](./getdatafields/) | Obtient un objet PivotField qui représente tous les champs de données d'un PivotTable. Lecture seule. Il ne serait initialisé que lorsqu'il y a deux champs de données ou plus dans le DataPiovtFiels. Il n'est utilisé que pour ajouter DataPivotField à la zone ligne/colonne du PivotTable. La valeur par défaut est dans la zone ligne. |
| [GetValuesField](./getvaluesfield/) | Obtient un objet PivotField qui représente tous les champs de données d'un PivotTable. Lecture seule. Il ne serait créé que lorsqu'il y a deux champs de données ou plus dans la région Data. Par défaut, il se trouve dans la région ligne. Vous pouvez le faire glisser vers la région ligne/colonne avec la méthode PivotTable.AddFieldToArea(). |
| [GetBaseFields](./getbasefields/) | Renvoie tous les champs pivot de base du PivotTable. |
| [GetPivotFilters](./getpivotfilters/) | Renvoie tous les filtres des champs pivot du pivot table. |
| [GetButtonArea](./getbuttonarea/) | Obtient la zone contenant le bouton de champ. |
| [GetTopRightArea](./gettoprightarea/) | Représente la zone vide en haut à droite du PivotTable (en haut à gauche pour les feuilles RTL). |
| [GetFilterArea](./getfilterarea/) | Obtient la zone de la région de filtre. |
| [GetColumnRange](./getcolumnrange/) | Renvoie un objet CellArea qui représente la plage qui contient la zone de colonne dans le rapport de tableau croisé dynamique. Lecture seule. |
| [GetRowRange](./getrowrange/) | Renvoie un objet CellArea qui représente la plage qui contient la zone de ligne dans le rapport de tableau croisé dynamique. Lecture seule. |
| [GetDataBodyRange](./getdatabodyrange/) | Renvoie un objet CellArea qui représente la plage qui contient la zone de données dans la liste entre la ligne d'en-tête et la ligne d'insertion. Lecture seule. |
| [GetTableRange1](./gettablerange1/) | Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport de tableau croisé dynamique, mais n'inclut pas les champs de page. Lecture seule. |
| [GetTableRange2](./gettablerange2/) | Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport de tableau croisé dynamique, incluant les champs de page. Lecture seule. |
| [MoveTo_Int_Int](./moveto_int_int/) | Déplace le tableau croisé dynamique vers un autre emplacement dans la feuille de calcul. |
| [MoveTo_Int_Int_Int](./moveto_int_int_int/) | Déplace le tableau croisé dynamique vers un autre emplacement dans la feuille de calcul. |
| [MoveTo_String](./moveto_string/) | Déplace le tableau croisé dynamique vers un autre emplacement dans la feuille de calcul. |
| [IsGridDropZones](./isgriddropzones/) | Indique si le rapport de tableau croisé dynamique affiche la disposition classique du tableau croisé dynamique (permet de faire glisser les champs dans la grille). |
| [SetIsGridDropZones](./setisgriddropzones/) | Indique si le rapport de tableau croisé dynamique affiche la disposition classique du tableau croisé dynamique (permet de faire glisser les champs dans la grille). |
| [GetShowColumnGrandTotals](./getshowcolumngrandtotals/) | Indique s'il faut afficher les totaux généraux pour les colonnes de ce tableau croisé dynamique. |
| [SetShowColumnGrandTotals](./setshowcolumngrandtotals/) | Indique s'il faut afficher les totaux généraux pour les colonnes de ce tableau croisé dynamique. |
| [GetShowRowGrandTotals](./getshowrowgrandtotals/) | Indique s'il faut afficher les totaux généraux pour les lignes du tableau croisé dynamique. |
| [SetShowRowGrandTotals](./setshowrowgrandtotals/) | Indique s'il faut afficher les totaux généraux pour les lignes du tableau croisé dynamique. |
| [GetDisplayNullString](./getdisplaynullstring/) | Indique si le rapport de tableau croisé dynamique affiche une chaîne personnalisée lorsque la valeur est nulle. |
| [SetDisplayNullString](./setdisplaynullstring/) | Indique si le rapport de tableau croisé dynamique affiche une chaîne personnalisée lorsque la valeur est nulle. |
| [GetNullString](./getnullstring/) | Obtient la chaîne affichée dans les cellules contenant des valeurs nulles lorsque la propriété DisplayNullString est vraie. La valeur par défaut est une chaîne vide. |
| [SetNullString](./setnullstring/) | Obtient la chaîne affichée dans les cellules contenant des valeurs nulles lorsque la propriété DisplayNullString est vraie. La valeur par défaut est une chaîne vide. |
| [GetDisplayErrorString](./getdisplayerrorstring/) | Indique si le rapport de tableau croisé dynamique affiche une chaîne personnalisée dans les cellules contenant des erreurs. |
| [SetDisplayErrorString](./setdisplayerrorstring/) | Indique si le rapport de tableau croisé dynamique affiche une chaîne personnalisée dans les cellules contenant des erreurs. |
| [GetDataFieldHeaderName](./getdatafieldheadername/) | Obtient et définit le nom de l'en-tête du champ de zone de valeur dans le tableau croisé dynamique. |
| [SetDataFieldHeaderName](./setdatafieldheadername/) | Obtient et définit le nom de l'en-tête du champ de zone de valeur dans le tableau croisé dynamique. |
| [GetErrorString](./geterrorstring/) | Obtient la chaîne affichée dans les cellules contenant des erreurs lorsque la propriété DisplayErrorString est vraie. La valeur par défaut est une chaîne vide. |
| [SetErrorString](./seterrorstring/) | Obtient la chaîne affichée dans les cellules contenant des erreurs lorsque la propriété DisplayErrorString est vraie. La valeur par défaut est une chaîne vide. |
| [IsAutoFormat](./isautoformat/) | Indique si le rapport de tableau croisé dynamique est formaté automatiquement. Case à cocher "autoformat table" qui se trouve dans l'option tableau croisé dynamique pour Excel 2003. |
| [SetIsAutoFormat](./setisautoformat/) | Indique si le rapport de tableau croisé dynamique est formaté automatiquement. Case à cocher "autoformat table" qui se trouve dans l'option tableau croisé dynamique pour Excel 2003. |
| [GetAutofitColumnWidthOnUpdate](./getautofitcolumnwidthonupdate/) | Indique s'il faut ajuster automatiquement la largeur des colonnes lors de la mise à jour. |
| [SetAutofitColumnWidthOnUpdate](./setautofitcolumnwidthonupdate/) | Indique s'il faut ajuster automatiquement la largeur des colonnes lors de la mise à jour. |
| [GetAutoFormatType](./getautoformattype/) | Obtient et définit le type de formatage automatique du tableau croisé dynamique. |
| [SetAutoFormatType](./setautoformattype/) | Obtient et définit le type de formatage automatique du tableau croisé dynamique. |
| [GetMergeLabels](./getmergelabels/) | Indique si les titres de lignes ou de colonnes qui s'étendent sur plusieurs cellules doivent être fusionnés en une seule cellule. |
| [SetMergeLabels](./setmergelabels/) | Indique si les titres de lignes ou de colonnes qui s'étendent sur plusieurs cellules doivent être fusionnés en une seule cellule. |
| [GetPreserveCellFormattingOnUpdate](./getpreservecellformattingonupdate/) | Indique s'il faut conserver le format des cellules (PivotTableFormat) lorsque le tableau croisé dynamique est actualisé ou recalculé. |
| [SetPreserveCellFormattingOnUpdate](./setpreservecellformattingonupdate/) | Indique s'il faut conserver le format des cellules (PivotTableFormat) lorsque le tableau croisé dynamique est actualisé ou recalculé. |
| [GetShowDrill](./getshowdrill/) | Obtient et définit l'affichage des boutons d'extension/réduction. |
| [SetShowDrill](./setshowdrill/) | Obtient et définit l'affichage des boutons d'extension/réduction. |
| [GetEnableDrilldown](./getenabledrilldown/) | Indique si le forage (drilldown) est activé. |
| [SetEnableDrilldown](./setenabledrilldown/) | Indique si le forage (drilldown) est activé. |
| [GetEnableFieldDialog](./getenablefielddialog/) | Indique si la boîte de dialogue Champ du tableau croisé dynamique est disponible lorsque l'utilisateur double-clique sur le champ du tableau croisé dynamique. |
| [SetEnableFieldDialog](./setenablefielddialog/) | Indique si la boîte de dialogue Champ du tableau croisé dynamique est disponible lorsque l'utilisateur double-clique sur le champ du tableau croisé dynamique. |
| [GetEnableFieldList](./getenablefieldlist/) | Indique si la liste des champs du tableau croisé dynamique est disponible dans la vue d'Excel. |
| [SetEnableFieldList](./setenablefieldlist/) | Indique si la liste des champs du tableau croisé dynamique est disponible dans la vue d'Excel. |
| [GetEnableWizard](./getenablewizard/) | Indique si l'assistant de tableau croisé dynamique est disponible. |
| [SetEnableWizard](./setenablewizard/) | Indique si l'assistant de tableau croisé dynamique est disponible. |
| [GetSubtotalHiddenPageItems](./getsubtotalhiddenpageitems/) | Indique si les éléments de champ de page masqués dans le rapport de tableau croisé dynamique sont inclus dans les sous-totaux de lignes et de colonnes, les totaux de bloc et les totaux généraux. La valeur par défaut est False. |
| [SetSubtotalHiddenPageItems](./setsubtotalhiddenpageitems/) | Indique si les éléments de champ de page masqués dans le rapport de tableau croisé dynamique sont inclus dans les sous-totaux de lignes et de colonnes, les totaux de bloc et les totaux généraux. La valeur par défaut est False. |
| [GetGrandTotalName](./getgrandtotalname/) | Renvoie l'étiquette affichée dans l'en-tête de colonne ou de ligne du total général. La valeur par défaut est la chaîne "Grand Total". |
| [SetGrandTotalName](./setgrandtotalname/) | Renvoie l'étiquette affichée dans l'en-tête de colonne ou de ligne du total général. La valeur par défaut est la chaîne "Grand Total". |
| [GetManualUpdate](./getmanualupdate/) | Indique si le rapport de tableau croisé dynamique est recalculé uniquement à la demande de l'utilisateur. |
| [SetManualUpdate](./setmanualupdate/) | Indique si le rapport de tableau croisé dynamique est recalculé uniquement à la demande de l'utilisateur. |
| [GetAllowMultipleFiltersPerField](./getallowmultiplefiltersperfield/) | Spécifie une valeur booléenne qui indique si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués. |
| [SetAllowMultipleFiltersPerField](./setallowmultiplefiltersperfield/) | Spécifie une valeur booléenne qui indique si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués. |
| [GetEnableDataValueEditing](./getenabledatavalueediting/) | Spécifie une valeur booléenne qui indique si l'utilisateur est autorisé à modifier les cellules de la zone de données du tableau croisé dynamique. Active la modification des cellules dans la zone des valeurs. |
| [SetEnableDataValueEditing](./setenabledatavalueediting/) | Spécifie une valeur booléenne qui indique si l'utilisateur est autorisé à modifier les cellules de la zone de données du tableau croisé dynamique. Active la modification des cellules dans la zone des valeurs. |
| [GetShowDataTips](./getshowdatatips/) | Indique si les infobulles doivent être affichées pour les cellules de données du tableau croisé dynamique. |
| [SetShowDataTips](./setshowdatatips/) | Indique si les infobulles doivent être affichées pour les cellules de données du tableau croisé dynamique. |
| [GetShowMemberPropertyTips](./getshowmemberpropertytips/) | Spécifie une valeur booléenne qui indique si les informations de propriété des membres doivent être omises des infobulles du tableau croisé dynamique. |
| [SetShowMemberPropertyTips](./setshowmemberpropertytips/) | Spécifie une valeur booléenne qui indique si les informations de propriété des membres doivent être omises des infobulles du tableau croisé dynamique. |
| [GetShowValuesRow](./getshowvaluesrow/) | Indique si la ligne des valeurs est affichée. |
| [SetShowValuesRow](./setshowvaluesrow/) | Indique si la ligne des valeurs est affichée. |
| [GetShowEmptyCol](./getshowemptycol/) | Indique s'il faut inclure les colonnes vides dans le tableau. |
| [SetShowEmptyCol](./setshowemptycol/) | Indique s'il faut inclure les colonnes vides dans le tableau. |
| [GetShowEmptyRow](./getshowemptyrow/) | Indique s'il faut inclure les lignes vides dans le tableau. |
| [SetShowEmptyRow](./setshowemptyrow/) | Indique s'il faut inclure les lignes vides dans le tableau. |
| [GetFieldListSortAscending](./getfieldlistsortascending/) | Indique si les champs du tableau croisé dynamique sont triés dans un ordre non par défaut dans la liste des champs. |
| [SetFieldListSortAscending](./setfieldlistsortascending/) | Indique si les champs du tableau croisé dynamique sont triés dans un ordre non par défaut dans la liste des champs. |
| [GetPrintDrill](./getprintdrill/) | Spécifie une valeur booléenne qui indique si les indicateurs de forage doivent être imprimés. Imprime les boutons d'expansion/réduction lorsqu'ils sont affichés sur le tableau croisé dynamique. |
| [SetPrintDrill](./setprintdrill/) | Spécifie une valeur booléenne qui indique si les indicateurs de forage doivent être imprimés. Imprime les boutons d'expansion/réduction lorsqu'ils sont affichés sur le tableau croisé dynamique. |
| [GetAltTextTitle](./getalttexttitle/) | Obtient et définit le titre du texte alternatif. |
| [SetAltTextTitle](./setalttexttitle/) | Obtient et définit le titre du texte alternatif. |
| [GetAltTextDescription](./getalttextdescription/) | Obtient la description du texte alternatif. |
| [SetAltTextDescription](./setalttextdescription/) | Obtient la description du texte alternatif. |
| [GetName](./getname/) | Obtient le nom du tableau croisé dynamique. |
| [SetName](./setname/) | Obtient le nom du tableau croisé dynamique. |
| [GetColumnHeaderCaption](./getcolumnheadercaption/) | Obtient et définit la légende personnalisée de l'en-tête de colonne du tableau croisé dynamique. |
| [SetColumnHeaderCaption](./setcolumnheadercaption/) | Obtient et définit la légende personnalisée de l'en-tête de colonne du tableau croisé dynamique. |
| [GetIndent](./getindent/) | Spécifie l'incrément d'indentation pour l'axe compact et peut être utilisé pour définir la mise en page du rapport en forme compacte. |
| [SetIndent](./setindent/) | Spécifie l'incrément d'indentation pour l'axe compact et peut être utilisé pour définir la mise en page du rapport en forme compacte. |
| [GetRowHeaderCaption](./getrowheadercaption/) | Obtient et définit la légende personnalisée de l'en-tête de ligne dans ce tableau croisé dynamique. |
| [SetRowHeaderCaption](./setrowheadercaption/) | Obtient et définit la légende personnalisée de l'en-tête de ligne dans ce tableau croisé dynamique. |
| [GetShowHeaders](./getshowheaders/) | Indique s'il faut afficher les légendes des champs de données et les légendes des champs de tableau croisé sur l'axe des lignes et l'axe des colonnes dans la vue du tableau croisé dynamique. |
| [SetShowHeaders](./setshowheaders/) | Indique s'il faut afficher les légendes des champs de données et les légendes des champs de tableau croisé sur l'axe des lignes et l'axe des colonnes dans la vue du tableau croisé dynamique. |
| [GetCustomListSort](./getcustomlistsort/) | Indique s'il faut prendre en compte la liste personnalisée intégrée lors du tri des données. |
| [SetCustomListSort](./setcustomlistsort/) | Indique s'il faut prendre en compte la liste personnalisée intégrée lors du tri des données. |
| [GetConditionalFormats](./getconditionalformats/) | Obtient les formats conditionnels du tableau croisé dynamique. |
| [GetPageFieldOrder](./getpagefieldorder/) | Obtient et définit l'ordre dans lequel les champs de page sont ajoutés à la mise en page du rapport du tableau croisé dynamique. |
| [SetPageFieldOrder](./setpagefieldorder/) | Obtient et définit l'ordre dans lequel les champs de page sont ajoutés à la mise en page du rapport du tableau croisé dynamique. |
| [GetPageFieldWrapCount](./getpagefieldwrapcount/) | Obtient le nombre de champs de page dans chaque colonne ou ligne du rapport du tableau croisé dynamique. |
| [SetPageFieldWrapCount](./setpagefieldwrapcount/) | Obtient le nombre de champs de page dans chaque colonne ou ligne du rapport du tableau croisé dynamique. |
| [GetTag](./gettag/) | Obtient et définit une chaîne définie par l'utilisateur associée à cette vue du tableau croisé dynamique. |
| [SetTag](./settag/) | Obtient et définit une chaîne définie par l'utilisateur associée à cette vue du tableau croisé dynamique. |
| [GetSaveData](./getsavedata/) | Indique si les données du rapport du tableau croisé dynamique sont enregistrées avec le classeur. |
| [SetSaveData](./setsavedata/) | Indique si les données du rapport du tableau croisé dynamique sont enregistrées avec le classeur. |
| [GetRefreshDataOnOpeningFile](./getrefreshdataonopeningfile/) | Indique si les données doivent être rafraîchies lors de l'ouverture du fichier. |
| [SetRefreshDataOnOpeningFile](./setrefreshdataonopeningfile/) | Indique si les données doivent être rafraîchies lors de l'ouverture du fichier. |
| [GetSourceType](./getsourcetype/) | Obtient le type de source de données du tableau croisé dynamique. |
| [GetSourceDataConnections](./getsourcedataconnections/) | Obtient les sources de données de connexion externes. |
| [GetNamesOfSourceDataConnections](./getnamesofsourcedataconnections/) | Obtient les noms des connexions de sources de données externes. |
| [GetDataSource](./getdatasource/) | Obtient et définit la source de données du tableau croisé dynamique. |
| [SetDataSource](./setdatasource/) | Obtient et définit la source de données du tableau croisé dynamique. |
| [ChangeDataSource](./changedatasource/) | Modifie la source de données du tableau croisé dynamique. |
| [GetSource](./getsource/) | Obtenez la source de données de ce tableau croisé dynamique. |
| [GetSource_Bool](./getsource_bool/) | Obtenez la source de données de ce tableau croisé dynamique. |
| [Refresh](./refresh/) | Actualise le PivotCache à partir de la source de données et calcule les données et le style pour la vue du tableau croisé dynamique. |
| [CalculateData](./calculatedata/) | Calcule les données du tableau croisé dynamique dans les cellules. |
| [CalculateData_PivotTableCalculateOption](./calculatedata_pivottablecalculateoption/) | Calcule le tableau croisé dynamique avec des options. |
| [GetPivotTablesWithSamePivotCache](./getpivottableswithsamepivotcache/) | Obtient tous les tableaux croisés dynamiques partageant le même cache de pivot. |
| [ClearData](./cleardata/) | Efface les données et le formatage de la vue du tableau croisé dynamique. |
| [ClearFilters](./clearfilters/) | Efface tous les filtres de ce tableau croisé dynamique. |
| [ClearAll](./clearall/) | Supprime tous les champs des régions. |
| [CalculateRange](./calculaterange/) | Calcule la plage du tableau croisé dynamique. |
| [FormatAll](./formatall/) | Formate toutes les cellules de la zone du tableau croisé dynamique |
| [FormatRow](./formatrow/) | Formate les données de ligne dans la zone du tableau croisé dynamique |
| [Format_PivotArea_Style](./format_pivotarea_style/) | Formate la zone sélectionnée du tableau croisé dynamique. |
| [Format_CellArea_Style](./format_cellarea_style/) | Formate la zone sélectionnée du tableau croisé dynamique. |
| [Format_Int_Int_Style](./format_int_int_style/) | Formate la cellule de la zone du tableau croisé dynamique |
| [SelectArea](./selectarea/) | Sélectionnez une zone de la vue du tableau croisé dynamique. |
| [ShowDetail](./showdetail/) | Affiche le détail d'un élément de la région de données dans un nouveau tableau. |
| [GetPivotFormats](./getpivotformats/) | Obtient tous les formats appliqués au tableau croisé dynamique. |
| [GetRepeatItemsOnEachPrintedPage](./getrepeatitemsoneachprintedpage/) | Indique si les légendes des éléments de pivot dans la zone de lignes sont répétées sur chaque page imprimée pour les champs de pivot sous forme tabulaire. |
| [SetRepeatItemsOnEachPrintedPage](./setrepeatitemsoneachprintedpage/) | Indique si les légendes des éléments de pivot dans la zone de lignes sont répétées sur chaque page imprimée pour les champs de pivot sous forme tabulaire. |
| [GetPrintTitles](./getprinttitles/) | Indique si les titres d'impression de la feuille de calcul sont définis en fonction du rapport du tableau croisé dynamique. La valeur par défaut est false. |
| [SetPrintTitles](./setprinttitles/) | Indique si les titres d'impression de la feuille de calcul sont définis en fonction du rapport du tableau croisé dynamique. La valeur par défaut est false. |
| [GetDisplayImmediateItems](./getdisplayimmediateitems/) | Indique si les éléments des zones de lignes et de colonnes sont visibles lorsque la zone de données du tableau croisé dynamique est vide. La valeur par défaut est true. |
| [SetDisplayImmediateItems](./setdisplayimmediateitems/) | Indique si les éléments des zones de lignes et de colonnes sont visibles lorsque la zone de données du tableau croisé dynamique est vide. La valeur par défaut est true. |
| [IsSelected](./isselected/) | Indique si ce tableau croisé dynamique est sélectionné. |
| [SetIsSelected](./setisselected/) | Indique si ce tableau croisé dynamique est sélectionné. |
| [GetShowPivotStyleRowHeader](./getshowpivotstylerowheader/) | Indique si l'en-tête de ligne du tableau croisé dynamique doit avoir le style appliqué. |
| [SetShowPivotStyleRowHeader](./setshowpivotstylerowheader/) | Indique si l'en-tête de ligne du tableau croisé dynamique doit avoir le style appliqué. |
| [GetShowPivotStyleColumnHeader](./getshowpivotstylecolumnheader/) | Indique si l'en-tête de colonne du tableau croisé dynamique doit avoir le style appliqué. |
| [SetShowPivotStyleColumnHeader](./setshowpivotstylecolumnheader/) | Indique si l'en-tête de colonne du tableau croisé dynamique doit avoir le style appliqué. |
| [GetShowPivotStyleRowStripes](./getshowpivotstylerowstripes/) | Indique si le formatage en bandes de lignes est appliqué. |
| [SetShowPivotStyleRowStripes](./setshowpivotstylerowstripes/) | Indique si le formatage en bandes de lignes est appliqué. |
| [GetShowPivotStyleColumnStripes](./getshowpivotstylecolumnstripes/) | Indique si le formatage en bandes est appliqué pour la colonne. |
| [SetShowPivotStyleColumnStripes](./setshowpivotstylecolumnstripes/) | Indique si le formatage en bandes est appliqué pour la colonne. |
| [GetShowPivotStyleLastColumn](./getshowpivotstylelastcolumn/) | Indique si le formatage de colonne est appliqué. |
| [SetShowPivotStyleLastColumn](./setshowpivotstylelastcolumn/) | Indique si le formatage de colonne est appliqué. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Obtient les sauts de page horizontaux de ce tableau croisé dynamique. |
| [ShowInCompactForm](./showincompactform/) | Disposition de la vue du tableau croisé dynamique sous forme compacte. |
| [ShowInOutlineForm](./showinoutlineform/) | Disposition du tableau croisé dynamique sous forme de plan. |
| [ShowInTabularForm](./showintabularform/) | Disposition du tableau croisé dynamique sous forme tabulaire. |
| [GetCellByDisplayName](./getcellbydisplayname/) | Obtient l'objet Cell par le nom d'affichage du PivotField. |
| [GetDependentPivotTables](./getdependentpivottables/) | Obtient tous les PivotTables qui utilisent ce PivotTable comme source de données. |
| [ExportViewToJson](./exportviewtojson/) | Exporte la vue pivot en JSON. |
