---
title: "Classe Worksheet"
linktitle: "Worksheet"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe Worksheet. Incapsula l'oggetto che rappresenta il foglio di lavoro in Go."
type: docs
weight: 200
url: /it/go-cpp/worksheet/
---

## Worksheet class

Incapsula l'oggetto che rappresenta un singolo foglio di lavoro.

```go

type Worksheet struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [Dispose](./dispose/) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino delle risorse non gestite. |
| [GetProtection](./getprotection/) | Rappresenta i vari tipi di opzioni di protezione disponibili per un foglio di lavoro. Supporta opzioni di protezione avanzate in ExcelXP e versioni successive. |
| [GetUniqueId](./getuniqueid/) | Ottiene e imposta l'ID univoco, è lo stesso di {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [SetUniqueId](./setuniqueid/) | Ottiene e imposta l'ID univoco, è lo stesso di {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}. |
| [GetPanes](./getpanes/) | Ottiene i riquadri della finestra. |
| [GetWorkbook](./getworkbook/) | Ottiene l'oggetto cartella di lavoro che contiene questo foglio. |
| [GetCells](./getcells/) | Ottiene la collezione Aspose.Cells.Cells. |
| [GetQueryTables](./getquerytables/) | Ottiene QueryTableCollection nel foglio di lavoro. |
| [GetType](./gettype/) | Rappresenta il tipo di foglio di lavoro. |
| [SetType](./settype/) | Rappresenta il tipo di foglio di lavoro. |
| [GetName](./getname/) | Ottiene o imposta il nome del foglio di lavoro. |
| [SetName](./setname/) | Ottiene o imposta il nome del foglio di lavoro. |
| [GetShowFormulas](./getshowformulas/) | Indica se mostrare le formule o i loro risultati. |
| [SetShowFormulas](./setshowformulas/) | Indica se mostrare le formule o i loro risultati. |
| [GetShowDataTypeIcons](./getshowdatatypeicons/) | Indica se mostrare le icone del tipo di dati. |
| [SetShowDataTypeIcons](./setshowdatatypeicons/) | Indica se mostrare le icone del tipo di dati. |
| [IsGridlinesVisible](./isgridlinesvisible/) | Ottiene o imposta un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true. |
| [SetIsGridlinesVisible](./setisgridlinesvisible/) | Ottiene o imposta un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true. |
| [IsRowColumnHeadersVisible](./isrowcolumnheadersvisible/) | Ottiene o imposta un valore che indica se il foglio di lavoro visualizzerà le intestazioni di righe e colonne. Il valore predefinito è true. |
| [SetIsRowColumnHeadersVisible](./setisrowcolumnheadersvisible/) | Ottiene o imposta un valore che indica se il foglio di lavoro visualizzerà le intestazioni di righe e colonne. Il valore predefinito è true. |
| [GetPaneState](./getpanestate/) | Indica se il riquadro ha divisioni orizzontali o verticali e se tali divisioni sono bloccate. |
| [GetDisplayZeros](./getdisplayzeros/) | True se i valori zero sono visualizzati. |
| [SetDisplayZeros](./setdisplayzeros/) | True se i valori zero sono visualizzati. |
| [GetDisplayRightToLeft](./getdisplayrighttoleft/) | Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra anziché da sinistra a destra. Il valore predefinito è false. |
| [SetDisplayRightToLeft](./setdisplayrighttoleft/) | Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra anziché da sinistra a destra. Il valore predefinito è false. |
| [IsOutlineShown](./isoutlineshown/) | Indica se mostrare la struttura. |
| [SetIsOutlineShown](./setisoutlineshown/) | Indica se mostrare la struttura. |
| [IsSelected](./isselected/) | Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta. |
| [SetIsSelected](./setisselected/) | Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta. |
| [FreezePanes_Int_Int_Int_Int](./freezepanes_int_int_int_int/) | Blocca i riquadri nella cella specificata del foglio di lavoro. |
| [GetFreezedPanes](./getfreezedpanes/) | Ottiene i riquadri bloccati. |
| [Split](./split/) | Dividi la finestra. |
| [FreezePanes_String_Int_Int](./freezepanes_string_int_int/) | Blocca i riquadri nella cella specificata del foglio di lavoro. |
| [UnFreezePanes](./unfreezepanes/) | Sblocca i riquadri nel foglio di lavoro. |
| [RemoveSplit](./removesplit/) | Rimuove la divisione della finestra. |
| [GetPivotTables](./getpivottables/) | Ottiene tutte le tabelle pivot in questo foglio di lavoro. |
| [GetListObjects](./getlistobjects/) | Ottiene tutti i ListObjects in questo foglio di lavoro. |
| [GetTabId](./gettabid/) | Specifica l'identificatore interno per il foglio. |
| [SetTabId](./settabid/) | Specifica l'identificatore interno per il foglio. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Ottiene la collezione HorizontalPageBreakCollection. |
| [GetVerticalPageBreaks](./getverticalpagebreaks/) | Ottiene la collezione VerticalPageBreakCollection. |
| [AddPageBreaks](./addpagebreaks/) | Aggiunge un'interruzione di pagina. |
| [GetHyperlinks](./gethyperlinks/) | Ottiene la collezione HyperlinkCollection. |
| [Copy_Worksheet](./copy_worksheet/) | Copia i contenuti e i formati da un altro foglio di lavoro. |
| [Copy_Worksheet_CopyOptions](./copy_worksheet_copyoptions/) | Copia i contenuti e i formati da un altro foglio di lavoro. |
| [AutoFitColumn_Int_Int_Int](./autofitcolumn_int_int_int/) | Adatta automaticamente la larghezza della colonna. |
| [AutoFitColumns](./autofitcolumns/) | Adatta automaticamente tutte le colonne in questo foglio di lavoro. |
| [AutoFitColumns_AutoFitterOptions](./autofitcolumns_autofitteroptions/) | Adatta automaticamente tutte le colonne in questo foglio di lavoro. |
| [AutoFitColumn_Int](./autofitcolumn_int/) | Adatta automaticamente la larghezza della colonna. |
| [AutoFitColumns_Int_Int](./autofitcolumns_int_int/) | Adatta automaticamente la larghezza delle colonne. |
| [AutoFitColumns_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_autofitteroptions/) | Adatta automaticamente la larghezza delle colonne. |
| [AutoFitColumns_Int_Int_Int_Int](./autofitcolumns_int_int_int_int/) | Adatta automaticamente la larghezza delle colonne. |
| [AutoFitColumns_Int_Int_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_int_int_autofitteroptions/) | Adatta automaticamente la larghezza delle colonne. |
| [AutoFitRow_Int_Int_Int](./autofitrow_int_int_int/) | Adatta automaticamente l'altezza della riga. |
| [AutoFitRow_Int_Int_Int_AutoFitterOptions](./autofitrow_int_int_int_autofitteroptions/) | Adatta automaticamente l'altezza della riga. |
| [AutoFitRows](./autofitrows/) | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [AutoFitRows_Bool](./autofitrows_bool/) | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [AutoFitRows_AutoFitterOptions](./autofitrows_autofitteroptions/) | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [AutoFitRows_Int_Int](./autofitrows_int_int/) | Adatta automaticamente l'altezza della riga in un intervallo. |
| [AutoFitRows_Int_Int_AutoFitterOptions](./autofitrows_int_int_autofitteroptions/) | Adatta automaticamente l'altezza della riga in un intervallo. |
| [AutoFitRow_Int_Int_Int_Int](./autofitrow_int_int_int_int/) | Adatta automaticamente l'altezza della riga in un intervallo rettangolare. |
| [AutoFitRow_Int](./autofitrow_int/) | Adatta automaticamente l'altezza della riga. |
| [GetPageSetup](./getpagesetup/) | Rappresenta la descrizione dell'impostazione pagina in questo foglio. |
| [GetAutoFilter](./getautofilter/) | Rappresenta il filtro automatico per il foglio di lavoro specificato. |
| [Filter](./filter/) | Filtra l'intervallo. |
| [GetAdvancedFilter](./getadvancedfilter/) | Ottiene le impostazioni del filtro avanzato. |
| [Advanced_Filter](./advanced_filter/) | Filtra i dati utilizzando criteri complessi. |
| [RemoveAutoFilter](./removeautofilter/) | Rimuove il filtro automatico del foglio di lavoro. |
| [GetHasAutofilter](./gethasautofilter/) | Indica se questo foglio di lavoro ha il filtro automatico. |
| [GetTransitionEvaluation](./gettransitionevaluation/) | Indica se l'opzione Valutazione della Formula di Transizione (compatibilità Lotus) è abilitata. |
| [SetTransitionEvaluation](./settransitionevaluation/) | Indica se l'opzione Valutazione della Formula di Transizione (compatibilità Lotus) è abilitata. |
| [GetTransitionEntry](./gettransitionentry/) | Indica se l'opzione Inserimento della Formula di Transizione (compatibilità Lotus) è abilitata. |
| [SetTransitionEntry](./settransitionentry/) | Indica se l'opzione Inserimento della Formula di Transizione (compatibilità Lotus) è abilitata. |
| [GetVisibilityType](./getvisibilitytype/) | Indica lo stato di visibilità per questo foglio. |
| [SetVisibilityType](./setvisibilitytype/) | Indica lo stato di visibilità per questo foglio. |
| [SetVisible](./setvisible/) | Imposta le opzioni di visibilità. |
| [IsVisible](./isvisible/) | Rappresenta se il foglio di lavoro è visibile. |
| [SetIsVisible](./setisvisible/) | Rappresenta se il foglio di lavoro è visibile. |
| [SelectRange](./selectrange/) | Seleziona un intervallo. |
| [RemoveAllDrawingObjects](./removealldrawingobjects/) | Rimuove tutti gli oggetti di disegno in questo foglio di lavoro. |
| [ClearComments](./clearcomments/) | Cancella tutti i commenti nel foglio di calcolo del designer. |
| [GetSparklineGroups](./getsparklinegroups/) | Ottiene i gruppi di sparkline nel foglio di lavoro. |
| [GetCharts](./getcharts/) | Ottiene una raccolta di grafici |
| [GetComments](./getcomments/) | Ottiene la raccolta di commenti. |
| [GetPictures](./getpictures/) | Ottiene una raccolta di immagini. |
| [GetAllPictures](./getallpictures/) | Ottiene tutte le immagini, incluse quelle incorporate nella cella e sopra le celle. |
| [GetTextBoxes](./gettextboxes/) | Ottiene una raccolta di caselle di testo. |
| [GetCheckBoxes](./getcheckboxes/) | Ottiene una raccolta di caselle di controllo. |
| [GetOleObjects](./getoleobjects/) | Rappresenta una raccolta di OleObject in un foglio di lavoro. |
| [GetShapes](./getshapes/) | Restituisce tutte le forme di disegno in questo foglio di lavoro. |
| [GetSlicers](./getslicers/) | Ottieni la raccolta di Slicer nel foglio di lavoro |
| [GetTimelines](./gettimelines/) | Ottieni la raccolta di Timeline nel foglio di lavoro |
| [Protect_ProtectionType](./protect_protectiontype/) | Protegge il foglio di lavoro. |
| [Protect_ProtectionType_String_String](./protect_protectiontype_string_string/) | Protegge il foglio di lavoro. |
| [Unprotect](./unprotect/) | Rimuove la protezione del foglio di lavoro. |
| [Unprotect_String](./unprotect_string/) | Rimuove la protezione del foglio di lavoro. |
| [GetIndex](./getindex/) | Ottiene l'indice del foglio nella raccolta di fogli di lavoro. |
| [MoveTo](./moveto/) | Sposta il foglio in un'altra posizione nel foglio di calcolo. |
| [IsProtected](./isprotected/) | Indica se il foglio di lavoro è protetto. |
| [GetValidations](./getvalidations/) | Ottiene la raccolta delle impostazioni di convalida dei dati nel foglio di lavoro. |
| [GetAllowEditRanges](./getalloweditranges/) | Ottiene la raccolta degli intervalli di modifica consentita nel foglio di lavoro. |
| [GetErrorCheckOptions](./geterrorcheckoptions/) | Ottiene le impostazioni di controllo errori applicate a determinati intervalli. |
| [GetOutline](./getoutline/) | Ottiene la struttura in questo foglio di lavoro. |
| [GetFirstVisibleRow](./getfirstvisiblerow/) | Rappresenta l'indice della prima riga visibile. |
| [SetFirstVisibleRow](./setfirstvisiblerow/) | Rappresenta l'indice della prima riga visibile. |
| [GetFirstVisibleColumn](./getfirstvisiblecolumn/) | Rappresenta l'indice della prima colonna visibile. |
| [SetFirstVisibleColumn](./setfirstvisiblecolumn/) | Rappresenta l'indice della prima colonna visibile. |
| [Replace](./replace/) | Sostituisce il testo di tutte le celle con una nuova stringa. |
| [GetZoom](./getzoom/) | Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400. |
| [SetZoom](./setzoom/) | Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400. |
| [GetViewType](./getviewtype/) | Ottiene e imposta il tipo di visualizzazione. |
| [SetViewType](./setviewtype/) | Ottiene e imposta il tipo di visualizzazione. |
| [IsPageBreakPreview](./ispagebreakpreview/) | Indica se il foglio di lavoro specificato è mostrato nella visualizzazione normale o nell'anteprima interruzioni di pagina. |
| [SetIsPageBreakPreview](./setispagebreakpreview/) | Indica se il foglio di lavoro specificato è mostrato nella visualizzazione normale o nell'anteprima interruzioni di pagina. |
| [IsRulerVisible](./isrulervisible/) | Indica se il righello è visibile. Questa proprietà è applicata solo per l'anteprima interruzioni di pagina. |
| [SetIsRulerVisible](./setisrulervisible/) | Indica se il righello è visibile. Questa proprietà è applicata solo per l'anteprima interruzioni di pagina. |
| [GetSelectedAreas](./getselectedareas/) | Ottiene gli intervalli di celle selezionati nel foglio di calcolo del designer. |
| [GetTabColor](./gettabcolor/) | Rappresenta il colore della scheda del foglio di lavoro. |
| [SetTabColor](./settabcolor/) | Rappresenta il colore della scheda del foglio di lavoro. |
| [GetGridlineColor](./getgridlinecolor/) | Ottiene e imposta il colore della griglia |
| [SetGridlineColor](./setgridlinecolor/) | Ottiene e imposta il colore della griglia |
| [GetCodeName](./getcodename/) | Ottiene il nome codice del foglio di lavoro. |
| [SetCodeName](./setcodename/) | Ottiene il nome codice del foglio di lavoro. |
| [GetBackgroundImage](./getbackgroundimage/) | Ottiene e imposta l'immagine di sfondo del foglio di lavoro. |
| [SetBackgroundImage](./setbackgroundimage/) | Ottiene e imposta l'immagine di sfondo del foglio di lavoro. |
| [GetConditionalFormattings](./getconditionalformattings/) | Ottiene i ConditionalFormattings nel foglio di lavoro. |
| [GetActiveCell](./getactivecell/) | Ottiene o imposta la cella attiva nel foglio di lavoro. |
| [SetActiveCell](./setactivecell/) | Ottiene o imposta la cella attiva nel foglio di lavoro. |
| [GetCustomProperties](./getcustomproperties/) | Ottiene un oggetto che rappresenta le informazioni di identificatore associate a un foglio di lavoro. |
| [GetPrintingPageBreaks](./getprintingpagebreaks/) | Ottiene le interruzioni di pagina automatiche. |
| [GetSmartTagSetting](./getsmarttagsetting/) | Ottiene tutti gli oggetti SmartTagCollection del foglio di lavoro. |
| [ToString](./tostring/) | Restituisce una stringa che rappresenta l'oggetto Worksheet corrente. |
| [GetScenarios](./getscenarios/) | Ottiene la collezione di Scenario. |
| [StartAccessCache](./startaccesscache/) | Avvia la sessione che utilizza le cache per accedere ai dati in questo foglio di lavoro. |
| [CloseAccessCache](./closeaccesscache/) | Chiude la sessione che utilizza le cache per accedere ai dati in questo foglio di lavoro. |
| [ConvertFormulaReferenceStyle](./convertformulareferencestyle/) | Converte lo stile di riferimento della formula. |
| [CalculateFormula_String](./calculateformula_string/) | Calcola una formula. |
| [CalculateFormula_String_CalculationOptions](./calculateformula_string_calculationoptions/) | Calcola direttamente un'espressione di formula. |
| [CalculateFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_CalculationData](./calculateformula_string_formulaparseoptions_calculationoptions_int_int_calculationdata/) | Calcola direttamente un'espressione di formula. |
| [CalculateArrayFormula_String_CalculationOptions](./calculatearrayformula_string_calculationoptions/) | Calcola una formula come formula di matrice. |
| [CalculateArrayFormula_String_CalculationOptions_Int_Int](./calculatearrayformula_string_calculationoptions_int_int/) | Calcola una formula come formula di matrice. |
| [CalculateArrayFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_Int_Int_CalculationData](./calculatearrayformula_string_formulaparseoptions_calculationoptions_int_int_int_int_calculationdata/) | Calcola una formula come formula di matrice. |
| [CalculateFormula_CalculationOptions_Bool](./calculateformula_calculationoptions_bool/) | Calcola tutte le formule in questo foglio di lavoro. |
| [GetAreasOfXmlMapQuery](./getareasofxmlmapquery/) | Interroga le aree di celle che sono mappate/collegate al percorso specifico della mappa xml. |
| [GetCellWatches](./getcellwatches/) | Ottiene la collezione di celle in questo foglio di lavoro monitorate nella 'finestra di osservazione'. |
| [RefreshPivotTables](./refreshpivottables/) | Aggiorna tutte le PivotTable in questo foglio di lavoro. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Aggiorna tutte le PivotTable in questo foglio di lavoro. |
