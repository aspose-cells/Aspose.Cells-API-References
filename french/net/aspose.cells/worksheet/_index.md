---
title: Worksheet
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule lobjet qui représente une seule feuille de calcul.
type: docs
weight: 6510
url: /fr/net/aspose.cells/worksheet/
---
## Worksheet class

Encapsule l'objet qui représente une seule feuille de calcul.

```csharp
public class Worksheet : IDisposable
```

## Propriétés

| Nom | La description |
| --- | --- |
| [ActiveCell](../../aspose.cells/worksheet/activecell) { get; set; } | Obtient ou définit la cellule active dans la feuille de calcul. |
| [AllowEditRanges](../../aspose.cells/worksheet/alloweditranges) { get; } | Obtient la collection de plage de modification autorisée dans la feuille de calcul. |
| [AutoFilter](../../aspose.cells/worksheet/autofilter) { get; } | Représente le filtre automatique pour la feuille de calcul spécifiée. |
| [BackgroundImage](../../aspose.cells/worksheet/backgroundimage) { get; set; } | Récupère et définit l'image d'arrière-plan de la feuille de calcul. |
| [Cells](../../aspose.cells/worksheet/cells) { get; } | Obtient le[`Cells`](./cells) collection. |
| [CellWatches](../../aspose.cells/worksheet/cellwatches) { get; } | Obtient une collection de cellules sur cette feuille de calcul en cours de surveillance dans la "fenêtre de surveillance". |
| [Charts](../../aspose.cells/worksheet/charts) { get; } | Obtient un[`Chart`](../../aspose.cells.charts/chart) collection |
| [CheckBoxes](../../aspose.cells/worksheet/checkboxes) { get; } | Obtient un[`CheckBox`](../../aspose.cells.drawing/checkbox) collection. |
| [CodeName](../../aspose.cells/worksheet/codename) { get; set; } | Obtient le nom du code de la feuille de calcul. |
| [Comments](../../aspose.cells/worksheet/comments) { get; } | Obtient le[`Comment`](../comment) collection. |
| [ConditionalFormattings](../../aspose.cells/worksheet/conditionalformattings) { get; } | Obtient les ConditionalFormattings dans la feuille de calcul. |
| [CustomProperties](../../aspose.cells/worksheet/customproperties) { get; } | Obtient un objet représentant les informations d'identification associées à une feuille de calcul. |
| [DisplayRightToLeft](../../aspose.cells/worksheet/displayrighttoleft) { get; set; } | Indique si la feuille de calcul spécifiée est affichée de droite à gauche au lieu de gauche à droite. La valeur par défaut est false. |
| [DisplayZeros](../../aspose.cells/worksheet/displayzeros) { get; set; } | Vrai si des valeurs nulles sont affichées. |
| [ErrorCheckOptions](../../aspose.cells/worksheet/errorcheckoptions) { get; } | Obtient le paramètre de vérification des erreurs appliqué à certaines plages. |
| [FirstVisibleColumn](../../aspose.cells/worksheet/firstvisiblecolumn) { get; set; } | Représente le premier index de colonne visible. |
| [FirstVisibleRow](../../aspose.cells/worksheet/firstvisiblerow) { get; set; } | Représente le premier index de ligne visible. |
| [HasAutofilter](../../aspose.cells/worksheet/hasautofilter) { get; } | Indique si cette feuille de calcul a un filtre automatique. |
| [HorizontalPageBreaks](../../aspose.cells/worksheet/horizontalpagebreaks) { get; } | Obtient le[`HorizontalPageBreakCollection`](../horizontalpagebreakcollection) le recueil. |
| [Hyperlinks](../../aspose.cells/worksheet/hyperlinks) { get; } | Obtient le[`HyperlinkCollection`](../hyperlinkcollection) collection. |
| [Index](../../aspose.cells/worksheet/index) { get; } | Obtient l'index de la feuille dans la collection de feuilles de calcul. |
| [IsGridlinesVisible](../../aspose.cells/worksheet/isgridlinesvisible) { get; set; } | Obtient ou définit une valeur indiquant si le quadrillage est visible. La valeur par défaut est true. |
| [IsOutlineShown](../../aspose.cells/worksheet/isoutlineshown) { get; set; } | Indique s'il faut afficher le contour. |
| [IsPageBreakPreview](../../aspose.cells/worksheet/ispagebreakpreview) { get; set; } | Indique si la feuille de calcul spécifiée est affichée en vue normale ou en aperçu de saut de page. |
| [IsProtected](../../aspose.cells/worksheet/isprotected) { get; } | Indique si la feuille de calcul est protégée. |
| [IsRowColumnHeadersVisible](../../aspose.cells/worksheet/isrowcolumnheadersvisible) { get; set; } | Obtient ou définit une valeur indiquant si la feuille de calcul affichera les en-têtes de ligne et de colonne. La valeur par défaut est true. |
| [IsRulerVisible](../../aspose.cells/worksheet/isrulervisible) { get; set; } | Indique si la règle est visible. Cette propriété s'applique uniquement à l'aperçu des sauts de page. |
| [IsSelected](../../aspose.cells/worksheet/isselected) { get; set; } | Indique si cette feuille de calcul est sélectionnée lorsque le classeur est ouvert. |
| [IsVisible](../../aspose.cells/worksheet/isvisible) { get; set; } | Indique si la feuille de calcul est visible. |
| [ListObjects](../../aspose.cells/worksheet/listobjects) { get; } | Obtient tous les ListObjects de cette feuille de calcul. |
| [Name](../../aspose.cells/worksheet/name) { get; set; } | Obtient ou définit le nom de la feuille de calcul. |
| [OleObjects](../../aspose.cells/worksheet/oleobjects) { get; } | Représente une collection de[`OleObject`](../../aspose.cells.drawing/oleobject) dans une feuille de calcul. |
| [Outline](../../aspose.cells/worksheet/outline) { get; } | Obtient le plan sur cette feuille de calcul. |
| [PageSetup](../../aspose.cells/worksheet/pagesetup) { get; } | Représente la description de la mise en page dans cette feuille. |
| [PaneState](../../aspose.cells/worksheet/panestate) { get; } | Indique si le volet a des fractionnements horizontaux ou verticaux, et si ces fractionnements sont figés. |
| [Pictures](../../aspose.cells/worksheet/pictures) { get; } | Obtient un[`Picture`](../../aspose.cells.drawing/picture) collection. |
| [PivotTables](../../aspose.cells/worksheet/pivottables) { get; } | Obtient tous les tableaux croisés dynamiques de cette feuille de calcul. |
| [Protection](../../aspose.cells/worksheet/protection) { get; } | Représente les différents types d'options de protection disponibles pour une feuille de calcul. Prend en charge les options de protection avancées dans ExcelXP et les versions supérieures. |
| [QueryTables](../../aspose.cells/worksheet/querytables) { get; } | Obtient[`QueryTableCollection`](../querytablecollection) dans la feuille de calcul. |
| [Scenarios](../../aspose.cells/worksheet/scenarios) { get; } | Obtient la collection de[`Scenario`](../scenario) . |
| [Shapes](../../aspose.cells/worksheet/shapes) { get; } | Renvoie toutes les formes de dessin dans cette feuille de calcul. |
| [ShowFormulas](../../aspose.cells/worksheet/showformulas) { get; set; } | Indique s'il faut afficher les formules ou leurs résultats. |
| [Slicers](../../aspose.cells/worksheet/slicers) { get; } | Obtenir la collection Slicer dans la feuille de calcul |
| [SmartTagSetting](../../aspose.cells/worksheet/smarttagsetting) { get; } | Obtient tout[`SmartTagCollection`](../../aspose.cells.markup/smarttagcollection) objets de la feuille de calcul. |
| [SparklineGroupCollection](../../aspose.cells/worksheet/sparklinegroupcollection) { get; } | Obtient la collection du groupe sparkline dans la feuille de calcul. |
| [TabColor](../../aspose.cells/worksheet/tabcolor) { get; set; } | Représente la couleur de l'onglet de la feuille de calcul. |
| [TabId](../../aspose.cells/worksheet/tabid) { get; set; } | Spécifie l'identifiant interne de la feuille. |
| [TextBoxes](../../aspose.cells/worksheet/textboxes) { get; } | Obtient un[`TextBox`](../../aspose.cells.drawing/textbox) collection. |
| [Timelines](../../aspose.cells/worksheet/timelines) { get; } | Obtenir la collection Timeline dans la feuille de calcul |
| [TransitionEntry](../../aspose.cells/worksheet/transitionentry) { get; set; } | Indique si l'option Transition Formula Entry (Compatibilité Lotus) est activée. |
| [TransitionEvaluation](../../aspose.cells/worksheet/transitionevaluation) { get; set; } | Indique si l'option Évaluation de la formule de transition (compatibilité Lotus) est activée. |
| [Type](../../aspose.cells/worksheet/type) { get; set; } | Représente le type de feuille de calcul. |
| [UniqueId](../../aspose.cells/worksheet/uniqueid) { get; set; } | Obtient et définit l'identifiant unique, il est identique à {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [Validations](../../aspose.cells/worksheet/validations) { get; } | Obtient la collection de paramètres de validation des données dans la feuille de calcul. |
| [VerticalPageBreaks](../../aspose.cells/worksheet/verticalpagebreaks) { get; } | Obtient le[`VerticalPageBreakCollection`](../verticalpagebreakcollection) collection. |
| [ViewType](../../aspose.cells/worksheet/viewtype) { get; set; } | Obtient et définit le type de vue. |
| [VisibilityType](../../aspose.cells/worksheet/visibilitytype) { get; set; } | Indique l'état visible de cette feuille. |
| [Workbook](../../aspose.cells/worksheet/workbook) { get; } | Obtient l'objet classeur qui contient cette feuille. |
| [Zoom](../../aspose.cells/worksheet/zoom) { get; set; } | Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400. |

## Méthodes

| Nom | La description |
| --- | --- |
| [AddPageBreaks](../../aspose.cells/worksheet/addpagebreaks)(string) | Ajoute un saut de page. |
| [AdvancedFilter](../../aspose.cells/worksheet/advancedfilter)(bool, string, string, string, bool) | Filtre les données à l'aide de critères complexes. |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn#autofitcolumn)(int) | Ajuste automatiquement la largeur de la colonne. |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn#autofitcolumn_1)(int, int, int) | Ajuste automatiquement la largeur de la colonne. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns)() | Ajuste automatiquement toutes les colonnes de cette feuille de calcul. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_1)(AutoFitterOptions) | Ajuste automatiquement toutes les colonnes de cette feuille de calcul. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_2)(int, int) | Ajuste automatiquement la largeur des colonnes. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_3)(int, int, AutoFitterOptions) | Ajuste automatiquement la largeur des colonnes. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_4)(int, int, int, int) | Ajuste automatiquement la largeur des colonnes. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_5)(int, int, int, int, AutoFitterOptions) | Ajuste automatiquement la largeur des colonnes. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow)(int) | Ajuste automatiquement la hauteur de ligne. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow_1)(int, int, int) | Ajuste automatiquement la hauteur de ligne. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow_2)(int, int, int, AutoFitterOptions) | Ajuste automatiquement la hauteur de ligne. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow_3)(int, int, int, int) | Ajuste automatiquement la hauteur de ligne dans une plage de rectangles. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows)() | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_1)(AutoFitterOptions) | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_2)(bool) | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_3)(int, int) | Ajuste automatiquement la hauteur de ligne dans une plage. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_4)(int, int, AutoFitterOptions) | Ajuste automatiquement la hauteur de ligne dans une plage. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula#calculateformula)(string) | Calcule une formule. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula#calculateformula_2)(CalculationOptions, bool) | Calcule toutes les formules de cette feuille de calcul. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula#calculateformula_1)(string, CalculationOptions) | Calcule une formule. |
| [ClearComments](../../aspose.cells/worksheet/clearcomments)() | Efface tous les commentaires dans la feuille de calcul du concepteur. |
| [CloseAccessCache](../../aspose.cells/worksheet/closeaccesscache)(AccessCacheOptions) | Ferme la session qui utilise des caches pour accéder aux données de cette feuille de calcul. |
| [Copy](../../aspose.cells/worksheet/copy#copy)(Worksheet) | Copie le contenu et les formats d'une autre feuille de calcul. |
| [Copy](../../aspose.cells/worksheet/copy#copy_1)(Worksheet, CopyOptions) | Copie le contenu et les formats d'une autre feuille de calcul. |
| [Dispose](../../aspose.cells/worksheet/dispose)() | Effectue des tâches définies par l'application associées à la libération, à la libération ou à la réinitialisation des ressources non gérées. |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes#freezepanes_1)(string, int, int) | Gèle les volets au niveau de la cellule spécifiée dans la feuille de calcul. |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes#freezepanes)(int, int, int, int) | Gèle les volets au niveau de la cellule spécifiée dans la feuille de calcul. |
| [GetFreezedPanes](../../aspose.cells/worksheet/getfreezedpanes)(out int, out int, out int, out int) | Obtient les volets de gel. |
| [GetPanes](../../aspose.cells/worksheet/getpanes)() | Obtient les volets de la fenêtre. |
| [GetPrintingPageBreaks](../../aspose.cells/worksheet/getprintingpagebreaks)(ImageOrPrintOptions) | Obtient des sauts de page automatiques. |
| [GetSelectedRanges](../../aspose.cells/worksheet/getselectedranges)() | Obtient les plages de cellules sélectionnées dans la feuille de calcul du concepteur. |
| [MoveTo](../../aspose.cells/worksheet/moveto)(int) | Déplace la feuille vers un autre emplacement dans la feuille de calcul. |
| [Protect](../../aspose.cells/worksheet/protect#protect)(ProtectionType) | Protège la feuille de calcul. |
| [Protect](../../aspose.cells/worksheet/protect#protect_1)(ProtectionType, string, string) | Protège la feuille de calcul. |
| [RefreshPivotTables](../../aspose.cells/worksheet/refreshpivottables)() | Actualise tous les tableaux croisés dynamiques de cette feuille de calcul. |
| [RemoveAllDrawingObjects](../../aspose.cells/worksheet/removealldrawingobjects)() | Supprime tous les objets de dessin de cette feuille de calcul. |
| [RemoveAutoFilter](../../aspose.cells/worksheet/removeautofilter)() | Supprime le filtre automatique de la feuille de calcul. |
| [RemoveSplit](../../aspose.cells/worksheet/removesplit)() | Supprime la fenêtre fractionnée. |
| [Replace](../../aspose.cells/worksheet/replace)(string, string) | Remplace le texte de toutes les cellules par une nouvelle chaîne. |
| [SelectRange](../../aspose.cells/worksheet/selectrange)(int, int, int, int, bool) | Sélectionne une plage. |
| [SetVisible](../../aspose.cells/worksheet/setvisible)(bool, bool) | Définit les options visibles. |
| [Split](../../aspose.cells/worksheet/split)() | Fractionne la fenêtre. |
| [StartAccessCache](../../aspose.cells/worksheet/startaccesscache)(AccessCacheOptions) | Démarre la session qui utilise des caches pour accéder aux données de cette feuille de calcul. |
| override [ToString](../../aspose.cells/worksheet/tostring)() | Renvoie une chaîne représentant l'objet Worksheet actuel. |
| [UnFreezePanes](../../aspose.cells/worksheet/unfreezepanes)() | Dégèle les volets de la feuille de calcul. |
| [Unprotect](../../aspose.cells/worksheet/unprotect#unprotect)() | Déprotége la feuille de calcul. |
| [Unprotect](../../aspose.cells/worksheet/unprotect#unprotect_1)(string) | Déprotége la feuille de calcul. |
| [XmlMapQuery](../../aspose.cells/worksheet/xmlmapquery)(string, XmlMap) | Interroger les zones de cellules mappées/liées au chemin spécifique de la carte xml. |

### Exemples

```csharp
[C#]

Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//Geler les volets à "AS40" avec 10 lignes et 10 colonnes
sheet.FreezePanes("AS40", 10, 10);

//Ajouter un lien hypertexte dans la cellule A1
sheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

[Visual Basic]

Dim workbook as Workbook = new Workbook()

Dim sheet as Worksheet = workbook.Worksheets(0)

'Freeze panes at "AS40" with 10 rows and 10 columns
sheet.FreezePanes("AS40", 10, 10)

'Ajouter un lien hypertexte dans la cellule A1
sheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com")
```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
