---
title: "Classe Worksheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Worksheet class. Encapsule l'objet qui représente une seule feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/
---
## Worksheet class

Encapsule l'objet qui représente une seule feuille de calcul.

```csharp
public class Worksheet : IDisposable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ActiveCell](../../aspose.cells/worksheet/activecell/) { get; set; } | Obtient ou définit la cellule active dans la feuille de calcul. |
| [AllowEditRanges](../../aspose.cells/worksheet/alloweditranges/) { get; } | Obtient la collection des plages d'édition autorisées dans la feuille de calcul. |
| [AutoFilter](../../aspose.cells/worksheet/autofilter/) { get; } | Représente le filtre automatique pour la feuille de calcul spécifiée. |
| [BackgroundImage](../../aspose.cells/worksheet/backgroundimage/) { get; set; } | Obtient et définit l'image d'arrière-plan de la feuille de calcul. |
| [Cells](../../aspose.cells/worksheet/cells/) { get; } | Obtient la collection [`Cells`](../cells/). |
| [CellWatches](../../aspose.cells/worksheet/cellwatches/) { get; } | Obtient la collection de cellules de cette feuille de calcul surveillées dans le 'watch window'. |
| [Charts](../../aspose.cells/worksheet/charts/) { get; } | Obtient une collection [`Chart`](../../aspose.cells.charts/chart/). |
| [CheckBoxes](../../aspose.cells/worksheet/checkboxes/) { get; } | Obtient une collection [`CheckBox`](../../aspose.cells.drawing/checkbox/). |
| [CodeName](../../aspose.cells/worksheet/codename/) { get; set; } | Obtient le nom de code de la feuille de calcul. |
| [Comments](../../aspose.cells/worksheet/comments/) { get; } | Obtient la collection [`Comment`](../comment/). |
| [ConditionalFormattings](../../aspose.cells/worksheet/conditionalformattings/) { get; } | Obtient les ConditionalFormattings dans la feuille de calcul. |
| [CustomProperties](../../aspose.cells/worksheet/customproperties/) { get; } | Obtient un objet représentant les informations d'identifiant associées à une feuille de calcul. |
| [DisplayRightToLeft](../../aspose.cells/worksheet/displayrighttoleft/) { get; set; } | Indique si la feuille de calcul spécifiée est affichée de droite à gauche au lieu de gauche à droite. La valeur par défaut est false. |
| [DisplayZeros](../../aspose.cells/worksheet/displayzeros/) { get; set; } | Vrai si les valeurs zéro sont affichées. |
| [ErrorCheckOptions](../../aspose.cells/worksheet/errorcheckoptions/) { get; } | Obtient le paramètre de vérification d'erreurs appliqué à certaines plages. |
| [FirstVisibleColumn](../../aspose.cells/worksheet/firstvisiblecolumn/) { get; set; } | Représente l'index de la première colonne visible. |
| [FirstVisibleRow](../../aspose.cells/worksheet/firstvisiblerow/) { get; set; } | Représente l'index de la première ligne visible. |
| [GridlineColor](../../aspose.cells/worksheet/gridlinecolor/) { get; set; } | Obtient et définit la couleur de la ligne de grille |
| [HasAutofilter](../../aspose.cells/worksheet/hasautofilter/) { get; } | Indique si cette feuille de calcul possède un filtre automatique. |
| [HorizontalPageBreaks](../../aspose.cells/worksheet/horizontalpagebreaks/) { get; } | Obtient la collection [`HorizontalPageBreakCollection`](../horizontalpagebreakcollection/). |
| [Hyperlinks](../../aspose.cells/worksheet/hyperlinks/) { get; } | Obtient la collection [`HyperlinkCollection`](../hyperlinkcollection/). |
| [Index](../../aspose.cells/worksheet/index/) { get; } | Obtient l'index de la feuille dans la collection de feuilles de calcul. |
| [IsGridlinesVisible](../../aspose.cells/worksheet/isgridlinesvisible/) { get; set; } | Obtient ou définit une valeur indiquant si les lignes de grille sont visibles. La valeur par défaut est true. |
| [IsOutlineShown](../../aspose.cells/worksheet/isoutlineshown/) { get; set; } | Indique s'il faut afficher le contour. |
| [IsPageBreakPreview](../../aspose.cells/worksheet/ispagebreakpreview/) { get; set; } | Indique si la feuille de calcul spécifiée est affichée en mode normal ou en aperçu des sauts de page. |
| [IsProtected](../../aspose.cells/worksheet/isprotected/) { get; } | Indique si la feuille de calcul est protégée. |
| [IsRowColumnHeadersVisible](../../aspose.cells/worksheet/isrowcolumnheadersvisible/) { get; set; } | Obtient ou définit une valeur indiquant si la feuille de calcul affichera les en-têtes de lignes et de colonnes. La valeur par défaut est true. |
| [IsRulerVisible](../../aspose.cells/worksheet/isrulervisible/) { get; set; } | Indique si la règle est visible. Cette propriété n'est appliquée que pour l'aperçu des sauts de page. |
| [IsSelected](../../aspose.cells/worksheet/isselected/) { get; set; } | Indique si cette feuille de calcul est sélectionnée lorsque le classeur est ouvert. |
| [IsVisible](../../aspose.cells/worksheet/isvisible/) { get; set; } | Représente si la feuille de calcul est visible. |
| [ListObjects](../../aspose.cells/worksheet/listobjects/) { get; } | Obtient tous les ListObjects dans cette feuille de calcul. |
| [Name](../../aspose.cells/worksheet/name/) { get; set; } | Obtient ou définit le nom de la feuille de calcul. |
| [OleObjects](../../aspose.cells/worksheet/oleobjects/) { get; } | Représente une collection de [`OleObject`](../../aspose.cells.drawing/oleobject/) dans une feuille de calcul. |
| [Outline](../../aspose.cells/worksheet/outline/) { get; } | Obtient le contour de cette feuille de calcul. |
| [PageSetup](../../aspose.cells/worksheet/pagesetup/) { get; } | Représente la description de la mise en page de cette feuille. |
| [PaneState](../../aspose.cells/worksheet/panestate/) { get; } | Indique si le volet possède des séparations horizontales ou verticales, et si ces séparations sont figées. |
| [Pictures](../../aspose.cells/worksheet/pictures/) { get; } | Obtient une collection [`Picture`](../../aspose.cells.drawing/picture/). |
| [PivotTables](../../aspose.cells/worksheet/pivottables/) { get; } | Obtient tous les tableaux croisés dynamiques de cette feuille de calcul. |
| [Protection](../../aspose.cells/worksheet/protection/) { get; } | Représente les différents types d'options de protection disponibles pour une feuille de calcul. Prend en charge les options de protection avancées dans ExcelXP et les versions ultérieures. |
| [QueryTables](../../aspose.cells/worksheet/querytables/) { get; } | Obtient [`QueryTableCollection`](../querytablecollection/) dans la feuille de calcul. |
| [Scenarios](../../aspose.cells/worksheet/scenarios/) { get; } | Obtient la collection de [`Scenario`](../scenario/). |
| [Shapes](../../aspose.cells/worksheet/shapes/) { get; } | Renvoie toutes les formes de dessin de cette feuille de calcul. |
| [ShowDataTypeIcons](../../aspose.cells/worksheet/showdatatypeicons/) { get; set; } | Indique s'il faut afficher les icônes de type de données. |
| [ShowFormulas](../../aspose.cells/worksheet/showformulas/) { get; set; } | Indique s'il faut afficher les formules ou leurs résultats. |
| [Slicers](../../aspose.cells/worksheet/slicers/) { get; } | Obtenez la collection Slicer dans la feuille de calcul |
| [SmartTagSetting](../../aspose.cells/worksheet/smarttagsetting/) { get; } | Obtient tous les objets [`SmartTagCollection`](../../aspose.cells.markup/smarttagcollection/) de la feuille de calcul. |
| [SparklineGroups](../../aspose.cells/worksheet/sparklinegroups/) { get; } | Obtient les groupes de sparkline dans la feuille de calcul. |
| [TabColor](../../aspose.cells/worksheet/tabcolor/) { get; set; } | Représente la couleur de l'onglet de la feuille de calcul. |
| [TabId](../../aspose.cells/worksheet/tabid/) { get; set; } | Spécifie l'identifiant interne de la feuille. |
| [TextBoxes](../../aspose.cells/worksheet/textboxes/) { get; } | Obtient une collection [`TextBox`](../../aspose.cells.drawing/textbox/). |
| [Timelines](../../aspose.cells/worksheet/timelines/) { get; } | Obtenez la collection Timeline dans la feuille de calcul |
| [TransitionEntry](../../aspose.cells/worksheet/transitionentry/) { get; set; } | Indique si l'option Transition Formula Entry (compatibilité Lotus) est activée. |
| [TransitionEvaluation](../../aspose.cells/worksheet/transitionevaluation/) { get; set; } | Indique si l'option Transition Formula Evaluation (compatibilité Lotus) est activée. |
| [Type](../../aspose.cells/worksheet/type/) { get; set; } | Représente le type de feuille de calcul. |
| [UniqueId](../../aspose.cells/worksheet/uniqueid/) { get; set; } | Obtient et définit l'ID unique, il est identique à {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [Validations](../../aspose.cells/worksheet/validations/) { get; } | Obtient la collection des paramètres de validation des données dans la feuille de calcul. |
| [VerticalPageBreaks](../../aspose.cells/worksheet/verticalpagebreaks/) { get; } | Obtient la collection [`VerticalPageBreakCollection`](../verticalpagebreakcollection/). |
| [ViewType](../../aspose.cells/worksheet/viewtype/) { get; set; } | Obtient et définit le type de vue. |
| [VisibilityType](../../aspose.cells/worksheet/visibilitytype/) { get; set; } | Indique l'état de visibilité de cette feuille. |
| [Workbook](../../aspose.cells/worksheet/workbook/) { get; } | Obtient l'objet classeur qui contient cette feuille. |
| [Zoom](../../aspose.cells/worksheet/zoom/) { get; set; } | Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddPageBreaks](../../aspose.cells/worksheet/addpagebreaks/)(string) | Ajoute un saut de page. |
| [AdvancedFilter](../../aspose.cells/worksheet/advancedfilter/)(bool, string, string, string, bool) | Filtre les données en utilisant des critères complexes. |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn/#autofitcolumn)(int) | Ajuste automatiquement la largeur de la colonne. |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Ajuste automatiquement la largeur de la colonne. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns)() | Ajuste automatiquement toutes les colonnes de cette feuille de calcul. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_1)(AutoFitterOptions) | Ajuste automatiquement toutes les colonnes de cette feuille de calcul. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_2)(int, int) | Ajuste automatiquement la largeur des colonnes. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_3)(int, int, AutoFitterOptions) | Ajuste automatiquement la largeur des colonnes. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_4)(int, int, int, int) | Ajuste automatiquement la largeur des colonnes. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_5)(int, int, int, int, AutoFitterOptions) | Ajuste automatiquement la largeur des colonnes. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow/#autofitrow)(int) | Ajuste automatiquement la hauteur de la ligne. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow/#autofitrow_1)(int, int, int) | Ajuste automatiquement la hauteur de la ligne. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow/#autofitrow_2)(int, int, int, AutoFitterOptions) | Ajuste automatiquement la hauteur de la ligne. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow/#autofitrow_3)(int, int, int, int) | Ajuste automatiquement la hauteur de la ligne dans une plage rectangulaire. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows)() | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows_1)(AutoFitterOptions) | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows_2)(bool) | Ajuste automatiquement toutes les lignes de cette feuille de calcul. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows_3)(int, int) | Ajuste automatiquement la hauteur de la ligne dans une plage. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows_4)(int, int, AutoFitterOptions) | Ajuste automatiquement la hauteur de la ligne dans une plage. |
| [CalculateArrayFormula](../../aspose.cells/worksheet/calculatearrayformula/#calculatearrayformula)(string, CalculationOptions) | Calcule une formule en tant que formule matricielle. |
| [CalculateArrayFormula](../../aspose.cells/worksheet/calculatearrayformula/#calculatearrayformula_1)(string, CalculationOptions, int, int) | Calcule une formule en tant que formule matricielle. |
| [CalculateArrayFormula](../../aspose.cells/worksheet/calculatearrayformula/#calculatearrayformula_2)(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) | Calcule une formule en tant que formule matricielle. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula/#calculateformula)(string) | Calcule une formule. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula/#calculateformula_3)(CalculationOptions, bool) | Calcule toutes les formules de cette feuille de calcul. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula/#calculateformula_1)(string, CalculationOptions) | Calcule directement une expression de formule. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula/#calculateformula_2)(string, FormulaParseOptions, CalculationOptions, int, int, CalculationData) | Calcule directement une expression de formule. |
| [ClearComments](../../aspose.cells/worksheet/clearcomments/)() | Efface tous les commentaires dans la feuille de calcul du concepteur. |
| [CloseAccessCache](../../aspose.cells/worksheet/closeaccesscache/)(AccessCacheOptions) | Ferme la session qui utilise des caches pour accéder aux données de cette feuille de calcul. |
| [ConvertFormulaReferenceStyle](../../aspose.cells/worksheet/convertformulareferencestyle/)(string, bool, int, int) | Convertit le style de référence de la formule. |
| [Copy](../../aspose.cells/worksheet/copy/#copy)(Worksheet) | Copie le contenu et les formats d'une autre feuille de calcul. |
| [Copy](../../aspose.cells/worksheet/copy/#copy_1)(Worksheet, CopyOptions) | Copie le contenu et les formats d'une autre feuille de calcul. |
| [Dispose](../../aspose.cells/worksheet/dispose/)() | Effectue des tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [Filter](../../aspose.cells/worksheet/filter/)(CellArea) | Filtre la plage. |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes/#freezepanes_1)(string, int, int) | Gèle les volets à la cellule spécifiée dans la feuille de calcul. |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes/#freezepanes)(int, int, int, int) | Gèle les volets à la cellule spécifiée dans la feuille de calcul. |
| [GetAdvancedFilter](../../aspose.cells/worksheet/getadvancedfilter/)() | Obtient les paramètres du filtre avancé. |
| [GetAllPictures](../../aspose.cells/worksheet/getallpictures/)() | Obtient toutes les images, y compris celles intégrées dans la cellule et au-dessus des cellules. |
| [GetAreasOfXmlMapQuery](../../aspose.cells/worksheet/getareasofxmlmapquery/)(string, XmlMap) | Interroge les zones de cellules qui sont mappées/liées au chemin spécifique de la carte XML. |
| [GetFreezedPanes](../../aspose.cells/worksheet/getfreezedpanes/)(out int, out int, out int, out int) | Obtient les volets figés. |
| [GetPanes](../../aspose.cells/worksheet/getpanes/)() | Obtient les volets de la fenêtre. |
| [GetPrintingPageBreaks](../../aspose.cells/worksheet/getprintingpagebreaks/)(ImageOrPrintOptions) | Obtient les sauts de page automatiques. |
| [GetSelectedAreas](../../aspose.cells/worksheet/getselectedareas/)() | Obtient les plages de cellules sélectionnées dans la feuille de calcul du concepteur. |
| [GetSelectedRanges](../../aspose.cells/worksheet/getselectedranges/)() | (**Obsolete.**) Obtient les plages de cellules sélectionnées dans la feuille de calcul du concepteur. |
| [MoveTo](../../aspose.cells/worksheet/moveto/)(int) | Déplace la feuille vers un autre emplacement dans la feuille de calcul. |
| [Protect](../../aspose.cells/worksheet/protect/#protect)(ProtectionType) | Protège la feuille de calcul. |
| [Protect](../../aspose.cells/worksheet/protect/#protect_1)(ProtectionType, string, string) | Protège la feuille de calcul. |
| [RefreshPivotTables](../../aspose.cells/worksheet/refreshpivottables/#refreshpivottables_1)() | Actualise tous les tableaux croisés dynamiques de cette feuille de calcul. |
| [RefreshPivotTables](../../aspose.cells/worksheet/refreshpivottables/#refreshpivottables)(PivotTableRefreshOption) | Actualise tous les tableaux croisés dynamiques de cette feuille de calcul. |
| [RemoveAllDrawingObjects](../../aspose.cells/worksheet/removealldrawingobjects/)() | Supprime tous les objets de dessin de cette feuille de calcul. |
| [RemoveAutoFilter](../../aspose.cells/worksheet/removeautofilter/)() | Supprime le filtre automatique de la feuille de calcul. |
| [RemoveSplit](../../aspose.cells/worksheet/removesplit/)() | Supprime la fenêtre fractionnée. |
| [Replace](../../aspose.cells/worksheet/replace/)(string, string) | Remplace le texte de toutes les cellules par une nouvelle chaîne. |
| [SelectRange](../../aspose.cells/worksheet/selectrange/)(int, int, int, int, bool) | Sélectionne une plage. |
| [SetVisible](../../aspose.cells/worksheet/setvisible/)(bool, bool) | Définit les options visibles. |
| [Split](../../aspose.cells/worksheet/split/)() | Fractionne la fenêtre. |
| [StartAccessCache](../../aspose.cells/worksheet/startaccesscache/)(AccessCacheOptions) | Démarre la session qui utilise des caches pour accéder aux données de cette feuille de calcul. |
| override [ToString](../../aspose.cells/worksheet/tostring/)() | Renvoie une chaîne qui représente l'objet feuille de calcul actuel. |
| [UnFreezePanes](../../aspose.cells/worksheet/unfreezepanes/)() | Défige les volets dans la feuille de calcul. |
| [Unprotect](../../aspose.cells/worksheet/unprotect/#unprotect)() | Supprime la protection de la feuille de calcul. |
| [Unprotect](../../aspose.cells/worksheet/unprotect/#unprotect_1)(string) | Supprime la protection de la feuille de calcul. |
| [XmlMapQuery](../../aspose.cells/worksheet/xmlmapquery/)(string, XmlMap) | (**Obsolete.**) Interroge les zones de cellules qui sont mappées/liées au chemin spécifique de la carte XML. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetDemo
    {
        public static void WorksheetExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir les propriétés de la feuille de calcul
            worksheet.Name = "DemoSheet";
            worksheet.IsGridlinesVisible = true;
            worksheet.IsRowColumnHeadersVisible = true;
            worksheet.DisplayZeros = true;
            worksheet.DisplayRightToLeft = false;
            worksheet.IsOutlineShown = true;
            worksheet.IsSelected = true;
            worksheet.FirstVisibleRow = 0;
            worksheet.FirstVisibleColumn = 0;
            worksheet.Zoom = 100;
            worksheet.ViewType = ViewType.PageLayoutView;
            worksheet.IsPageBreakPreview = false;
            worksheet.IsRulerVisible = true;
            worksheet.TabColor = System.Drawing.Color.Blue;
            worksheet.CodeName = "Sheet1";
            worksheet.ActiveCell = "A1";

            // Ajouter un hyperlien dans la cellule A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Figer les volets à "C3" avec 3 lignes et 3 colonnes
            worksheet.FreezePanes("C3", 3, 3);

            // Ajouter une règle de mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Définition des propriétés pour la règle AboveAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // Enregistrez le classeur
            workbook.Save("WorksheetExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


