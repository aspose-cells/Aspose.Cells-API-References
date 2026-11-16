---
title: "Classe Worksheet"
linktitle: "Worksheet"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Worksheet. Encapsule l'objet qui représente une feuille de calcul dans Go."
type: docs
weight: 200
url: /fr/go-cpp/worksheet/
---

## Worksheet class

Encapsule l'objet qui représente une seule feuille de calcul.

```go

type Worksheet struct  {
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
| [GetProtection](./getprotection/) | Représente les différents types d'options de protection disponibles pour une feuille de calcul. Prend en charge les options de protection avancées dans ExcelXP et les versions ultérieures. |
| [GetUniqueId](./getuniqueid/) | Obtient et définit l'identifiant unique, il est identique à {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [SetUniqueId](./setuniqueid/) | Obtient et définit l'identifiant unique, il est identique à {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [GetPanes](./getpanes/) | Obtient les volets de la fenêtre. |
| [GetWorkbook](./getworkbook/) | Obtient l'objet classeur qui contient cette feuille. |
| [GetCells](./getcells/) | Obtient la collection Aspose.Cells.Cells. |
| [GetQueryTables](./getquerytables/) | Obtient QueryTableCollection dans la feuille de calcul. |
| [GetType](./gettype/) | Représente le type de feuille de calcul. |
| [SetType](./settype/) | Représente le type de feuille de calcul. |
| [GetName](./getname/) | Obtient ou définit le nom de la feuille de calcul. |
| [SetName](./setname/) | Obtient ou définit le nom de la feuille de calcul. |
| [GetShowFormulas](./getshowformulas/) | Indique s'il faut afficher les formules ou leurs résultats. |
| [SetShowFormulas](./setshowformulas/) | Indique s'il faut afficher les formules ou leurs résultats. |
| [GetShowDataTypeIcons](./getshowdatatypeicons/) | Indique s'il faut afficher les icônes de type de données. |
| [SetShowDataTypeIcons](./setshowdatatypeicons/) | Indique s'il faut afficher les icônes de type de données. |
| [IsGridlinesVisible](./isgridlinesvisible/) | Obtient ou définit une valeur indiquant si les quadrillages sont visibles. La valeur par défaut est vraie. |
| [SetIsGridlinesVisible](./setisgridlinesvisible/) | Obtient ou définit une valeur indiquant si les quadrillages sont visibles. La valeur par défaut est vraie. |
| [IsRowColumnHeadersVisible](./isrowcolumnheadersvisible/) | Obtient ou définit une valeur indiquant si la feuille de calcul affichera les en-têtes de lignes et de colonnes. La valeur par défaut est vraie. |
| [SetIsRowColumnHeadersVisible](./setisrowcolumnheadersvisible/) | Obtient ou définit une valeur indiquant si la feuille de calcul affichera les en-têtes de lignes et de colonnes. La valeur par défaut est vraie. |
| [GetPaneState](./getpanestate/) | Indique si le volet possède des divisions horizontales ou verticales, et si ces divisions sont figées. |
| [GetDisplayZeros](./getdisplayzeros/) | Vrai si les valeurs zéro sont affichées. |
| [SetDisplayZeros](./setdisplayzeros/) | Vrai si les valeurs zéro sont affichées. |
| [GetDisplayRightToLeft](./getdisplayrighttoleft/) | Indique si la feuille de calcul spécifiée est affichée de droite à gauche au lieu de gauche à droite. La valeur par défaut est fausse. |
| [SetDisplayRightToLeft](./setdisplayrighttoleft/) | Indique si la feuille de calcul spécifiée est affichée de droite à gauche au lieu de gauche à droite. La valeur par défaut est fausse. |
| [IsOutlineShown](./isoutlineshown/) | Indique s'il faut afficher le plan. |
| [SetIsOutlineShown](./setisoutlineshown/) | Indique s'il faut afficher le plan. |
| [IsSelected](./isselected/) | Indique si cette feuille de calcul est sélectionnée lors de l'ouverture du classeur. |
| [SetIsSelected](./setisselected/) | Indique si cette feuille de calcul est sélectionnée lors de l'ouverture du classeur. |
| [FreezePanes_Int_Int_Int_Int](./freezepanes_int_int_int_int/) | Fige les volets à la cellule spécifiée dans la feuille de calcul. |
| [GetFreezedPanes](./getfreezedpanes/) | Obtient les volets figés. |
| [Split](./split/) | Divise la fenêtre. |
| [FreezePanes_String_Int_Int](./freezepanes_string_int_int/) | Fige les volets à la cellule spécifiée dans la feuille de calcul. |
| [UnFreezePanes](./unfreezepanes/) | Dégèle les volets dans la feuille de calcul. |
| [RemoveSplit](./removesplit/) | Supprime la division de la fenêtre. |
| [GetPivotTables](./getpivottables/) | Obtient tous les tableaux croisés dynamiques dans cette feuille de calcul. |
| [GetListObjects](./getlistobjects/) | Obtient tous les ListObjects dans cette feuille de calcul. |
| [GetTabId](./gettabid/) | Spécifie l'identifiant interne de la feuille. |
| [SetTabId](./settabid/) | Spécifie l'identifiant interne de la feuille. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Obtient la collection HorizontalPageBreakCollection. |
| [GetVerticalPageBreaks](./getverticalpagebreaks/) | Obtient la collection VerticalPageBreakCollection. |
| [AddPageBreaks](./addpagebreaks/) | Ajoute un saut de page. |
| [GetHyperlinks](./gethyperlinks/) | Obtient la collection HyperlinkCollection. |
| [Copy_Worksheet](./copy_worksheet/) | Copie le contenu et les formats d'une autre feuille de calcul. |
| [Copy_Worksheet_CopyOptions](./copy_worksheet_copyoptions/) | Copie le contenu et les formats d'une autre feuille de calcul. |
| [AutoFitColumn_Int_Int_Int](./autofitcolumn_int_int_int/) | Ajuste automatiquement la largeur de la colonne. |
| [AutoFitColumns](./autofitcolumns/) | Ajuste automatiquement toutes les colonnes de cette feuille de calcul. |
| [AutoFitColumns_AutoFitterOptions](./autofitcolumns_autofitteroptions/) | Ajuste automatiquement toutes les colonnes de cette feuille de calcul. |
| [AutoFitColumn_Int](./autofitcolumn_int/) | Ajuste automatiquement la largeur de la colonne. |
| [AutoFitColumns_Int_Int](./autofitcolumns_int_int/) | Ajuste automatiquement la largeur des colonnes. |
| [AutoFitColumns_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_autofitteroptions/) | Ajuste automatiquement la largeur des colonnes. |
| [AutoFitColumns_Int_Int_Int_Int](./autofitcolumns_int_int_int_int/) | Ajuste automatiquement la largeur des colonnes. |
| [AutoFitColumns_Int_Int_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_int_int_autofitteroptions/) | Ajuste automatiquement la largeur des colonnes. |
| [AutoFitRow_Int_Int_Int](./autofitrow_int_int_int/) | Ajuste automatiquement la hauteur de la ligne. |
| [AutoFitRow_Int_Int_Int_AutoFitterOptions](./autofitrow_int_int_int_autofitteroptions/) | Ajuste automatiquement la hauteur de la ligne. |
| [AutoFitRows](./autofitrows/) | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [AutoFitRows_Bool](./autofitrows_bool/) | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [AutoFitRows_AutoFitterOptions](./autofitrows_autofitteroptions/) | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [AutoFitRows_Int_Int](./autofitrows_int_int/) | Ajuste automatiquement la hauteur des lignes dans une plage. |
| [AutoFitRows_Int_Int_AutoFitterOptions](./autofitrows_int_int_autofitteroptions/) | Ajuste automatiquement la hauteur des lignes dans une plage. |
| [AutoFitRow_Int_Int_Int_Int](./autofitrow_int_int_int_int/) | Ajuste automatiquement la hauteur des lignes dans une plage rectangulaire. |
| [AutoFitRow_Int](./autofitrow_int/) | Ajuste automatiquement la hauteur de la ligne. |
| [GetPageSetup](./getpagesetup/) | Représente la description de la mise en page de cette feuille. |
| [GetAutoFilter](./getautofilter/) | Représente le filtre automatique pour la feuille de calcul spécifiée. |
| [Filter](./filter/) | Filtre la plage. |
| [GetAdvancedFilter](./getadvancedfilter/) | Obtient les paramètres du filtre avancé. |
| [Advanced_Filter](./advanced_filter/) | Filtre les données en utilisant des critères complexes. |
| [RemoveAutoFilter](./removeautofilter/) | Supprime le filtre automatique de la feuille de calcul. |
| [GetHasAutofilter](./gethasautofilter/) | Indique si cette feuille de calcul possède un filtre automatique. |
| [GetTransitionEvaluation](./gettransitionevaluation/) | Indique si l'option d'évaluation de formule de transition (compatibilité Lotus) est activée. |
| [SetTransitionEvaluation](./settransitionevaluation/) | Indique si l'option d'évaluation de formule de transition (compatibilité Lotus) est activée. |
| [GetTransitionEntry](./gettransitionentry/) | Indique si l'option d'entrée de formule de transition (compatibilité Lotus) est activée. |
| [SetTransitionEntry](./settransitionentry/) | Indique si l'option d'entrée de formule de transition (compatibilité Lotus) est activée. |
| [GetVisibilityType](./getvisibilitytype/) | Indique l'état de visibilité de cette feuille. |
| [SetVisibilityType](./setvisibilitytype/) | Indique l'état de visibilité de cette feuille. |
| [SetVisible](./setvisible/) | Définit les options de visibilité. |
| [IsVisible](./isvisible/) | Représente si la feuille de calcul est visible. |
| [SetIsVisible](./setisvisible/) | Représente si la feuille de calcul est visible. |
| [SelectRange](./selectrange/) | Sélectionne une plage. |
| [RemoveAllDrawingObjects](./removealldrawingobjects/) | Supprime tous les objets de dessin dans cette feuille de calcul. |
| [ClearComments](./clearcomments/) | Efface tous les commentaires dans la feuille de calcul du concepteur. |
| [GetSparklineGroups](./getsparklinegroups/) | Obtient les groupes de sparkline dans la feuille de calcul. |
| [GetCharts](./getcharts/) | Obtient une collection de graphiques |
| [GetComments](./getcomments/) | Obtient la collection de commentaires. |
| [GetPictures](./getpictures/) | Obtient une collection d'images. |
| [GetAllPictures](./getallpictures/) | Obtient toutes les images, y compris les images incorporées dans la cellule et au-dessus des cellules. |
| [GetTextBoxes](./gettextboxes/) | Obtient une collection de zones de texte. |
| [GetCheckBoxes](./getcheckboxes/) | Obtient une collection de cases à cocher. |
| [GetOleObjects](./getoleobjects/) | Représente une collection d'OleObject dans une feuille de calcul. |
| [GetShapes](./getshapes/) | Renvoie toutes les formes de dessin dans cette feuille de calcul. |
| [GetSlicers](./getslicers/) | Obtenez la collection de Slicer dans la feuille de calcul |
| [GetTimelines](./gettimelines/) | Obtenez la collection de Timeline dans la feuille de calcul |
| [Protect_ProtectionType](./protect_protectiontype/) | Protège la feuille de calcul. |
| [Protect_ProtectionType_String_String](./protect_protectiontype_string_string/) | Protège la feuille de calcul. |
| [Unprotect](./unprotect/) | Supprime la protection de la feuille de calcul. |
| [Unprotect_String](./unprotect_string/) | Supprime la protection de la feuille de calcul. |
| [GetIndex](./getindex/) | Obtient l'index de la feuille dans la collection de feuilles de calcul. |
| [MoveTo](./moveto/) | Déplace la feuille vers un autre emplacement dans le classeur. |
| [IsProtected](./isprotected/) | Indique si la feuille de calcul est protégée. |
| [GetValidations](./getvalidations/) | Obtient la collection des paramètres de validation des données dans la feuille de calcul. |
| [GetAllowEditRanges](./getalloweditranges/) | Obtient la collection des plages d'édition autorisées dans la feuille de calcul. |
| [GetErrorCheckOptions](./geterrorcheckoptions/) | Obtient les paramètres de vérification d'erreurs appliqués à certaines plages. |
| [GetOutline](./getoutline/) | Obtient le contour de cette feuille de calcul. |
| [GetFirstVisibleRow](./getfirstvisiblerow/) | Représente l'index de la première ligne visible. |
| [SetFirstVisibleRow](./setfirstvisiblerow/) | Représente l'index de la première ligne visible. |
| [GetFirstVisibleColumn](./getfirstvisiblecolumn/) | Représente l'index de la première colonne visible. |
| [SetFirstVisibleColumn](./setfirstvisiblecolumn/) | Représente l'index de la première colonne visible. |
| [Replace](./replace/) | Remplace le texte de toutes les cellules par une nouvelle chaîne. |
| [GetZoom](./getzoom/) | Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400. |
| [SetZoom](./setzoom/) | Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400. |
| [GetViewType](./getviewtype/) | Obtient et définit le type de vue. |
| [SetViewType](./setviewtype/) | Obtient et définit le type de vue. |
| [IsPageBreakPreview](./ispagebreakpreview/) | Indique si la feuille de calcul spécifiée est affichée en vue normale ou en aperçu des sauts de page. |
| [SetIsPageBreakPreview](./setispagebreakpreview/) | Indique si la feuille de calcul spécifiée est affichée en vue normale ou en aperçu des sauts de page. |
| [IsRulerVisible](./isrulervisible/) | Indique si la règle est visible. Cette propriété n'est appliquée que pour l'aperçu des sauts de page. |
| [SetIsRulerVisible](./setisrulervisible/) | Indique si la règle est visible. Cette propriété n'est appliquée que pour l'aperçu des sauts de page. |
| [GetSelectedAreas](./getselectedareas/) | Obtient les plages de cellules sélectionnées dans la feuille de calcul du concepteur. |
| [GetTabColor](./gettabcolor/) | Représente la couleur de l'onglet de la feuille de calcul. |
| [SetTabColor](./settabcolor/) | Représente la couleur de l'onglet de la feuille de calcul. |
| [GetGridlineColor](./getgridlinecolor/) | Obtient et définit la couleur de la grille |
| [SetGridlineColor](./setgridlinecolor/) | Obtient et définit la couleur de la grille |
| [GetCodeName](./getcodename/) | Obtient le nom de code de la feuille de calcul. |
| [SetCodeName](./setcodename/) | Obtient le nom de code de la feuille de calcul. |
| [GetBackgroundImage](./getbackgroundimage/) | Obtient et définit l'image d'arrière-plan de la feuille de calcul. |
| [SetBackgroundImage](./setbackgroundimage/) | Obtient et définit l'image d'arrière-plan de la feuille de calcul. |
| [GetConditionalFormattings](./getconditionalformattings/) | Obtient les ConditionalFormattings dans la feuille de calcul. |
| [GetActiveCell](./getactivecell/) | Obtient ou définit la cellule active dans la feuille de calcul. |
| [SetActiveCell](./setactivecell/) | Obtient ou définit la cellule active dans la feuille de calcul. |
| [GetCustomProperties](./getcustomproperties/) | Obtient un objet représentant les informations d'identifiant associées à une feuille de calcul. |
| [GetPrintingPageBreaks](./getprintingpagebreaks/) | Obtient les sauts de page automatiques. |
| [GetSmartTagSetting](./getsmarttagsetting/) | Obtient tous les objets SmartTagCollection de la feuille de calcul. |
| [ToString](./tostring/) | Renvoie une chaîne qui représente l'objet Worksheet actuel. |
| [GetScenarios](./getscenarios/) | Obtient la collection de Scenario. |
| [StartAccessCache](./startaccesscache/) | Démarre la session qui utilise des caches pour accéder aux données de cette feuille de calcul. |
| [CloseAccessCache](./closeaccesscache/) | Ferme la session qui utilise des caches pour accéder aux données de cette feuille de calcul. |
| [ConvertFormulaReferenceStyle](./convertformulareferencestyle/) | Convertit le style de référence de formule. |
| [CalculateFormula_String](./calculateformula_string/) | Calcule une formule. |
| [CalculateFormula_String_CalculationOptions](./calculateformula_string_calculationoptions/) | Calcule directement une expression de formule. |
| [CalculateFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_CalculationData](./calculateformula_string_formulaparseoptions_calculationoptions_int_int_calculationdata/) | Calcule directement une expression de formule. |
| [CalculateArrayFormula_String_CalculationOptions](./calculatearrayformula_string_calculationoptions/) | Calcule une formule en tant que formule matricielle. |
| [CalculateArrayFormula_String_CalculationOptions_Int_Int](./calculatearrayformula_string_calculationoptions_int_int/) | Calcule une formule en tant que formule matricielle. |
| [CalculateArrayFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_Int_Int_CalculationData](./calculatearrayformula_string_formulaparseoptions_calculationoptions_int_int_int_int_calculationdata/) | Calcule une formule en tant que formule matricielle. |
| [CalculateFormula_CalculationOptions_Bool](./calculateformula_calculationoptions_bool/) | Calcule toutes les formules de cette feuille de calcul. |
| [GetAreasOfXmlMapQuery](./getareasofxmlmapquery/) | Interroge les zones de cellules qui sont mappées/liées au chemin spécifique de la carte XML. |
| [GetCellWatches](./getcellwatches/) | Obtient la collection de cellules de cette feuille de calcul surveillée dans la 'fenêtre de surveillance'. |
| [RefreshPivotTables](./refreshpivottables/) | Actualise toutes les tableaux croisés dynamiques de cette feuille de calcul. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Actualise toutes les tableaux croisés dynamiques de cette feuille de calcul. |
