---
title: "Classe Worksheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Worksheet. Incapsula l'oggetto che rappresenta un singolo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/
---
## Worksheet class

Incapsula l'oggetto che rappresenta un singolo foglio di lavoro.

```csharp
public class Worksheet : IDisposable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActiveCell](../../aspose.cells/worksheet/activecell/) { get; set; } | Ottiene o imposta la cella attiva nel foglio di lavoro. |
| [AllowEditRanges](../../aspose.cells/worksheet/alloweditranges/) { get; } | Ottiene la collezione di intervalli di modifica consentiti nel foglio di lavoro. |
| [AutoFilter](../../aspose.cells/worksheet/autofilter/) { get; } | Rappresenta il filtro automatico per il foglio di lavoro specificato. |
| [BackgroundImage](../../aspose.cells/worksheet/backgroundimage/) { get; set; } | Ottiene e imposta l'immagine di sfondo del foglio di lavoro. |
| [Cells](../../aspose.cells/worksheet/cells/) { get; } | Ottiene la collezione [`Cells`](../cells/). |
| [CellWatches](../../aspose.cells/worksheet/cellwatches/) { get; } | Ottiene la collezione di celle di questo foglio di lavoro monitorate nella 'watch window'. |
| [Charts](../../aspose.cells/worksheet/charts/) { get; } | Ottiene una collezione [`Chart`](../../aspose.cells.charts/chart/) |
| [CheckBoxes](../../aspose.cells/worksheet/checkboxes/) { get; } | Ottiene una collezione [`CheckBox`](../../aspose.cells.drawing/checkbox/). |
| [CodeName](../../aspose.cells/worksheet/codename/) { get; set; } | Ottiene il nome codice del foglio di lavoro. |
| [Comments](../../aspose.cells/worksheet/comments/) { get; } | Ottiene la collezione [`Comment`](../comment/). |
| [ConditionalFormattings](../../aspose.cells/worksheet/conditionalformattings/) { get; } | Ottiene i ConditionalFormattings nel foglio di lavoro. |
| [CustomProperties](../../aspose.cells/worksheet/customproperties/) { get; } | Ottiene un oggetto che rappresenta le informazioni di identificatore associate a un foglio di lavoro. |
| [DisplayRightToLeft](../../aspose.cells/worksheet/displayrighttoleft/) { get; set; } | Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra invece che da sinistra a destra. Il valore predefinito è false. |
| [DisplayZeros](../../aspose.cells/worksheet/displayzeros/) { get; set; } | True se i valori zero sono visualizzati. |
| [ErrorCheckOptions](../../aspose.cells/worksheet/errorcheckoptions/) { get; } | Ottiene l'impostazione di controllo errori applicata su alcuni intervalli. |
| [FirstVisibleColumn](../../aspose.cells/worksheet/firstvisiblecolumn/) { get; set; } | Rappresenta l'indice della prima colonna visibile. |
| [FirstVisibleRow](../../aspose.cells/worksheet/firstvisiblerow/) { get; set; } | Rappresenta l'indice della prima riga visibile. |
| [GridlineColor](../../aspose.cells/worksheet/gridlinecolor/) { get; set; } | Ottiene e imposta il colore della griglia |
| [HasAutofilter](../../aspose.cells/worksheet/hasautofilter/) { get; } | Indica se questo foglio di lavoro ha un filtro automatico. |
| [HorizontalPageBreaks](../../aspose.cells/worksheet/horizontalpagebreaks/) { get; } | Ottiene la collezione [`HorizontalPageBreakCollection`](../horizontalpagebreakcollection/). |
| [Hyperlinks](../../aspose.cells/worksheet/hyperlinks/) { get; } | Ottiene la collezione [`HyperlinkCollection`](../hyperlinkcollection/). |
| [Index](../../aspose.cells/worksheet/index/) { get; } | Ottiene l'indice del foglio nella collezione dei fogli di lavoro. |
| [IsGridlinesVisible](../../aspose.cells/worksheet/isgridlinesvisible/) { get; set; } | Ottiene o imposta un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true. |
| [IsOutlineShown](../../aspose.cells/worksheet/isoutlineshown/) { get; set; } | Indica se mostrare la struttura. |
| [IsPageBreakPreview](../../aspose.cells/worksheet/ispagebreakpreview/) { get; set; } | Indica se il foglio di lavoro specificato è mostrato nella visualizzazione normale o nell'anteprima interruzione di pagina. |
| [IsProtected](../../aspose.cells/worksheet/isprotected/) { get; } | Indica se il foglio di lavoro è protetto. |
| [IsRowColumnHeadersVisible](../../aspose.cells/worksheet/isrowcolumnheadersvisible/) { get; set; } | Ottiene o imposta un valore che indica se il foglio di lavoro visualizzerà le intestazioni di righe e colonne. Il valore predefinito è true. |
| [IsRulerVisible](../../aspose.cells/worksheet/isrulervisible/) { get; set; } | Indica se il righello è visibile. Questa proprietà è applicata solo per l'anteprima interruzione di pagina. |
| [IsSelected](../../aspose.cells/worksheet/isselected/) { get; set; } | Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta. |
| [IsVisible](../../aspose.cells/worksheet/isvisible/) { get; set; } | Rappresenta se il foglio di lavoro è visibile. |
| [ListObjects](../../aspose.cells/worksheet/listobjects/) { get; } | Ottiene tutti i ListObjects in questo foglio di lavoro. |
| [Name](../../aspose.cells/worksheet/name/) { get; set; } | Ottiene o imposta il nome del foglio di lavoro. |
| [OleObjects](../../aspose.cells/worksheet/oleobjects/) { get; } | Rappresenta una collezione di [`OleObject`](../../aspose.cells.drawing/oleobject/) in un foglio di lavoro. |
| [Outline](../../aspose.cells/worksheet/outline/) { get; } | Ottiene la struttura in questo foglio di lavoro. |
| [PageSetup](../../aspose.cells/worksheet/pagesetup/) { get; } | Rappresenta la descrizione dell'impostazione della pagina in questo foglio. |
| [PaneState](../../aspose.cells/worksheet/panestate/) { get; } | Indica se il riquadro ha divisioni orizzontali o verticali e se tali divisioni sono bloccate. |
| [Pictures](../../aspose.cells/worksheet/pictures/) { get; } | Ottiene una collezione di [`Picture`](../../aspose.cells.drawing/picture/). |
| [PivotTables](../../aspose.cells/worksheet/pivottables/) { get; } | Ottiene tutte le tabelle pivot in questo foglio di lavoro. |
| [Protection](../../aspose.cells/worksheet/protection/) { get; } | Rappresenta i vari tipi di opzioni di protezione disponibili per un foglio di lavoro. Supporta opzioni di protezione avanzate in ExcelXP e versioni successive. |
| [QueryTables](../../aspose.cells/worksheet/querytables/) { get; } | Ottiene [`QueryTableCollection`](../querytablecollection/) nel foglio di lavoro. |
| [Scenarios](../../aspose.cells/worksheet/scenarios/) { get; } | Ottiene la collezione di [`Scenario`](../scenario/). |
| [Shapes](../../aspose.cells/worksheet/shapes/) { get; } | Restituisce tutte le forme di disegno in questo foglio di lavoro. |
| [ShowDataTypeIcons](../../aspose.cells/worksheet/showdatatypeicons/) { get; set; } | Indica se mostrare le icone del tipo di dato. |
| [ShowFormulas](../../aspose.cells/worksheet/showformulas/) { get; set; } | Indica se mostrare le formule o i loro risultati. |
| [Slicers](../../aspose.cells/worksheet/slicers/) { get; } | Ottieni la collezione di Slicer nel foglio di lavoro |
| [SmartTagSetting](../../aspose.cells/worksheet/smarttagsetting/) { get; } | Ottiene tutti gli oggetti [`SmartTagCollection`](../../aspose.cells.markup/smarttagcollection/) del foglio di lavoro. |
| [SparklineGroups](../../aspose.cells/worksheet/sparklinegroups/) { get; } | Ottiene i gruppi di sparkline nel foglio di lavoro. |
| [TabColor](../../aspose.cells/worksheet/tabcolor/) { get; set; } | Rappresenta il colore della scheda del foglio di lavoro. |
| [TabId](../../aspose.cells/worksheet/tabid/) { get; set; } | Specifica l'identificatore interno per il foglio. |
| [TextBoxes](../../aspose.cells/worksheet/textboxes/) { get; } | Ottiene una collezione di [`TextBox`](../../aspose.cells.drawing/textbox/). |
| [Timelines](../../aspose.cells/worksheet/timelines/) { get; } | Ottieni la collezione di Timeline nel foglio di lavoro |
| [TransitionEntry](../../aspose.cells/worksheet/transitionentry/) { get; set; } | Indica se l'opzione Transition Formula Entry (compatibilità Lotus) è abilitata. |
| [TransitionEvaluation](../../aspose.cells/worksheet/transitionevaluation/) { get; set; } | Indica se l'opzione Transition Formula Evaluation (compatibilità Lotus) è abilitata. |
| [Type](../../aspose.cells/worksheet/type/) { get; set; } | Rappresenta il tipo di foglio di lavoro. |
| [UniqueId](../../aspose.cells/worksheet/uniqueid/) { get; set; } | Ottiene e imposta l'ID univoco, è lo stesso di {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [Validations](../../aspose.cells/worksheet/validations/) { get; } | Ottiene la collezione delle impostazioni di convalida dei dati nel foglio di lavoro. |
| [VerticalPageBreaks](../../aspose.cells/worksheet/verticalpagebreaks/) { get; } | Ottiene la collezione [`VerticalPageBreakCollection`](../verticalpagebreakcollection/). |
| [ViewType](../../aspose.cells/worksheet/viewtype/) { get; set; } | Ottiene e imposta il tipo di visualizzazione. |
| [VisibilityType](../../aspose.cells/worksheet/visibilitytype/) { get; set; } | Indica lo stato di visibilità per questo foglio. |
| [Workbook](../../aspose.cells/worksheet/workbook/) { get; } | Ottiene l'oggetto cartella di lavoro che contiene questo foglio. |
| [Zoom](../../aspose.cells/worksheet/zoom/) { get; set; } | Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddPageBreaks](../../aspose.cells/worksheet/addpagebreaks/)(string) | Aggiunge un'interruzione di pagina. |
| [AdvancedFilter](../../aspose.cells/worksheet/advancedfilter/)(bool, string, string, string, bool) | Filtra i dati usando criteri complessi. |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn/#autofitcolumn)(int) | Adatta automaticamente la larghezza della colonna. |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Adatta automaticamente la larghezza della colonna. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns)() | Adatta automaticamente tutte le colonne in questo foglio di lavoro. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_1)(AutoFitterOptions) | Adatta automaticamente tutte le colonne in questo foglio di lavoro. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_2)(int, int) | Adatta automaticamente la larghezza delle colonne. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_3)(int, int, AutoFitterOptions) | Adatta automaticamente la larghezza delle colonne. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_4)(int, int, int, int) | Adatta automaticamente la larghezza delle colonne. |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns/#autofitcolumns_5)(int, int, int, int, AutoFitterOptions) | Adatta automaticamente la larghezza delle colonne. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow/#autofitrow)(int) | Adatta automaticamente l'altezza della riga. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow/#autofitrow_1)(int, int, int) | Adatta automaticamente l'altezza della riga. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow/#autofitrow_2)(int, int, int, AutoFitterOptions) | Adatta automaticamente l'altezza della riga. |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow/#autofitrow_3)(int, int, int, int) | Adatta automaticamente l'altezza della riga in un intervallo rettangolare. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows)() | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows_1)(AutoFitterOptions) | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows_2)(bool) | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows_3)(int, int) | Adatta automaticamente l'altezza della riga in un intervallo. |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows/#autofitrows_4)(int, int, AutoFitterOptions) | Adatta automaticamente l'altezza della riga in un intervallo. |
| [CalculateArrayFormula](../../aspose.cells/worksheet/calculatearrayformula/#calculatearrayformula)(string, CalculationOptions) | Calcola una formula come formula di matrice. |
| [CalculateArrayFormula](../../aspose.cells/worksheet/calculatearrayformula/#calculatearrayformula_1)(string, CalculationOptions, int, int) | Calcola una formula come formula di matrice. |
| [CalculateArrayFormula](../../aspose.cells/worksheet/calculatearrayformula/#calculatearrayformula_2)(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) | Calcola una formula come formula di matrice. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula/#calculateformula)(string) | Calcola una formula. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula/#calculateformula_3)(CalculationOptions, bool) | Calcola tutte le formule in questo foglio di lavoro. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula/#calculateformula_1)(string, CalculationOptions) | Calcola direttamente un'espressione di formula. |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula/#calculateformula_2)(string, FormulaParseOptions, CalculationOptions, int, int, CalculationData) | Calcola direttamente un'espressione di formula. |
| [ClearComments](../../aspose.cells/worksheet/clearcomments/)() | Cancella tutti i commenti nel foglio di calcolo del designer. |
| [CloseAccessCache](../../aspose.cells/worksheet/closeaccesscache/)(AccessCacheOptions) | Chiude la sessione che utilizza cache per accedere ai dati in questo foglio di lavoro. |
| [ConvertFormulaReferenceStyle](../../aspose.cells/worksheet/convertformulareferencestyle/)(string, bool, int, int) | Converte lo stile di riferimento della formula. |
| [Copy](../../aspose.cells/worksheet/copy/#copy)(Worksheet) | Copia contenuti e formati da un altro foglio di lavoro. |
| [Copy](../../aspose.cells/worksheet/copy/#copy_1)(Worksheet, CopyOptions) | Copia contenuti e formati da un altro foglio di lavoro. |
| [Dispose](../../aspose.cells/worksheet/dispose/)() | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al reset delle risorse non gestite. |
| [Filter](../../aspose.cells/worksheet/filter/)(CellArea) | Filtra l'intervallo. |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes/#freezepanes_1)(string, int, int) | Blocca i riquadri nella cella specificata nel foglio di lavoro. |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes/#freezepanes)(int, int, int, int) | Blocca i riquadri nella cella specificata nel foglio di lavoro. |
| [GetAdvancedFilter](../../aspose.cells/worksheet/getadvancedfilter/)() | Ottiene le impostazioni del filtro avanzato. |
| [GetAllPictures](../../aspose.cells/worksheet/getallpictures/)() | Ottiene tutte le immagini, incluse quelle incorporate nella cella e sopra le celle. |
| [GetAreasOfXmlMapQuery](../../aspose.cells/worksheet/getareasofxmlmapquery/)(string, XmlMap) | Interroga le aree di celle mappate/collegate al percorso specifico della mappa XML. |
| [GetFreezedPanes](../../aspose.cells/worksheet/getfreezedpanes/)(out int, out int, out int, out int) | Ottiene i riquadri congelati. |
| [GetPanes](../../aspose.cells/worksheet/getpanes/)() | Ottiene i riquadri della finestra. |
| [GetPrintingPageBreaks](../../aspose.cells/worksheet/getprintingpagebreaks/)(ImageOrPrintOptions) | Ottiene le interruzioni di pagina automatiche. |
| [GetSelectedAreas](../../aspose.cells/worksheet/getselectedareas/)() | Ottiene gli intervalli selezionati di celle nel foglio di calcolo del designer. |
| [GetSelectedRanges](../../aspose.cells/worksheet/getselectedranges/)() | (**Obsolete.**) Ottiene gli intervalli selezionati di celle nel foglio di calcolo del designer. |
| [MoveTo](../../aspose.cells/worksheet/moveto/)(int) | Sposta il foglio in un'altra posizione nel foglio di calcolo. |
| [Protect](../../aspose.cells/worksheet/protect/#protect)(ProtectionType) | Protegge il worksheet. |
| [Protect](../../aspose.cells/worksheet/protect/#protect_1)(ProtectionType, string, string) | Protegge il worksheet. |
| [RefreshPivotTables](../../aspose.cells/worksheet/refreshpivottables/#refreshpivottables_1)() | Aggiorna tutte le PivotTables in questo Worksheet. |
| [RefreshPivotTables](../../aspose.cells/worksheet/refreshpivottables/#refreshpivottables)(PivotTableRefreshOption) | Aggiorna tutte le PivotTables in questo Worksheet. |
| [RemoveAllDrawingObjects](../../aspose.cells/worksheet/removealldrawingobjects/)() | Rimuove tutti gli oggetti di disegno in questo worksheet. |
| [RemoveAutoFilter](../../aspose.cells/worksheet/removeautofilter/)() | Rimuove il filtro automatico del worksheet. |
| [RemoveSplit](../../aspose.cells/worksheet/removesplit/)() | Rimuove la divisione della finestra. |
| [Replace](../../aspose.cells/worksheet/replace/)(string, string) | Sostituisce il testo di tutte le celle con una nuova stringa. |
| [SelectRange](../../aspose.cells/worksheet/selectrange/)(int, int, int, int, bool) | Seleziona un intervallo. |
| [SetVisible](../../aspose.cells/worksheet/setvisible/)(bool, bool) | Imposta le opzioni visibili. |
| [Split](../../aspose.cells/worksheet/split/)() | Dividi la finestra. |
| [StartAccessCache](../../aspose.cells/worksheet/startaccesscache/)(AccessCacheOptions) | Avvia la sessione che utilizza cache per accedere ai dati in questo worksheet. |
| override [ToString](../../aspose.cells/worksheet/tostring/)() | Restituisce una stringa che rappresenta l'oggetto Worksheet corrente. |
| [UnFreezePanes](../../aspose.cells/worksheet/unfreezepanes/)() | Sblocca i riquadri nel worksheet. |
| [Unprotect](../../aspose.cells/worksheet/unprotect/#unprotect)() | Rimuove la protezione del worksheet. |
| [Unprotect](../../aspose.cells/worksheet/unprotect/#unprotect_1)(string) | Rimuove la protezione del worksheet. |
| [XmlMapQuery](../../aspose.cells/worksheet/xmlmapquery/)(string, XmlMap) | (**Obsolete.**) Interroga le aree di celle mappate/collegate al percorso specifico della mappa xml. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetDemo
    {
        public static void WorksheetExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta le proprietà del worksheet
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

            // Aggiungi un collegamento ipertestuale in Cell A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Blocca i riquadri a "C3" con 3 righe e 3 colonne
            worksheet.FreezePanes("C3", 3, 3);

            // Aggiungi una regola di formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Impostazione delle proprietà per la regola AboveAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // Salva la cartella di lavoro
            workbook.Save("WorksheetExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


