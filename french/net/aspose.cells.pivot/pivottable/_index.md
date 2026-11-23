---
title: "Classe PivotTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotTable. Description résumée pour PivotTable"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

Description résumée pour le **PivotTable**.

```csharp
public class PivotTable : IDisposable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AllowMultipleFiltersPerField](../../aspose.cells.pivot/pivottable/allowmultiplefiltersperfield/) { get; set; } | Spécifie une valeur booléenne qui indique si les champs d’un PivotTable peuvent avoir plusieurs filtres appliqués. |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription/) { get; set; } | Obtient la description du texte alternatif. |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle/) { get; set; } | Obtient et définit le titre du texte alternatif. |
| [AutofitColumnWidthOnUpdate](../../aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/) { get; set; } | Indique s’il faut ajuster automatiquement la largeur des colonnes lors de la mise à jour |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype/) { get; set; } | Obtient et définit le type de format automatique du PivotTable. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields/) { get; } | Renvoie tous les champs pivot de base du PivotTable. |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields/) { get; } | Renvoie un objet PivotFields qui est actuellement affiché comme champs de colonne. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand/) { get; set; } | (**Obsolete.**) Indique si le rapport PivotTable affiche les totaux généraux pour les colonnes. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption/) { get; set; } | Obtient et définit la légende personnalisée de l’en-tête de colonne du PivotTable. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange/) { get; } | Renvoie un objet CellArea qui représente la plage contenant la zone de colonne dans le rapport PivotTable. Lecture seule. |
| [ConditionalFormats](../../aspose.cells.pivot/pivottable/conditionalformats/) { get; } | Obtient les formats conditionnels du tableau croisé dynamique. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort/) { get; set; } | Indique s’il faut prendre en compte la liste personnalisée intégrée lors du tri des données |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange/) { get; } | Renvoie un objet [`CellArea`](../../aspose.cells/cellarea/) qui représente la plage contenant la zone de données dans la liste entre la ligne d’en-tête et la ligne d’insertion. Lecture seule. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield/) { get; } | (**Obsolete.**) Obtient un objet [`PivotField`](../pivotfield/) qui représente tous les champs de données d’un PivotTable. Lecture seule. Il ne serait créé que lorsqu’il y a deux champs de données ou plus dans la région Data. Par défaut, il se trouve dans la région des lignes. Vous pouvez le faire glisser vers la région ligne/colonne avec la méthode PivotTable.AddFieldToArea(). |
| [DataFieldHeaderName](../../aspose.cells.pivot/pivottable/datafieldheadername/) { get; set; } | Obtient et définit le nom de l’en-tête du champ de la zone de valeurs dans le PivotTable. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields/) { get; } | Obtient une [`PivotFieldCollection`](../pivotfieldcollection/) qui représente tous les champs de données d’un PivotTable. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource/) { get; set; } | Obtient et définit la source de données du tableau croisé dynamique. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring/) { get; set; } | Indique si le rapport PivotTable affiche une chaîne personnalisée dans les cellules contenant des erreurs. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems/) { get; set; } | Indique si les éléments des zones de lignes et de colonnes sont visibles lorsque la zone de données du PivotTable est vide. La valeur par défaut est true. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring/) { get; set; } | Indique si le rapport PivotTable affiche une chaîne personnalisée lorsque la valeur est nulle. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting/) { get; set; } | Spécifie une valeur booléenne qui indique si l’utilisateur est autorisé à modifier les cellules de la zone de données du pivottable. La valeur par défaut est false. |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown/) { get; set; } | Indique si le drilldown est activé. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog/) { get; set; } | Indique si la boîte de dialogue Champ de tableau croisé dynamique est disponible lorsque l'utilisateur double-clique sur le champ du tableau croisé dynamique. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist/) { get; set; } | Indique si la liste des champs du tableau croisé dynamique est disponible dans la vue d'Excel. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard/) { get; set; } | Indique si l'assistant Tableau croisé dynamique est disponible. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring/) { get; set; } | Obtient la chaîne affichée dans les cellules contenant des erreurs lorsque la propriété DisplayErrorString est vraie. La valeur par défaut est une chaîne vide. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource/) { get; } | (**Obsolète.**) Obtient la source de données de connexion externe. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending/) { get; set; } | Indique si les champs du tableau croisé dynamique sont triés dans un ordre non par défaut dans la liste des champs. |
| [FilterArea](../../aspose.cells.pivot/pivottable/filterarea/) { get; } | Obtient la zone de la région de filtre. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname/) { get; set; } | Renvoie l'étiquette affichée dans l'en-tête de colonne ou de ligne du total général. La valeur par défaut est la chaîne "Grand Total". |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows/) { get; set; } | (**Obsolète.**) Indique s'il faut ajouter des lignes vides. Cette propriété ne s'applique qu'aux types de mise en forme automatique du tableau croisé dynamique qui nécessitent d'ajouter des lignes vides. |
| [Indent](../../aspose.cells.pivot/pivottable/indent/) { get; set; } | Spécifie l'incrément d'indentation pour l'axe compact et peut être utilisé pour définir la mise en page du rapport en forme compacte. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat/) { get; set; } | Indique si le rapport du tableau croisé dynamique est formaté automatiquement. Case à cocher "autoformat table" qui se trouve dans les options du tableau croisé dynamique pour Excel 2003. |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible/) { get; set; } | Spécifie si le tableau croisé dynamique est compatible avec Excel2003 lors du rafraîchissement. Si vrai, une chaîne doit contenir au maximum 255 caractères ; si la chaîne dépasse 255 caractères, elle sera tronquée. Si faux, aucune restriction de ce type ne s'applique. La valeur par défaut est vraie. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones/) { get; set; } | Indique si le rapport du tableau croisé dynamique affiche la disposition classique du tableau croisé dynamique. (permet de faire glisser les champs dans la grille) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters/) { get; set; } | (**Obsolète.**) Spécifie une valeur booléenne qui indique si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected/) { get; set; } | Indique si ce tableau croisé dynamique est sélectionné. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles/) { get; set; } | (**Obsolète.**) Indique si les noms de PivotItem doivent être répétés en haut de chaque page imprimée. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate/) { get; set; } | Indique si le rapport du tableau croisé dynamique est recalculé uniquement à la demande de l'utilisateur. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels/) { get; set; } | Obtient ou définit s'il faut fusionner les étiquettes de champs ligne/colonne qui s'étendent sur plusieurs cellules. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit/) { get; set; } | (**Obsolète.**) Spécifie une valeur booléenne qui indique si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres appliqués. |
| [Name](../../aspose.cells.pivot/pivottable/name/) { get; set; } | Obtient le nom du tableau croisé dynamique |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring/) { get; set; } | Obtient la chaîne affichée dans les cellules contenant des valeurs nulles lorsque la propriété DisplayNullString est vraie. La valeur par défaut est une chaîne vide. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder/) { get; set; } | Obtient et définit l'ordre dans lequel les champs de page sont ajoutés à la mise en page du rapport du tableau croisé dynamique. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields/) { get; } | Renvoie une [`PivotFieldCollection`](../pivotfieldcollection/) qui sont actuellement affichés comme champs de page. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount/) { get; set; } | Obtient le nombre de champs de page dans chaque colonne ou ligne du rapport du tableau croisé dynamique. |
| [PivotCache](../../aspose.cells.pivot/pivottable/pivotcache/) { get; } | Obtient la source de données. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters/) { get; } | Renvoie tous les filtres du tableau croisé dynamique. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions/) { get; } | (**Obsolète.**) Obtient les conditions de format du tableau croisé dynamique. |
| [PivotFormats](../../aspose.cells.pivot/pivottable/pivotformats/) { get; } | Obtient tous les formats de cellule appliqués à ce tableau croisé dynamique. |
| [PivotTableStyle](../../aspose.cells.pivot/pivottable/pivottablestyle/) { get; set; } | Obtient les paramètres TableStyle de ce tableau croisé dynamique. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename/) { get; set; } | Obtient ou définit le nom du style du tableau croisé dynamique. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype/) { get; set; } | Obtient et définit le style intégré du tableau croisé dynamique. |
| [PreserveCellFormattingOnUpdate](../../aspose.cells.pivot/pivottable/preservecellformattingonupdate/) { get; set; } | Indique s'il faut conserver le format des cellules ([`PivotTableFormat`](../pivottableformat/)) lorsque le tableau croisé dynamique est actualisé ou recalculé. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting/) { get; set; } | (**Obsolète.**) Indique si le format des cellules ([`PivotTableFormat`](../pivottableformat/)) est conservé lorsque le PivotTable est actualisé ou recalculé. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill/) { get; set; } | Spécifie une valeur booléenne indiquant si les indicateurs de forage doivent être imprimés. Imprime les boutons d'expansion/réduction lorsqu'ils sont affichés sur le tableau croisé dynamique. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles/) { get; set; } | Indique si les titres d'impression de la feuille de calcul sont définis en fonction du rapport du PivotTable. La valeur par défaut est false. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile/) { get; set; } | Indique s'il faut actualiser les données lors de l'ouverture du fichier. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate/) { get; } | Obtient la dernière date et heure à laquelle le PivotTable a été actualisé. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho/) { get; } | Obtient le nom du dernier utilisateur qui a actualisé ce PivotTable |
| [RepeatItemsOnEachPrintedPage](../../aspose.cells.pivot/pivottable/repeatitemsoneachprintedpage/) { get; set; } | Indique si les légendes des éléments de tableau croisé dynamique dans la zone de lignes sont répétées sur chaque page imprimée pour les champs de tableau croisé dynamique sous forme tabulaire. |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields/) { get; } | Renvoie une [`PivotFieldCollection`](../pivotfieldcollection/) qui sont actuellement affichées comme champs de lignes. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand/) { get; set; } | (**Obsolète.**) Indique s'il faut afficher les totaux généraux pour les lignes de ce tableau croisé dynamique. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption/) { get; set; } | Obtient et définit la légende personnalisée de l'en-tête de ligne dans ce PivotTable. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange/) { get; } | Renvoie un objet CellArea qui représente la plage contenant la zone de lignes dans le rapport du PivotTable. Lecture seule. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata/) { get; set; } | Indique si les données du rapport du PivotTable sont enregistrées avec le classeur. |
| [ShowColumnGrandTotals](../../aspose.cells.pivot/pivottable/showcolumngrandtotals/) { get; set; } | Indique s'il faut afficher les totaux généraux pour les colonnes de ce tableau croisé dynamique. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips/) { get; set; } | Indique si les infobulles doivent être affichées pour les cellules de données du PivotTable. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill/) { get; set; } | Obtient et définit l'affichage des boutons d'expansion/réduction. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol/) { get; set; } | Indique s'il faut inclure des colonnes vides dans le tableau |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow/) { get; set; } | Indique s'il faut inclure des lignes vides dans le tableau. |
| [ShowHeaders](../../aspose.cells.pivot/pivottable/showheaders/) { get; set; } | Indique s'il faut afficher les légendes des champs de données et les légendes des champs de tableau croisé dynamique sur l'axe des lignes et l'axe des colonnes dans la vue du PivotTable. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips/) { get; set; } | Spécifie une valeur booléenne indiquant si les informations de propriété des membres doivent être omises des infobulles du PivotTable. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader/) { get; set; } | Indique si l'en-tête de colonne du tableau croisé dynamique doit avoir le style appliqué. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes/) { get; set; } | Indique si le formatage en bandes est appliqué pour la colonne. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn/) { get; set; } | Indique si le formatage de la colonne est appliqué. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader/) { get; set; } | Indique si l'en-tête de ligne du tableau croisé dynamique doit avoir le style appliqué. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes/) { get; set; } | Indique si le formatage en bandes de ligne est appliqué. |
| [ShowRowGrandTotals](../../aspose.cells.pivot/pivottable/showrowgrandtotals/) { get; set; } | Indique s'il faut afficher les totaux généraux pour les lignes du tableau croisé dynamique. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption/) { get; set; } | (**Obsolete.**) Indique si la légende de l'en-tête de ligne est affichée dans le rapport PivotTable indique si les légendes des champs d'affichage et les listes déroulantes de filtre sont affichées. |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow/) { get; set; } | Indique si la ligne des valeurs est affichée. |
| [SourceType](../../aspose.cells.pivot/pivottable/sourcetype/) { get; } | Obtient le type de source de données du tableau croisé dynamique. |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems/) { get; set; } | Indique si les éléments de champ de page masqués dans le rapport PivotTable sont inclus dans les sous‑totaux de lignes et de colonnes, les totaux de blocs et les totaux généraux. La valeur par défaut est False. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1/) { get; } | Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport PivotTable, mais n'inclut pas les champs de page. Lecture seule. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2/) { get; } | Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport PivotTable, incluant les champs de page. Lecture seule. |
| [Tag](../../aspose.cells.pivot/pivottable/tag/) { get; set; } | Obtient et définit une chaîne définie par l'utilisateur associée à cette vue PivotTable. |
| [TopRightArea](../../aspose.cells.pivot/pivottable/toprightarea/) { get; } | Représente la zone vide en haut à droite du PivotTable (en haut à gauche pour les feuilles RTL). |
| [ValuesField](../../aspose.cells.pivot/pivottable/valuesfield/) { get; } | Obtient un objet [`PivotField`](../pivotfield/) qui représente tous les champs de données d'un PivotTable. Lecture seule. Il ne serait créé que lorsqu'il y a deux champs de données ou plus dans la région Data. Par défaut, il se trouve dans la région des lignes. Vous pouvez le faire glisser vers la région ligne/colonne avec la méthode PivotTable.AddFieldToArea(). |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield)(string, string) | Ajoute un champ calculé au champ pivot et le fait glisser vers la zone de données. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield_1)(string, string, bool) | Ajoute un champ calculé au champ pivot. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_1)(PivotFieldType, int) | Ajoute le champ à la zone spécifique. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea)(PivotFieldType, PivotField) | Ajoute le champ à la zone spécifique. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_2)(PivotFieldType, string) | Ajoute le champ à la zone spécifique. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata_1)() | Calcule les données du pivottable dans les cellules. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata)(PivotTableCalculateOption) | Calcule le tableau croisé dynamique avec des options. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange/)() | Calcule la plage du pivottable. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource/)(string[]) | Modifie la source de données du tableau croisé dynamique. |
| [ClearAll](../../aspose.cells.pivot/pivottable/clearall/)() | Supprime tous les champs des régions. |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata/)() | Efface les données et le formatage de la vue PivotTable. |
| [ClearFilters](../../aspose.cells.pivot/pivottable/clearfilters/)() | Efface tous les filtres de ce tableau croisé dynamique. |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle/)(PivotTable) | Copie le style nommé d'un autre tableau croisé dynamique. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose/)() | Effectue des tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [ExportViewToJson](../../aspose.cells.pivot/pivottable/exportviewtojson/)(PivotViewToJsonOptions) | Exporte la vue pivot en JSON. |
| [Fields](../../aspose.cells.pivot/pivottable/fields/)(PivotFieldType) | (**Obsolete.**) Obtient les champs spécifiques par le type de champ. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format)(CellArea, Style) | Formate la zone sélectionnée du tableau croisé dynamique. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_1)(PivotArea, Style) | Formate la zone sélectionnée du tableau croisé dynamique. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_2)(int, int, Style) | Formate la cellule dans la zone du tableau croisé dynamique |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall/)(Style) | Formate toutes les cellules dans la zone du tableau croisé dynamique |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow/)(int, Style) | Formate les données de ligne dans la zone du tableau croisé dynamique |
| [GetButtonArea](../../aspose.cells.pivot/pivottable/getbuttonarea/)(PivotFieldType) | Obtient la zone contenant le bouton de champ. |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname/)(string) | Obtient l'objet [`Cell`](../../aspose.cells/cell/) par le nom d'affichage du PivotField. |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren/)() | (**Obsolete.**) Obtient les tableaux croisés dynamiques enfants qui utilisent ces données de tableau croisé dynamique comme source de données. |
| [GetDependentPivotTables](../../aspose.cells.pivot/pivottable/getdependentpivottables/)() | Obtient tous les `PivotTable`s qui utilisent ce tableau croisé dynamique comme source de données. |
| [GetFields](../../aspose.cells.pivot/pivottable/getfields/)(PivotFieldType) | Obtient la liste spécifique des champs pivot par région. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks/)() | (**Obsolete.**) Obtient la liste des index de lignes du tableau croisé dynamique des sauts de page horizontaux |
| [GetHorizontalPageBreaks](../../aspose.cells.pivot/pivottable/gethorizontalpagebreaks/)() | Obtient les sauts de page horizontaux de ce tableau croisé dynamique. |
| [GetNamesOfSourceDataConnections](../../aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/)() | Obtient les noms des connexions de données source externes. |
| [GetPivotTablesWithSamePivotCache](../../aspose.cells.pivot/pivottable/getpivottableswithsamepivotcache/)() | Obtient tous les tableaux croisés dynamiques avec le même cache pivot. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource)() | Obtient la source de données de ce tableau croisé dynamique. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource_1)(bool) | Obtient la source de données de ce tableau croisé dynamique. |
| [GetSourceDataConnections](../../aspose.cells.pivot/pivottable/getsourcedataconnections/)() | Obtient les sources de données de connexion externes. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move_1)(string) | (**Obsolete.**) Déplace le tableau croisé dynamique vers un autre emplacement dans la feuille de calcul. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move)(int, int) | (**Obsolete.**) Déplace le tableau croisé dynamique vers un autre emplacement dans la feuille de calcul. |
| [MoveItem](../../aspose.cells.pivot/pivottable/moveitem/)(PivotFieldType, string[], bool, int) | Déplace un élément vers le haut ou vers le bas. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_2)(string) | Déplace le tableau croisé dynamique vers un autre emplacement dans la feuille de calcul. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto)(int, int) | Déplace le tableau croisé dynamique vers un autre emplacement dans la feuille de calcul. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_1)(int, int, int) | Déplace le tableau croisé dynamique vers un autre emplacement dans la feuille de calcul. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh)() | Actualise le [`PivotCache`](./pivotcache/) depuis la source de données et calcule les données et le style pour la vue pivot. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh_1)(PivotTableRefreshOption) | Actualise le [`PivotCache`](./pivotcache/) depuis la source de données et calcule les données et le style pour la vue pivot. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata)() | (**Obsolete.**) Actualise les données depuis sa source de données vers le cache pivot. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata_1)(PivotTableRefreshOption) | (**Obsolete.**) Actualise les données et les paramètres du tableau croisé dynamique depuis sa source de données avec des options. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_1)(PivotFieldType, int) | Supprime un champ d'une région pivot spécifique. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield)(PivotFieldType, PivotField) | Supprime le champ d'une zone de champ spécifique |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_2)(PivotFieldType, string) | Supprime un champ d'une zone de champ spécifique |
| [SelectArea](../../aspose.cells.pivot/pivottable/selectarea/)(CellArea) | Sélectionnez une zone de la vue du tableau croisé dynamique. |
| [ShowDetail](../../aspose.cells.pivot/pivottable/showdetail/)(int, int, bool, int, int) | Affiche le détail d'un élément dans la région de données dans un nouveau tableau. |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform/)() | Mise en page de la vue du tableau croisé dynamique sous forme compacte. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform/)() | Mise en page du tableau croisé dynamique sous forme de plan. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform/)() | Mise en page du tableau croisé dynamique sous forme tabulaire. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage/)(PivotField) | Affiche toutes les pages de filtre de rapport selon le champ PivotField, le champ PivotField doit être situé dans les champs de page. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex/)(int) | Affiche toutes les pages de filtre de rapport selon l'index de position dans les champs de page. |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname/)(string) | Affiche toutes les pages de filtre de rapport selon le nom du champ PivotField, le champ PivotField doit être situé dans les champs de page. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotTableDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Définir des données d'exemple
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";

            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;

            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];

            // Ajouter des champs
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Styliser le tableau croisé dynamique
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Personnaliser le champ de ligne
            PivotField rowField = pivot.RowFields[0];
            rowField.DisplayName = "Fruit Category";

            // Actualiser et calculer les données
            pivot.RefreshData();
            pivot.CalculateData();

            // Enregistrez le classeur
            book.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


