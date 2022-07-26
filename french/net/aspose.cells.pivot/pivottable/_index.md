---
title: PivotTable
second_title: Référence de l'API Aspose.Cells pour .NET
description: Description sommaire du tableau croisé dynamique.
type: docs
weight: 4690
url: /fr/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

Description sommaire du tableau croisé dynamique.

```csharp
public class PivotTable : IDisposable
```

## Propriétés

| Nom | La description |
| --- | --- |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription) { get; set; } | Obtient la description du texte alternatif |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle) { get; set; } | Obtient le titre de l'altertext |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype) { get; set; } | Obtient le type de format automatique du tableau croisé dynamique. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields) { get; } | Renvoie un objet PivotFields qui inclut tous les champs du rapport de tableau croisé dynamique |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields) { get; } | Renvoie un objet PivotFields actuellement affiché sous forme de champs de colonne. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand) { get; set; } | Indique si le rapport de tableau croisé dynamique affiche les totaux généraux pour les colonnes. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption) { get; set; } | Obtient la légende de l'en-tête de colonne du tableau croisé dynamique. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange) { get; } | Renvoie un objet CellArea qui représente la plage qui contient la zone de colonne dans le rapport de tableau croisé dynamique. Lecture seule. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort) { get; set; } | Indique si la liste personnalisée intégrée doit être prise en compte lors du tri des données |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange) { get; } | Renvoie un objet CellArea qui représente la plage contenant la zone de données dans la liste entre la ligne d'en-tête et la ligne d'insertion. Lecture seule. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield) { get; } | Obtient un objet PivotField qui représente tous les champs de données d'un tableau croisé dynamique. En lecture seule. Il ne serait init que lorsqu'il y a deux champs de données ou plus dans les DataPiovtFiels. Il sert uniquement à ajouter DataPivotField à la ligne/colonne du tableau croisé dynamique Région . La valeur par défaut est dans la zone de ligne. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields) { get; } | Obtient un objet PivotField qui représente tous les champs de données d'un tableau croisé dynamique. En lecture seule. Il ne serait init que lorsqu'il y a deux champs de données ou plus dans les DataPiovtFiels. Il sert uniquement à ajouter DataPivotField à la ligne/colonne du tableau croisé dynamique Région . La valeur par défaut est dans la zone de ligne. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource) { get; set; } | Obtient et définit la source de données du tableau croisé dynamique. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring) { get; set; } | Indique si le rapport de tableau croisé dynamique affiche une chaîne personnalisée dans les cellules contenant des erreurs. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems) { get; set; } | Indique si les éléments des zones de ligne et de colonne sont visibles lorsque la zone de données du tableau croisé dynamique est vide. La valeur par défaut est true. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring) { get; set; } | Indique si le rapport de tableau croisé dynamique affiche une chaîne personnalisée dans les cellules contenant des valeurs nulles. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting) { get; set; } | Spécifie une valeur booléenne qui indique si l'utilisateur est autorisé à modifier les cellules dans la zone de données du tableau croisé dynamique. Activer la modification des cellules dans la zone de valeurs |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown) { get; set; } | Obtient si l'exploration est activée. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog) { get; set; } | Indique si la boîte de dialogue Champ de tableau croisé dynamique est disponible lorsque l'utilisateur double-clique sur le champ de tableau croisé dynamique. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist) { get; set; } | Obtient si activer la liste des champs pour le tableau croisé dynamique. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard) { get; set; } | Indique si l'assistant de tableau croisé dynamique est disponible. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring) { get; set; } | Obtient la chaîne affichée dans les cellules contenant des erreurs lorsque la propriété DisplayErrorString est vraie. La valeur par défaut est une chaîne vide. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource) { get; } | Obtient la source de données de connexion externe. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending) { get; set; } | Spécifie une valeur booléenne qui indique si les champs du tableau croisé dynamique sont triés dans un ordre autre que celui par défaut dans la liste des champs. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname) { get; set; } | Renvoie l'étiquette de la chaîne de texte qui s'affiche dans l'en-tête de colonne ou de ligne du total général. La valeur par défaut est la chaîne « Total général ». |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows) { get; set; } | Indique s'il faut ajouter des lignes vides. Cette propriété s'applique uniquement aux types de format automatique de tableau croisé dynamique qui doivent ajouter des lignes vides. |
| [Indent](../../aspose.cells.pivot/pivottable/indent) { get; set; } | Spécifie l'incrément d'indentation pour l'axe compact et peut être utilisé pour définir la mise en page du rapport sur forme compacte. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat) { get; set; } | Indique si le rapport de tableau croisé dynamique est formaté automatiquement. Case à cocher "tableau de mise en forme automatique" qui est dans l'option de tableau croisé dynamique pour Excel 2003 Case à cocher "largeur de colonne d'ajustement automatique lors de la mise à jour" qui est dans le tableau croisé dynamique Options :Format de mise en page pour Excel 2007 |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible) { get; set; } | Spécifie si le tableau croisé dynamique est compatible avec Excel2003 lors de l'actualisation du tableau croisé dynamique, si vrai, une chaîne doit être inférieure ou égale à 255 caractères, donc si la chaîne est supérieure à 255 caractères, elle sera tronquée. si false, une chaîne n'aura pas la restriction susmentionnée. La valeur par défaut est true. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones) { get; set; } | Indique si le rapport de tableau croisé dynamique affiche une disposition de tableau croisé dynamique classique. (permet de faire glisser des champs dans la grille) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters) { get; set; } | Spécifie une valeur booléenne qui indique si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres définis sur eux. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected) { get; set; } | Indique si le tableau croisé dynamique est sélectionné. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles) { get; set; } | Un bit qui spécifie si les légendes des éléments de pivot sur l'axe de ligne sont répétées sur chaque page imprimée pour les champs de pivot sous forme de tableau. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate) { get; set; } | Indique si le rapport de tableau croisé dynamique est recalculé uniquement à la demande de l'utilisateur. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels) { get; set; } | Indique si l'élément de ligne externe, l'élément de colonne, le sous-total, et les étiquettes de total général du rapport de tableau croisé dynamique spécifié utilisent des cellules fusionnées. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit) { get; set; } | Spécifie une valeur booléenne qui indique si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres définis sur eux. |
| [Name](../../aspose.cells.pivot/pivottable/name) { get; set; } | Obtient le nom du tableau croisé dynamique |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring) { get; set; } | Obtient la chaîne affichée dans les cellules qui contiennent des valeurs nulles lorsque la propriété DisplayNullString est vraie. La valeur par défaut est une chaîne vide. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder) { get; set; } | Obtient l'ordre dans lequel les champs de page sont ajoutés à la disposition du rapport de tableau croisé dynamique. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields) { get; } | Renvoie un objet PivotFields actuellement affiché sous forme de champs de page. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount) { get; set; } | Obtient le nombre de champs de page dans chaque colonne ou ligne du rapport de tableau croisé dynamique. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters) { get; } | Renvoie un objet PivotFilterCollection. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions) { get; } | Obtient les conditions de format du tableau croisé dynamique. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename) { get; set; } | Obtient et définit le nom du style de tableau croisé dynamique. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype) { get; set; } | Obtient et définit le style de tableau croisé dynamique intégré. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting) { get; set; } | Indique si la mise en forme est conservée lorsque le tableau croisé dynamique est actualisé ou recalculé. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill) { get; set; } | Spécifie une valeur booléenne qui indique si les indicateurs d'exploration doivent être imprimés. imprimer les boutons de développement/réduction lorsqu'ils sont affichés sur le tableau croisé dynamique. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles) { get; set; } | Indique si les titres d'impression de la feuille de calcul sont définis en fonction de sur le rapport de tableau croisé dynamique. La valeur par défaut est false. |
| [RefreshDataFlag](../../aspose.cells.pivot/pivottable/refreshdataflag) { get; set; } | Indique si Actualiser les données ou non. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile) { get; set; } | Indique si Actualiser les données lors de l'ouverture du fichier. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate) { get; } | Obtient la date à laquelle le tableau croisé dynamique a été actualisé pour la dernière fois. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho) { get; } | Obtient le nom de l'utilisateur qui a actualisé le tableau croisé dynamique pour la dernière fois |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields) { get; } | Renvoie un objet PivotFields actuellement affiché sous forme de champs de ligne. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand) { get; set; } | Indique si le rapport de tableau croisé dynamique affiche les totaux généraux pour les lignes. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption) { get; set; } | Obtient la légende d'en-tête de ligne du tableau croisé dynamique. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange) { get; } | Renvoie un objet CellArea qui représente la plage qui contient la zone de ligne dans le rapport de tableau croisé dynamique. Lecture seule. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata) { get; set; } | Indique si les données du rapport de tableau croisé dynamique sont enregistrées avec le classeur. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips) { get; set; } | Spécifie une valeur booléenne qui indique si les info-bulles doivent être affichées pour les cellules de données de tableau croisé dynamique. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill) { get; set; } | Obtient si les boutons développer/réduire sont affichés. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol) { get; set; } | Spécifie une valeur booléenne qui indique s'il faut inclure des colonnes vides dans la table |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow) { get; set; } | Spécifie une valeur booléenne qui indique s'il faut inclure des lignes vides dans la table. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips) { get; set; } | Spécifie une valeur booléenne qui indique si les informations de propriété de membre doivent être omises des info-bulles de tableau croisé dynamique. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader) { get; set; } | Indique si l'en-tête de colonne dans le tableau croisé dynamique doit avoir le style appliqué. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes) { get; set; } | Indique si le format de bande de colonne est appliqué. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn) { get; set; } | Indique si le format de bande de colonne est appliqué. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader) { get; set; } | Indique si l'en-tête de ligne dans le tableau croisé dynamique doit avoir le style appliqué. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes) { get; set; } | Indique si la mise en forme des bandes de lignes est appliquée. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption) { get; set; } | Indique si la légende de l'en-tête de ligne est affichée dans le rapport de tableau croisé dynamique Indique si Afficher les légendes des champs et les listes déroulantes des filtres |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow) { get; set; } | Spécifie une valeur booléenne qui indique si afficher les valeurs row. afficher les valeurs row |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems) { get; set; } | Indique si les éléments de champ de page masqués dans le rapport de tableau croisé dynamique sont inclus dans les sous-totaux de ligne et de colonne, les totaux de bloc et les totaux généraux. La valeur par défaut est False. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1) { get; } | Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport de tableau croisé dynamique, mais n'inclut pas les champs de page. Lecture seule. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2) { get; } | Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport de tableau croisé dynamique, inclut les champs de page. Lecture seule. |
| [Tag](../../aspose.cells.pivot/pivottable/tag) { get; set; } | Obtient une chaîne enregistrée avec le rapport de tableau croisé dynamique. |

## Méthodes

| Nom | La description |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield)(string, string) | Ajoute un champ calculé au champ pivot et le fait glisser vers la zone de données. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield_1)(string, string, bool) | Ajoute un champ calculé au champ pivot. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_1)(PivotFieldType, int) | Ajoute le champ à la zone spécifique. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea)(PivotFieldType, PivotField) | Ajoute le champ à la zone spécifique. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_2)(PivotFieldType, string) | Ajoute le champ à la zone spécifique. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata)() | Calcule les données du tableau croisé dynamique en cellules. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange)() | Calcule la plage du tableau croisé dynamique. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource)(string[]) | Définir les données source du tableau croisé dynamique. Sheet1 !$A$1 :$C$3 |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata)() | Effacer les données et la mise en forme du tableau croisé dynamique |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle)(PivotTable) | Copie le style nommé d'un autre tableau croisé dynamique. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose)() | Effectue des tâches définies par l'application associées à la libération, à la libération ou à la réinitialisation des ressources non gérées. |
| [Fields](../../aspose.cells.pivot/pivottable/fields)(PivotFieldType) | Obtient les champs spécifiques par le type de champ. |
| [Format](../../aspose.cells.pivot/pivottable/format)(int, int, Style) | Formater la cellule dans la zone de tableau croisé dynamique |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall)(Style) | Formater toutes les cellules de la zone de tableau croisé dynamique |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow)(int, Style) | Formater les données de ligne dans la zone de tableau croisé dynamique |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname)(string) | Obtient l'objet Cell par le DisplayName de PivotField |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren)() | Obtient les tableaux croisés dynamiques enfants qui utilisent ces données de tableau croisé dynamique comme source de données. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks)() | obtenir la liste d'index des lignes du tableau croisé dynamique des sauts de page horizontaux |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource)() | Obtenir les données source du tableau croisé dynamique. |
| [Move](../../aspose.cells.pivot/pivottable/move#move_1)(string) | Déplace le tableau croisé dynamique vers un autre emplacement dans la feuille de calcul. |
| [Move](../../aspose.cells.pivot/pivottable/move#move)(int, int) | Déplace le tableau croisé dynamique vers un autre emplacement dans la feuille de calcul. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata)() | Actualise les données et les paramètres du tableau croisé dynamique à partir de sa source de données. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_1)(PivotFieldType, int) | Supprime un champ d'une zone de champ spécifique |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield)(PivotFieldType, PivotField) | Supprimer le champ d'une zone de champ spécifique |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_2)(PivotFieldType, string) | Supprime un champ d'une zone de champ spécifique |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield_1)(int) | Définit le groupe de champs automatique par le tableau croisé dynamique. |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield)(PivotField) | Définit le groupe de champs automatique par le tableau croisé dynamique. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_3)(int, DateTime, DateTime, ArrayList, int) | Définit le groupe de champs manuels par le tableau croisé dynamique. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_2)(int, double, double, ArrayList, double) | Définit le groupe de champs manuels par le tableau croisé dynamique. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_1)(PivotField, DateTime, DateTime, ArrayList, int) | Définit le groupe de champs manuels par le tableau croisé dynamique. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield)(PivotField, double, double, ArrayList, double) | Définit le groupe de champs manuels par le tableau croisé dynamique. |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup_1)(int) | Ensembles dégroupés par le tableau croisé dynamique |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup)(PivotField) | Ensembles dégroupés par le tableau croisé dynamique |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform)() | Présente le tableau croisé dynamique sous forme compacte. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform)() | Présente le tableau croisé dynamique sous forme de plan. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform)() | Présente le tableau croisé dynamique sous forme de tableau. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage)(PivotField) | Afficher toutes les pages de filtre de rapport selon PivotField, le PivotField doit être situé dans PageFields. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex)(int) | Afficher toutes les pages de filtre de rapport en fonction de l'index de position dans PageFields |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname)(string) | Afficher toutes les pages de filtre de rapport en fonction du nom de PivotField, le PivotField doit être situé dans PageFields. |

### Exemples

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Modifier les attributs de PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

//Ajouter un filtre croisé dynamique
int index = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[index];
filter.AutoFilter.FilterTop10(0, false, false, 2);

//Ajouter une condition de format de pivot
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

pivot.RefreshData();
pivot.CalculateData();

//faites vos affaires

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'Ajouter un filtre croisé dynamique
Dim filterIndex As Int32 = pivot.PivotFilters.Add(0, PivotFilterType.Count)
Dim filter As PivotFilter = pivot.PivotFilters(filterIndex)
filter.AutoFilter.FilterTop10(0, False, False, 2)

'Ajouter une condition de format Pivot
Dim formatIndex As Int32 = pivot.PivotFormatConditions.Add()
Dim pfc As PivotFormatCondition = pivot.PivotFormatConditions(formatIndex)
Dim fcc As FormatConditionCollection = pfc.FormatConditions
fcc.AddArea(pivot.DataBodyRange)
Dim idx As Int32 = fcc.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = fcc(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Voir également

* espace de noms [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
