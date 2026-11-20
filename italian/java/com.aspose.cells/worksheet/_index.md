---
title: "Worksheet"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta un singolo foglio di lavoro."
type: docs
url: /it/java/com.aspose.cells/worksheet/
---

**Inheritance:**
java.lang.Object
```
public class Worksheet
```

Incapsula l'oggetto che rappresenta un singolo foglio di lavoro.

**Example**

Il seguente esempio mostra come bloccare i riquadri e inserire un collegamento ipertestuale al foglio di lavoro con .Net o VB.

```
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Freeze panes at "AS40" with 10 rows and 10 columns
         sheet.freezePanes("AS40", 10, 10);
 
         //Add a hyperlink in Cell A1
         sheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addPageBreaks(String cellName)](#addPageBreaks-java.lang.String-) | Aggiunge un'interruzione di pagina. |
| [advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)](#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-) | Filtra i dati usando criteri complessi. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Adatta automaticamente la larghezza della colonna. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Adatta automaticamente la larghezza della colonna. |
| [autoFitColumns()](#autoFitColumns--) | Adatta automaticamente tutte le colonne in questo foglio di lavoro. |
| [autoFitColumns(AutoFitterOptions options)](#autoFitColumns-com.aspose.cells.AutoFitterOptions-) | Adatta automaticamente tutte le colonne in questo foglio di lavoro. |
| [autoFitColumns(int firstColumn, int lastColumn)](#autoFitColumns-int-int-) | Adatta automaticamente la larghezza delle colonne. |
| [autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-) | Adatta automaticamente la larghezza delle colonne. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)](#autoFitColumns-int-int-int-int-) | Adatta automaticamente la larghezza delle colonne. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-) | Adatta automaticamente la larghezza delle colonne. |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Adatta automaticamente l'altezza della riga. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Adatta automaticamente l'altezza della riga. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-) | Adatta automaticamente l'altezza della riga. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Adatta automaticamente l'altezza della riga in un intervallo rettangolare. |
| [autoFitRows()](#autoFitRows--) | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [autoFitRows(AutoFitterOptions options)](#autoFitRows-com.aspose.cells.AutoFitterOptions-) | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Adatta automaticamente l'altezza della riga in un intervallo. |
| [autoFitRows(int startRow, int endRow, AutoFitterOptions options)](#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-) | Adatta automaticamente l'altezza della riga in un intervallo. |
| [calculateArrayFormula(String formula, CalculationOptions opts)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Calcola una formula come formula di matrice. |
| [calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-) | Calcola una formula come formula di matrice. |
| [calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)](#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-) | Calcola una formula come formula di matrice. |
| [calculateFormula(CalculationOptions options, boolean recursive)](#calculateFormula-com.aspose.cells.CalculationOptions-boolean-) | Calcola tutte le formule in questo foglio di lavoro. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Calcola una formula. |
| [calculateFormula(String formula, CalculationOptions opts)](#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Calcola direttamente un'espressione di formula. |
| [calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)](#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-) | Calcola direttamente un'espressione di formula. |
| [clearComments()](#clearComments--) | Cancella tutti i commenti nel foglio di calcolo del designer. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Chiude la sessione che utilizza cache per accedere ai dati in questo foglio di lavoro. |
| [convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)](#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-) | Converte lo stile di riferimento della formula. |
| [copy(Worksheet sourceSheet)](#copy-com.aspose.cells.Worksheet-) | Copia contenuti e formati da un altro foglio di lavoro. |
| [copy(Worksheet sourceSheet, CopyOptions copyOptions)](#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-) | Copia contenuti e formati da un altro foglio di lavoro. |
| [dispose()](#dispose--) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(CellArea ca)](#filter-com.aspose.cells.CellArea-) | Filtra l'intervallo. |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Blocca i riquadri nella cella specificata nel foglio di lavoro. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Blocca i riquadri nella cella specificata nel foglio di lavoro. |
| [getActiveCell()](#getActiveCell--) | Ottiene la cella attiva nel foglio di lavoro. |
| [getAdvancedFilter()](#getAdvancedFilter--) | Ottiene le impostazioni del filtro avanzato. |
| [getAllPictures()](#getAllPictures--) | Ottiene tutte le immagini, incluse quelle incorporate nella cella e sopra le celle. |
| [getAllowEditRanges()](#getAllowEditRanges--) | Ottiene la collezione di intervalli di modifica consentita nel foglio di lavoro. |
| [getAreasOfXmlMapQuery(String path, XmlMap xmlMap)](#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | Interroga le aree di celle mappate/collegate al percorso specifico della mappa XML. |
| [getAutoFilter()](#getAutoFilter--) | Rappresenta il filtro automatico per il foglio di lavoro specificato. |
| [getBackgroundImage()](#getBackgroundImage--) | Ottiene l'immagine di sfondo del foglio di lavoro. |
| [getCellWatches()](#getCellWatches--) | Ottiene la raccolta di celle in questo foglio di lavoro monitorata nella 'finestra di monitoraggio'. |
| [getCells()](#getCells--) | Ottiene la raccolta di [Cells](../../com.aspose.cells/cells). |
| [getCharts()](#getCharts--) | Ottiene una raccolta di [Chart](../../com.aspose.cells/chart) |
| [getCheckBoxes()](#getCheckBoxes--) | Ottiene una raccolta di [CheckBox](../../com.aspose.cells/checkbox). |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Ottiene il nome codice del foglio di lavoro. |
| [getComments()](#getComments--) | Ottiene la raccolta di [Comment](../../com.aspose.cells/comment). |
| [getConditionalFormattings()](#getConditionalFormattings--) | Ottiene i ConditionalFormattings nel foglio di lavoro. |
| [getCustomProperties()](#getCustomProperties--) | Ottiene un oggetto che rappresenta le informazioni di identificatore associate a un foglio di lavoro. |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra invece che da sinistra a destra. |
| [getDisplayZeros()](#getDisplayZeros--) | Vero se i valori zero sono visualizzati. |
| [getErrorCheckOptions()](#getErrorCheckOptions--) | Ottiene l'impostazione di controllo errori applicata a determinati intervalli. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | Rappresenta l'indice della prima colonna visibile. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | Rappresenta l'indice della prima riga visibile. |
| [getFreezedPanes()](#getFreezedPanes--) | Ottiene i riquadri di blocco. |
| [getGridlineColor()](#getGridlineColor--) | Ottiene il colore della griglia |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Ottiene la raccolta di [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection). |
| [getHyperlinks()](#getHyperlinks--) | Ottiene la raccolta di [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection). |
| [getIndex()](#getIndex--) | Ottiene l'indice del foglio nella raccolta di fogli di lavoro. |
| [getListObjects()](#getListObjects--) | Ottiene tutti i ListObjects in questo foglio di lavoro. |
| [getName()](#getName--) | Ottiene il nome del foglio di lavoro. |
| [getOleObjects()](#getOleObjects--) | Rappresenta una raccolta di [OleObject](../../com.aspose.cells/oleobject) in un foglio di lavoro. |
| [getOutline()](#getOutline--) | Ottiene la struttura in questo foglio di lavoro. |
| [getPageSetup()](#getPageSetup--) | Rappresenta la descrizione della configurazione di pagina in questo foglio. |
| [getPaneState()](#getPaneState--) | Indica se il riquadro ha divisioni orizzontali o verticali e se tali divisioni sono bloccate. |
| [getPanes()](#getPanes--) | Ottiene i riquadri della finestra. |
| [getPictures()](#getPictures--) | Ottiene una collezione di [Picture](../../com.aspose.cells/picture). |
| [getPivotTables()](#getPivotTables--) | Ottiene tutte le tabelle pivot in questo foglio di lavoro. |
| [getPrintingPageBreaks(ImageOrPrintOptions options)](#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-) | Ottiene le interruzioni di pagina automatiche. |
| [getProtection()](#getProtection--) | Rappresenta i vari tipi di opzioni di protezione disponibili per un foglio di lavoro. |
| [getQueryTables()](#getQueryTables--) | Ottiene [QueryTableCollection](../../com.aspose.cells/querytablecollection) nel foglio di lavoro. |
| [getScenarios()](#getScenarios--) | Ottiene la collezione di [Scenario](../../com.aspose.cells/scenario). |
| [getSelectedAreas()](#getSelectedAreas--) | Ottiene gli intervalli di celle selezionati nel foglio di calcolo del designer. |
| [getSelectedRanges()](#getSelectedRanges--) | Ottiene gli intervalli di celle selezionati nel foglio di calcolo del designer. |
| [getShapes()](#getShapes--) | Restituisce tutte le forme di disegno in questo foglio di lavoro. |
| [getShowDataTypeIcons()](#getShowDataTypeIcons--) | Indica se mostrare le icone del tipo di dati. |
| [getShowFormulas()](#getShowFormulas--) | Indica se mostrare le formule o i loro risultati. |
| [getSlicers()](#getSlicers--) | Ottieni la collezione di Slicer nel foglio di lavoro |
| [getSmartTagSetting()](#getSmartTagSetting--) | Ottiene tutti gli oggetti [SmartTagCollection](../../com.aspose.cells/smarttagcollection) del foglio di lavoro. |
| [getSparklineGroups()](#getSparklineGroups--) | Ottiene i gruppi di sparkline nel foglio di lavoro. |
| [getTabColor()](#getTabColor--) | Rappresenta il colore della scheda del foglio di lavoro. |
| [getTabId()](#getTabId--) | Specifica l'identificatore interno per il foglio. |
| [getTextBoxes()](#getTextBoxes--) | Ottiene una collezione di [TextBox](../../com.aspose.cells/textbox). |
| [getTimelines()](#getTimelines--) | Ottieni la collezione di Timeline nel foglio di lavoro |
| [getTransitionEntry()](#getTransitionEntry--) | Indica se l'opzione Transition Formula Entry (compatibilità Lotus) è abilitata. |
| [getTransitionEvaluation()](#getTransitionEvaluation--) | Indica se l'opzione Transition Formula Evaluation (compatibilità Lotus) è abilitata. |
| [getType()](#getType--) | Rappresenta il tipo di foglio di lavoro. |
| [getUniqueId()](#getUniqueId--) | Ottiene l'ID univoco, è lo stesso di \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [getValidations()](#getValidations--) | Ottiene la collezione delle impostazioni di convalida dei dati nel foglio di lavoro. |
| [getVerticalPageBreaks()](#getVerticalPageBreaks--) | Ottiene la collezione di [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection). |
| [getViewType()](#getViewType--) | Ottiene il tipo di visualizzazione. |
| [getVisibilityType()](#getVisibilityType--) | Indica lo stato di visibilità per questo foglio. |
| [getWorkbook()](#getWorkbook--) | Ottiene l'oggetto workbook che contiene questo foglio. |
| [getZoom()](#getZoom--) | Rappresenta il fattore di scala in percentuale. |
| [hasAutofilter()](#hasAutofilter--) | Indica se questo foglio di lavoro ha il filtro automatico. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Ottiene un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true. |
| [isOutlineShown()](#isOutlineShown--) | Indica se mostrare la struttura. |
| [isPageBreakPreview()](#isPageBreakPreview--) | Indica se il foglio di lavoro specificato è mostrato in visualizzazione normale o anteprima interruzione di pagina. |
| [isProtected()](#isProtected--) | Indica se il foglio di lavoro è protetto. |
| [isRowColumnHeadersVisible()](#isRowColumnHeadersVisible--) | Ottiene un valore che indica se il foglio di lavoro visualizzerà le intestazioni di righe e colonne. |
| [isRulerVisible()](#isRulerVisible--) | Indica se il righello è visibile. |
| [isSelected()](#isSelected--) | Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta. |
| [isVisible()](#isVisible--) | Rappresenta se il foglio di lavoro è visibile. |
| [moveTo(int index)](#moveTo-int-) | Sposta il foglio in un'altra posizione nel foglio di calcolo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(int type)](#protect-int-) | Protegge il foglio di lavoro. |
| [protect(int type, String password, String oldPassword)](#protect-int-java.lang.String-java.lang.String-) | Protegge il foglio di lavoro. |
| [refreshPivotTables()](#refreshPivotTables--) | Aggiorna tutte le PivotTable in questo foglio di lavoro. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Aggiorna tutte le PivotTable in questo foglio di lavoro. |
| [removeAllDrawingObjects()](#removeAllDrawingObjects--) | Rimuove tutti gli oggetti di disegno in questo foglio di lavoro. |
| [removeAutoFilter()](#removeAutoFilter--) | Rimuove il filtro automatico del foglio di lavoro. |
| [removeSplit()](#removeSplit--) | Rimuove la divisione della finestra. |
| [replace(String oldString, String newString)](#replace-java.lang.String-java.lang.String-) | Sostituisce il testo di tutte le celle con una nuova stringa. |
| [selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)](#selectRange-int-int-int-int-boolean-) | Seleziona un intervallo. |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Imposta la cella attiva nel foglio di lavoro. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Imposta l'immagine di sfondo del foglio di lavoro. |
| [setCodeName(String value)](#setCodeName-java.lang.String-) | Ottiene il nome codice del foglio di lavoro. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra invece che da sinistra a destra. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | Vero se i valori zero sono visualizzati. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | Rappresenta l'indice della prima colonna visibile. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | Rappresenta l'indice della prima riga visibile. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Imposta il colore della linea della griglia |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Imposta un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome del foglio di lavoro. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Indica se mostrare la struttura. |
| [setPageBreakPreview(boolean value)](#setPageBreakPreview-boolean-) | Indica se il foglio di lavoro specificato è mostrato in visualizzazione normale o anteprima interruzione di pagina. |
| [setRowColumnHeadersVisible(boolean value)](#setRowColumnHeadersVisible-boolean-) | Imposta un valore che indica se il foglio di lavoro visualizzerà le intestazioni di righe e colonne. |
| [setRulerVisible(boolean value)](#setRulerVisible-boolean-) | Indica se il righello è visibile. |
| [setSelected(boolean value)](#setSelected-boolean-) | Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta. |
| [setShowDataTypeIcons(boolean value)](#setShowDataTypeIcons-boolean-) | Indica se mostrare le icone del tipo di dati. |
| [setShowFormulas(boolean value)](#setShowFormulas-boolean-) | Indica se mostrare le formule o i loro risultati. |
| [setTabColor(Color value)](#setTabColor-com.aspose.cells.Color-) | Rappresenta il colore della scheda del foglio di lavoro. |
| [setTabId(int value)](#setTabId-int-) | Specifica l'identificatore interno per il foglio. |
| [setTransitionEntry(boolean value)](#setTransitionEntry-boolean-) | Indica se l'opzione Transition Formula Entry (compatibilità Lotus) è abilitata. |
| [setTransitionEvaluation(boolean value)](#setTransitionEvaluation-boolean-) | Indica se l'opzione Transition Formula Evaluation (compatibilità Lotus) è abilitata. |
| [setType(int value)](#setType-int-) | Rappresenta il tipo di foglio di lavoro. |
| [setUniqueId(String value)](#setUniqueId-java.lang.String-) | Imposta l'ID univoco, è lo stesso di \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}. |
| [setViewType(int value)](#setViewType-int-) | Imposta il tipo di visualizzazione. |
| [setVisibilityType(int value)](#setVisibilityType-int-) | Indica lo stato di visibilità per questo foglio. |
| [setVisible(boolean value)](#setVisible-boolean-) | Rappresenta se il foglio di lavoro è visibile. |
| [setVisible(boolean isVisible, boolean ignoreError)](#setVisible-boolean-boolean-) | Imposta le opzioni visibili. |
| [setZoom(int value)](#setZoom-int-) | Rappresenta il fattore di scala in percentuale. |
| [split()](#split--) | Dividi la finestra. |
| [startAccessCache(int opts)](#startAccessCache-int-) | Avvia la sessione che utilizza le cache per accedere ai dati in questo foglio di lavoro. |
| [toString()](#toString--) | Restituisce una stringa che rappresenta l'oggetto Worksheet corrente. |
| [unFreezePanes()](#unFreezePanes--) | Sblocca i riquadri nel foglio di lavoro. |
| [unprotect()](#unprotect--) | Rimuove la protezione dal foglio di lavoro. |
| [unprotect(String password)](#unprotect-java.lang.String-) | Rimuove la protezione dal foglio di lavoro. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [xmlMapQuery(String path, XmlMap xmlMap)](#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | Interroga le aree di celle mappate/collegate al percorso specifico della mappa XML. |
### addPageBreaks(String cellName) {#addPageBreaks-java.lang.String-}
```
public void addPageBreaks(String cellName)
```


Aggiunge un'interruzione di pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String |  |

### advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly) {#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public void advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)
```


Filtra i dati usando criteri complessi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isFilter | boolean | Indica se filtrare l'elenco in loco. |
| listRange | java.lang.String | L'intervallo dell'elenco. |
| criteriaRange | java.lang.String | L'intervallo dei criteri. |
| copyTo | java.lang.String | L'intervallo dove copiare i dati. |
| uniqueRecordOnly | boolean | Solo visualizzare o copiare righe uniche. |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Adatta automaticamente la larghezza della colonna.

**Remarks**

AutoFitColumn è una funzione imprecisa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


Adatta automaticamente la larghezza della colonna.

**Remarks**

Questo metodo adatta automaticamente una riga in base al contenuto di un intervallo di celle nella riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |
| firstRow | int | Indice della prima riga. |
| lastRow | int | Indice dell'ultima riga. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```


Adatta automaticamente tutte le colonne in questo foglio di lavoro.

### autoFitColumns(AutoFitterOptions options) {#autoFitColumns-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(AutoFitterOptions options)
```


Adatta automaticamente tutte le colonne in questo foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Le opzioni di adattamento automatico |

### autoFitColumns(int firstColumn, int lastColumn) {#autoFitColumns-int-int-}
```
public void autoFitColumns(int firstColumn, int lastColumn)
```


Adatta automaticamente la larghezza delle colonne.

**Remarks**

AutoFitColumn è una funzione imprecisa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstColumn | int | Indice della prima colonna. |
| lastColumn | int | Indice dell'ultima colonna. |

### autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```


Adatta automaticamente la larghezza delle colonne.

**Remarks**

AutoFitColumn è una funzione imprecisa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstColumn | int | Indice della prima colonna. |
| lastColumn | int | Indice dell'ultima colonna. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Le opzioni di adattamento automatico |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn) {#autoFitColumns-int-int-int-int-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```


Adatta automaticamente la larghezza delle colonne.

**Remarks**

AutoFitColumn è una funzione imprecisa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Indice della prima riga. |
| firstColumn | int | Indice della prima colonna. |
| lastRow | int | Indice dell'ultima riga. |
| lastColumn | int | Indice dell'ultima colonna. |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)
```


Adatta automaticamente la larghezza delle colonne.

**Remarks**

AutoFitColumn è una funzione imprecisa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | int | Indice della prima riga. |
| firstColumn | int | Indice della prima colonna. |
| lastRow | int | Indice dell'ultima riga. |
| lastColumn | int | Indice dell'ultima colonna. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Le opzioni di adattamento automatico |

### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


Adatta automaticamente l'altezza della riga.

**Remarks**

AutoFitRow è una funzione imprecisa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


Adatta automaticamente l'altezza della riga.

**Remarks**

Questo metodo adatta automaticamente una riga in base al contenuto di un intervallo di celle nella riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |
| firstColumn | int | Indice della prima colonna. |
| lastColumn | int | Indice dell'ultima colonna. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```


Adatta automaticamente l'altezza della riga.

**Remarks**

Questo metodo adatta automaticamente una riga in base al contenuto di un intervallo di celle nella riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |
| firstColumn | int | Indice della prima colonna. |
| lastColumn | int | Indice dell'ultima colonna. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Le opzioni del ridimensionatore automatico |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


Adatta automaticamente l'altezza della riga in un intervallo rettangolare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| endRow | int | Indice della riga finale. |
| startColumn | int | Indice della colonna di inizio. |
| endColumn | int | Indice della colonna finale. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


Adatta automaticamente tutte le righe in questo foglio di lavoro.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


Adatta automaticamente tutte le righe in questo foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| onlyAuto | boolean | True, ridimensiona automaticamente l'altezza della riga solo quando l'altezza della riga non è personalizzata. |

### autoFitRows(AutoFitterOptions options) {#autoFitRows-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(AutoFitterOptions options)
```


Adatta automaticamente tutte le righe in questo foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Le opzioni del ridimensionatore automatico |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


Adatta automaticamente l'altezza della riga in un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| endRow | int | Indice della riga finale. |

### autoFitRows(int startRow, int endRow, AutoFitterOptions options) {#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(int startRow, int endRow, AutoFitterOptions options)
```


Adatta automaticamente l'altezza della riga in un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| endRow | int | Indice della riga finale. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Le opzioni del ridimensionatore automatico. |

### calculateArrayFormula(String formula, CalculationOptions opts) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts)
```


Calcola una formula come formula di matrice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | Formula da calcolare. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opzioni per calcolare la formula |

**Returns:**
java.lang.Object[][]
### calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)
```


Calcola una formula come formula di matrice.

**Remarks**

La formula sarà considerata come formula di array dinamico per calcolare la dimensione e il risultato. La dimensione massima specificata dall'utente viene utilizzata nei casi in cui il risultato calcolato è un grande set di dati (ad esempio, il risultato calcolato può corrispondere a un'intera riga o colonna di dati) ma l'utente non necessita di un array così grande secondo i requisiti di business o per considerazioni di prestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | Formula da calcolare. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opzioni per calcolare la formula |
| maxRowCount | int | il conteggio massimo di righe dei dati risultanti. Se è non positivo o maggiore del conteggio reale di righe, verrà utilizzato il conteggio reale di righe. |
| maxColumnCount | int | il conteggio massimo di colonne dei dati risultanti. Se è non positivo o maggiore del conteggio reale di righe, verrà utilizzato il conteggio reale di colonne. |

**Returns:**
java.lang.Object[][] - Risultato della formula calcolata.
### calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData) {#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-}
```
public Object[][] calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)
```


Calcola una formula come formula di matrice.

**Remarks**

La formula sarà considerata come formula di array dinamico per calcolare la dimensione e il risultato. La dimensione massima specificata dall'utente viene utilizzata nei casi in cui il risultato calcolato è un grande set di dati (ad esempio, il risultato calcolato può corrispondere a un'intera riga o colonna di dati) ma l'utente non necessita di un array così grande secondo i requisiti di business o per considerazioni di prestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | Formula da calcolare. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opzioni per l'analisi della formula |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opzioni per calcolare la formula |
| baseCellRow | int | L'indice della riga della cella base. |
| baseCellColumn | int | L'indice della colonna della cella base. |
| maxRowCount | int | Il conteggio massimo di righe dei dati risultanti. Se è non positivo o maggiore del conteggio reale di righe, verrà utilizzato il conteggio reale di righe. |
| maxColumnCount | int | Il numero massimo di colonne dei dati risultanti. Se è non positivo o maggiore del conteggio reale delle righe, verrà usato il conteggio reale delle colonne. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | I dati di calcolo. Sono usati per la situazione in cui l'utente deve calcolare alcune formule statiche durante l'implementazione di un motore di calcolo personalizzato. Per questo tipo di situazione, l'utente deve specificarli con i dati di calcolo forniti per [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-). |

**Returns:**
java.lang.Object[][] - Risultato della formula calcolata.
### calculateFormula(CalculationOptions options, boolean recursive) {#calculateFormula-com.aspose.cells.CalculationOptions-boolean-}
```
public void calculateFormula(CalculationOptions options, boolean recursive)
```


Calcola tutte le formule in questo foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opzioni per il calcolo |
| recursive | boolean | True indica che se le celle del foglio di lavoro dipendono dalle celle di altri fogli, le celle dipendenti negli altri fogli saranno calcolate anch'esse. False indica che tutte le formule nel foglio di lavoro sono state calcolate e i valori sono corretti. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Calcola una formula.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | Formula da calcolare. |

**Returns:**
java.lang.Object - Risultato della formula calcolata.
### calculateFormula(String formula, CalculationOptions opts) {#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object calculateFormula(String formula, CalculationOptions opts)
```


Calcola direttamente un'espressione di formula.

**Remarks**

La formula sarà calcolata proprio come se fosse impostata nella cella A1. E la formula sarà trattata come formula normale. Se è necessario calcolare la formula come formula array e ottenere un array per il risultato calcolato, utilizzare invece [calculateArrayFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-CalculationOptions-).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | Formula da calcolare. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opzioni per calcolare la formula |

**Returns:**
java.lang.Object - Risultato calcolato della formula fornita. L'oggetto restituito può essere di tipi possibili come [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), o ReferredArea.
### calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData) {#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-}
```
public Object calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)
```


Calcola direttamente un'espressione di formula.

**Remarks**

La formula sarà calcolata proprio come se fosse impostata nella cella base specificata. E la formula sarà trattata come formula normale. Se è necessario calcolare la formula come formula array e ottenere un array per il risultato calcolato, utilizzare invece [calculateArrayFormula(String,FormulaParseOptions,CalculationOptions,int,int,int,int,CalculationData)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-FormulaParseOptions-CalculationOptions-int-int-int-int-CalculationData-).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | Formula da calcolare. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opzioni per l'analisi della formula. |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opzioni per il calcolo della formula. |
| baseCellRow | int | L'indice della riga della cella base. |
| baseCellColumn | int | L'indice della colonna della cella base. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | I dati di calcolo. Sono usati per la situazione in cui l'utente deve calcolare alcune formule statiche durante l'implementazione di un motore di calcolo personalizzato. Per questo tipo di situazione, l'utente deve specificarli con i dati di calcolo forniti per [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-). |

**Returns:**
java.lang.Object - Risultato calcolato della formula fornita. L'oggetto restituito può essere di tipi possibili come [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), o ReferredArea.
### clearComments() {#clearComments--}
```
public void clearComments()
```


Cancella tutti i commenti nel foglio di calcolo del designer.

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Chiude la sessione che utilizza cache per accedere ai dati in questo foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). opzioni di accesso ai dati |

### convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn) {#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-}
```
public String convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)
```


Converte lo stile di riferimento della formula.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | La formula da convertire. |
| toR1C1 | boolean | Quale stile di riferimento utilizzare per convertire la formula. Se la formula originale è nello stile di riferimento A1, questo valore deve essere true affinché la formula venga convertita dallo stile A1 a R1C1; se la formula originale è nello stile di riferimento R1C1, questo valore deve essere false affinché la formula venga convertita dallo stile R1C1 a A1; |
| baseCellRow | int | L'indice della riga della cella base. |
| baseCellColumn | int | L'indice della colonna della cella base. |

**Returns:**
java.lang.String - La formula convertita.
### copy(Worksheet sourceSheet) {#copy-com.aspose.cells.Worksheet-}
```
public void copy(Worksheet sourceSheet)
```


Copia contenuti e formati da un altro foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Foglio di lavoro di origine. |

### copy(Worksheet sourceSheet, CopyOptions copyOptions) {#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-}
```
public void copy(Worksheet sourceSheet, CopyOptions copyOptions)
```


Copia contenuti e formati da un altro foglio di lavoro.

**Remarks**

È possibile copiare i dati da un altro foglio di lavoro nello stesso file o in un altro file. Tuttavia, questo metodo non supporta la copia di oggetti grafici, come commenti, immagini e grafici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Foglio di lavoro di origine. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) |  |

### dispose() {#dispose--}
```
public void dispose()
```


Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### filter(CellArea ca) {#filter-com.aspose.cells.CellArea-}
```
public void filter(CellArea ca)
```


Filtra l'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | L'intervallo |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Blocca i riquadri nella cella specificata nel foglio di lavoro.

**Remarks**

L'indice di riga e l'indice di colonna non possono entrambi essere zero. Anche il numero di righe e il numero di colonne non possono entrambi essere zero.

I primi due parametri specificano la posizione congelata e gli ultimi due parametri specificano l'area congelata nel pannello superiore sinistro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| colonna | int | Indice di colonna. |
| freezedRows | int | Numero di righe visibili nel pannello superiore, non superiore all'indice di riga. |
| freezedColumns | int | Numero di colonne visibili nel pannello sinistro, non superiore all'indice di colonna. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


Blocca i riquadri nella cella specificata nel foglio di lavoro.

**Remarks**

L'indice di riga e l'indice di colonna non possono entrambi essere zero. Anche il numero di righe e il numero di colonne non possono entrambi essere zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Nome della cella. |
| freezedRows | int | Numero di righe visibili nel pannello superiore, non superiore all'indice di riga. |
| freezedColumns | int | Numero di colonne visibili nel pannello sinistro, non superiore all'indice di colonna. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


Ottiene la cella attiva nel foglio di lavoro.

**Returns:**
java.lang.String
### getAdvancedFilter() {#getAdvancedFilter--}
```
public AdvancedFilter getAdvancedFilter()
```


Ottiene le impostazioni del filtro avanzato.

**Returns:**
[AdvancedFilter](../../com.aspose.cells/advancedfilter) - 
### getAllPictures() {#getAllPictures--}
```
public Picture[] getAllPictures()
```


Ottiene tutte le immagini, incluse quelle incorporate nella cella e sopra le celle.

**Returns:**
com.aspose.cells.Picture[] -
### getAllowEditRanges() {#getAllowEditRanges--}
```
public ProtectedRangeCollection getAllowEditRanges()
```


Ottiene la collezione di intervalli di modifica consentita nel foglio di lavoro.

**Returns:**
[ProtectedRangeCollection](../../com.aspose.cells/protectedrangecollection)
### getAreasOfXmlMapQuery(String path, XmlMap xmlMap) {#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public CellArea[] getAreasOfXmlMapQuery(String path, XmlMap xmlMap)
```


Interroga le aree di celle mappate/collegate al percorso specifico della mappa XML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | java.lang.String | percorso dell'elemento xml |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Specificare una mappa xml se si desidera interrogare il percorso specifico all'interno di una mappa specifica |

**Returns:**
com.aspose.cells.CellArea[] - elenco di [CellArea](../../com.aspose.cells/cellarea) che è stato mappato/collegato al percorso specifico della mappa xml, viene restituito un elenco vuoto se nulla è stato mappato/collegato.
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Rappresenta il filtro automatico per il foglio di lavoro specificato.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Ottiene l'immagine di sfondo del foglio di lavoro.

**Returns:**
byte[]
### getCellWatches() {#getCellWatches--}
```
public CellWatchCollection getCellWatches()
```


Ottiene la raccolta di celle in questo foglio di lavoro monitorata nella 'finestra di monitoraggio'.

**Returns:**
[CellWatchCollection](../../com.aspose.cells/cellwatchcollection)
### getCells() {#getCells--}
```
public Cells getCells()
```


Ottiene la raccolta di [Cells](../../com.aspose.cells/cells).

**Returns:**
[Cells](../../com.aspose.cells/cells)
### getCharts() {#getCharts--}
```
public ChartCollection getCharts()
```


Ottiene una raccolta di [Chart](../../com.aspose.cells/chart)

**Returns:**
[ChartCollection](../../com.aspose.cells/chartcollection)
### getCheckBoxes() {#getCheckBoxes--}
```
public CheckBoxCollection getCheckBoxes()
```


Ottiene una raccolta di [CheckBox](../../com.aspose.cells/checkbox).

**Returns:**
[CheckBoxCollection](../../com.aspose.cells/checkboxcollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


Ottiene il nome codice del foglio di lavoro.

**Returns:**
java.lang.String
### getComments() {#getComments--}
```
public CommentCollection getComments()
```


Ottiene la raccolta di [Comment](../../com.aspose.cells/comment).

**Returns:**
[CommentCollection](../../com.aspose.cells/commentcollection)
### getConditionalFormattings() {#getConditionalFormattings--}
```
public ConditionalFormattingCollection getConditionalFormattings()
```


Ottiene i ConditionalFormattings nel foglio di lavoro.

**Returns:**
[ConditionalFormattingCollection](../../com.aspose.cells/conditionalformattingcollection)
### getCustomProperties() {#getCustomProperties--}
```
public CustomPropertyCollection getCustomProperties()
```


Ottiene un oggetto che rappresenta le informazioni di identificatore associate a un foglio di lavoro.

**Remarks**

Worksheet.CustomProperties fornisce un meccanismo preferito per memorizzare dati arbitrari. Supporta componenti di documenti di terze parti legacy, così come quelle situazioni che hanno una necessità stringente di parti binarie.

**Returns:**
[CustomPropertyCollection](../../com.aspose.cells/custompropertycollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra invece che da sinistra a destra. Il valore predefinito è false.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


Vero se i valori zero sono visualizzati.

**Returns:**
boolean
### getErrorCheckOptions() {#getErrorCheckOptions--}
```
public ErrorCheckOptionCollection getErrorCheckOptions()
```


Ottiene l'impostazione di controllo errori applicata a determinati intervalli.

**Returns:**
[ErrorCheckOptionCollection](../../com.aspose.cells/errorcheckoptioncollection)
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


Rappresenta l'indice della prima colonna visibile.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


Rappresenta l'indice della prima riga visibile.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


Ottiene i riquadri di blocco.

**Returns:**
int[] - Restituire null significa che il foglio di lavoro non è bloccato 0:indice riga;1:colonna;2:righe bloccate;3:righe bloccate
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Ottiene il colore della griglia

**Returns:**
[Color](../../com.aspose.cells/color)
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public HorizontalPageBreakCollection getHorizontalPageBreaks()
```


Ottiene la raccolta di [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection).

**Returns:**
[HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)
### getHyperlinks() {#getHyperlinks--}
```
public HyperlinkCollection getHyperlinks()
```


Ottiene la raccolta di [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection).

**Returns:**
[HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Ottiene l'indice del foglio nella raccolta di fogli di lavoro.

**Returns:**
int
### getListObjects() {#getListObjects--}
```
public ListObjectCollection getListObjects()
```


Ottiene tutti i ListObjects in questo foglio di lavoro.

**Returns:**
[ListObjectCollection](../../com.aspose.cells/listobjectcollection)
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome del foglio di lavoro.

**Remarks**

La lunghezza massima del nome del foglio è 31. E non è possibile assegnare lo stesso nome (senza distinzione tra maiuscole e minuscole) a due fogli di lavoro. Ad esempio, non è possibile impostare "SheetName1" al primo foglio e impostare "SHEETNAME1" al secondo foglio.

**Returns:**
java.lang.String
### getOleObjects() {#getOleObjects--}
```
public OleObjectCollection getOleObjects()
```


Rappresenta una raccolta di [OleObject](../../com.aspose.cells/oleobject) in un foglio di lavoro.

**Returns:**
[OleObjectCollection](../../com.aspose.cells/oleobjectcollection)
### getOutline() {#getOutline--}
```
public Outline getOutline()
```


Ottiene la struttura in questo foglio di lavoro.

**Returns:**
[Outline](../../com.aspose.cells/outline)
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Rappresenta la descrizione della configurazione di pagina in questo foglio.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPaneState() {#getPaneState--}
```
public int getPaneState()
```


Indica se il riquadro ha divisioni orizzontali o verticali e se tali divisioni sono bloccate.

Vedi [PaneStateType](../../com.aspose.cells/panestatetype).

**Returns:**
int
### getPanes() {#getPanes--}
```
public PaneCollection getPanes()
```


Ottiene i riquadri della finestra.

**Remarks**

Se la finestra non è divisa o bloccata.

**Returns:**
[PaneCollection](../../com.aspose.cells/panecollection)
### getPictures() {#getPictures--}
```
public PictureCollection getPictures()
```


Ottiene una collezione di [Picture](../../com.aspose.cells/picture).

**Returns:**
[PictureCollection](../../com.aspose.cells/picturecollection)
### getPivotTables() {#getPivotTables--}
```
public PivotTableCollection getPivotTables()
```


Ottiene tutte le tabelle pivot in questo foglio di lavoro.

**Returns:**
[PivotTableCollection](../../com.aspose.cells/pivottablecollection)
### getPrintingPageBreaks(ImageOrPrintOptions options) {#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-}
```
public CellArea[] getPrintingPageBreaks(ImageOrPrintOptions options)
```


Ottiene le interruzioni di pagina automatiche.

**Remarks**

Ogni area di cella rappresenta un foglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Le opzioni di stampa |

**Returns:**
com.aspose.cells.CellArea[] - Le aree di interruzioni di pagina automatiche.
### getProtection() {#getProtection--}
```
public Protection getProtection()
```


Rappresenta i vari tipi di opzioni di protezione disponibili per un foglio di lavoro. Supporta opzioni di protezione avanzate in ExcelXP e versioni successive.

**Remarks**

Questa proprietà può proteggere il foglio di lavoro in tutte le versioni del file Excel e supporta opzioni di protezione avanzate in ExcelXP e versioni successive.

**Returns:**
[Protection](../../com.aspose.cells/protection)
### getQueryTables() {#getQueryTables--}
```
public QueryTableCollection getQueryTables()
```


Ottiene [QueryTableCollection](../../com.aspose.cells/querytablecollection) nel foglio di lavoro.

**Returns:**
[QueryTableCollection](../../com.aspose.cells/querytablecollection)
### getScenarios() {#getScenarios--}
```
public ScenarioCollection getScenarios()
```


Ottiene la collezione di [Scenario](../../com.aspose.cells/scenario).

**Returns:**
[ScenarioCollection](../../com.aspose.cells/scenariocollection)
### getSelectedAreas() {#getSelectedAreas--}
```
public Range[] getSelectedAreas()
```


Ottiene gli intervalli di celle selezionati nel foglio di calcolo del designer.

**Returns:**
com.aspose.cells.Range[] - Restituisce tutti gli intervalli selezionati.
### getSelectedRanges() {#getSelectedRanges--}
```
public ArrayList getSelectedRanges()
```


Ottiene gli intervalli di celle selezionati nel foglio di calcolo del designer.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Worksheet.GetSelectedAreas(). Questa proprietà sarà rimossa 12 mesi dopo da marzo 2025. Aspose si scusa per qualsiasi inconveniente possa aver subito.

**Returns:**
java.util.ArrayList - Un ArrayList che contiene gli intervalli selezionati.
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Restituisce tutte le forme di disegno in questo foglio di lavoro.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTypeIcons() {#getShowDataTypeIcons--}
```
public boolean getShowDataTypeIcons()
```


Indica se mostrare le icone del tipo di dati.

**Returns:**
boolean
### getShowFormulas() {#getShowFormulas--}
```
public boolean getShowFormulas()
```


Indica se mostrare le formule o i loro risultati.

**Returns:**
boolean
### getSlicers() {#getSlicers--}
```
public SlicerCollection getSlicers()
```


Ottieni la collezione di Slicer nel foglio di lavoro

**Returns:**
[SlicerCollection](../../com.aspose.cells/slicercollection)
### getSmartTagSetting() {#getSmartTagSetting--}
```
public SmartTagSetting getSmartTagSetting()
```


Ottiene tutti gli oggetti [SmartTagCollection](../../com.aspose.cells/smarttagcollection) del foglio di lavoro.

**Returns:**
[SmartTagSetting](../../com.aspose.cells/smarttagsetting)
### getSparklineGroups() {#getSparklineGroups--}
```
public SparklineGroupCollection getSparklineGroups()
```


Ottiene i gruppi di sparkline nel foglio di lavoro.

**Returns:**
[SparklineGroupCollection](../../com.aspose.cells/sparklinegroupcollection)
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Rappresenta il colore della scheda del foglio di lavoro.

**Remarks**

Questa funzionalità è supportata solo in ExcelXP (Excel2002) e versioni successive. Se si salva il file in formato Excel97 o Excel2000, verrà omessa.

**Returns:**
[Color](../../com.aspose.cells/color)
### getTabId() {#getTabId--}
```
public int getTabId()
```


Specifica l'identificatore interno per il foglio.

**Returns:**
int
### getTextBoxes() {#getTextBoxes--}
```
public TextBoxCollection getTextBoxes()
```


Ottiene una collezione di [TextBox](../../com.aspose.cells/textbox).

**Returns:**
[TextBoxCollection](../../com.aspose.cells/textboxcollection)
### getTimelines() {#getTimelines--}
```
public TimelineCollection getTimelines()
```


Ottieni la collezione di Timeline nel foglio di lavoro

**Returns:**
[TimelineCollection](../../com.aspose.cells/timelinecollection)
### getTransitionEntry() {#getTransitionEntry--}
```
public boolean getTransitionEntry()
```


Indica se l'opzione Transition Formula Entry (compatibilità Lotus) è abilitata.

**Returns:**
boolean
### getTransitionEvaluation() {#getTransitionEvaluation--}
```
public boolean getTransitionEvaluation()
```


Indica se l'opzione Transition Formula Evaluation (compatibilità Lotus) è abilitata.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Rappresenta il tipo di foglio di lavoro.

Vedi [SheetType](../../com.aspose.cells/sheettype).

**Returns:**
int
### getUniqueId() {#getUniqueId--}
```
public String getUniqueId()
```


Ottiene l'ID univoco, è lo stesso di \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public ValidationCollection getValidations()
```


Ottiene la collezione delle impostazioni di convalida dei dati nel foglio di lavoro.

**Returns:**
[ValidationCollection](../../com.aspose.cells/validationcollection)
### getVerticalPageBreaks() {#getVerticalPageBreaks--}
```
public VerticalPageBreakCollection getVerticalPageBreaks()
```


Ottiene la collezione di [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection).

**Returns:**
[VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)
### getViewType() {#getViewType--}
```
public int getViewType()
```


Ottiene il tipo di visualizzazione.

Vedi [ViewType](../../com.aspose.cells/viewtype).

**Returns:**
int
### getVisibilityType() {#getVisibilityType--}
```
public int getVisibilityType()
```


Indica lo stato di visibilità per questo foglio.

Vedi [VisibilityType](../../com.aspose.cells/visibilitytype).

**Returns:**
int
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Ottiene l'oggetto workbook che contiene questo foglio.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400.

**Remarks**

Si prega di impostare prima il tipo di visualizzazione.

**Returns:**
int
### hasAutofilter() {#hasAutofilter--}
```
public boolean hasAutofilter()
```


Indica se questo foglio di lavoro ha il filtro automatico.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


Ottiene un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true.

**Returns:**
boolean
### isOutlineShown() {#isOutlineShown--}
```
public boolean isOutlineShown()
```


Indica se mostrare la struttura.

**Returns:**
boolean
### isPageBreakPreview() {#isPageBreakPreview--}
```
public boolean isPageBreakPreview()
```


Indica se il foglio di lavoro specificato è mostrato in visualizzazione normale o anteprima interruzione di pagina.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Indica se il foglio di lavoro è protetto.

**Returns:**
boolean
### isRowColumnHeadersVisible() {#isRowColumnHeadersVisible--}
```
public boolean isRowColumnHeadersVisible()
```


Ottiene un valore che indica se il foglio di lavoro visualizzerà le intestazioni di righe e colonne. Il valore predefinito è true.

**Returns:**
boolean
### isRulerVisible() {#isRulerVisible--}
```
public boolean isRulerVisible()
```


Indica se il righello è visibile. Questa proprietà viene applicata solo per l'anteprima dell'interruzione di pagina.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Rappresenta se il foglio di lavoro è visibile.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


Sposta il foglio in un'altra posizione nel foglio di calcolo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | Indice del foglio di destinazione. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### protect(int type) {#protect-int-}
```
public void protect(int type)
```


Protegge il foglio di lavoro.

**Remarks**

Questo metodo protegge il foglio di lavoro senza password. Può proteggere il foglio di lavoro in tutte le versioni del file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Tipo di protezione. |

### protect(int type, String password, String oldPassword) {#protect-int-java.lang.String-java.lang.String-}
```
public void protect(int type, String password, String oldPassword)
```


Protegge il foglio di lavoro.

**Remarks**

Questo metodo può proteggere il foglio di lavoro in tutte le versioni del file Excel.

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = excel.getWorksheets().get(0);
         //Protecting the worksheet with a password
         worksheet.protect(ProtectionType.ALL, "aspose", null);
         //Saving the modified Excel file in default (that is Excel 20003) format
         excel.save("output.xls");
         //Closing the file stream to free all resources
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Tipo di protezione. |
| password | java.lang.String | Password. |
| oldPassword | java.lang.String | Se il foglio di lavoro è già protetto da una password, fornire la vecchia password. In caso contrario, è possibile impostare un valore nullo o una stringa vuota per questo parametro. |

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Aggiorna tutte le PivotTable in questo foglio di lavoro.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Aggiorna tutte le PivotTable in questo foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | L'opzione per aggiornare l'origine dati della tabella pivot. |

**Returns:**
boolean
### removeAllDrawingObjects() {#removeAllDrawingObjects--}
```
public void removeAllDrawingObjects()
```


Rimuove tutti gli oggetti di disegno in questo foglio di lavoro.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Rimuove il filtro automatico del foglio di lavoro.

### removeSplit() {#removeSplit--}
```
public void removeSplit()
```


Rimuove la divisione della finestra.

### replace(String oldString, String newString) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String oldString, String newString)
```


Sostituisce il testo di tutte le celle con una nuova stringa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| oldString | java.lang.String | Valore della stringa vecchia. |
| newString | java.lang.String | Valore della nuova stringa. |

**Returns:**
int
### selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers) {#selectRange-int-int-int-int-boolean-}
```
public void selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)
```


Seleziona un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Riga di inizio. |
| startColumn | int | Colonna di inizio |
| totalRows | int | Numero di righe. |
| totalColumns | int | Numero di colonne |
| removeOthers | boolean | True indica la rimozione di altri intervalli selezionati e la selezione solo di questo intervallo. |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Imposta la cella attiva nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Imposta l'immagine di sfondo del foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte[] |  |

### setCodeName(String value) {#setCodeName-java.lang.String-}
```
public void setCodeName(String value)
```


Ottiene il nome codice del foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra invece che da sinistra a destra. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


Vero se i valori zero sono visualizzati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


Rappresenta l'indice della prima colonna visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


Rappresenta l'indice della prima riga visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Imposta il colore della linea della griglia

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Imposta un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome del foglio di lavoro.

**Remarks**

La lunghezza massima del nome del foglio è 31. E non è possibile assegnare lo stesso nome (senza distinzione tra maiuscole e minuscole) a due fogli di lavoro. Ad esempio, non è possibile impostare "SheetName1" al primo foglio e impostare "SHEETNAME1" al secondo foglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


Indica se mostrare la struttura.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPageBreakPreview(boolean value) {#setPageBreakPreview-boolean-}
```
public void setPageBreakPreview(boolean value)
```


Indica se il foglio di lavoro specificato è mostrato in visualizzazione normale o anteprima interruzione di pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRowColumnHeadersVisible(boolean value) {#setRowColumnHeadersVisible-boolean-}
```
public void setRowColumnHeadersVisible(boolean value)
```


Imposta un valore che indica se il foglio di lavoro visualizzerà le intestazioni di righe e colonne. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRulerVisible(boolean value) {#setRulerVisible-boolean-}
```
public void setRulerVisible(boolean value)
```


Indica se il righello è visibile. Questa proprietà viene applicata solo per l'anteprima dell'interruzione di pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowDataTypeIcons(boolean value) {#setShowDataTypeIcons-boolean-}
```
public void setShowDataTypeIcons(boolean value)
```


Indica se mostrare le icone del tipo di dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowFormulas(boolean value) {#setShowFormulas-boolean-}
```
public void setShowFormulas(boolean value)
```


Indica se mostrare le formule o i loro risultati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.cells.Color-}
```
public void setTabColor(Color value)
```


Rappresenta il colore della scheda del foglio di lavoro.

**Remarks**

Questa funzionalità è supportata solo in ExcelXP (Excel2002) e versioni successive. Se si salva il file in formato Excel97 o Excel2000, verrà omessa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setTabId(int value) {#setTabId-int-}
```
public void setTabId(int value)
```


Specifica l'identificatore interno per il foglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTransitionEntry(boolean value) {#setTransitionEntry-boolean-}
```
public void setTransitionEntry(boolean value)
```


Indica se l'opzione Transition Formula Entry (compatibilità Lotus) è abilitata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTransitionEvaluation(boolean value) {#setTransitionEvaluation-boolean-}
```
public void setTransitionEvaluation(boolean value)
```


Indica se l'opzione Transition Formula Evaluation (compatibilità Lotus) è abilitata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Rappresenta il tipo di foglio di lavoro.

Vedi [SheetType](../../com.aspose.cells/sheettype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setUniqueId(String value) {#setUniqueId-java.lang.String-}
```
public void setUniqueId(String value)
```


Imposta l'ID univoco, è lo stesso di \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\}.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setViewType(int value) {#setViewType-int-}
```
public void setViewType(int value)
```


Imposta il tipo di visualizzazione.

Vedi [ViewType](../../com.aspose.cells/viewtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setVisibilityType(int value) {#setVisibilityType-int-}
```
public void setVisibilityType(int value)
```


Indica lo stato di visibilità per questo foglio.

Vedi [VisibilityType](../../com.aspose.cells/visibilitytype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Rappresenta se il foglio di lavoro è visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setVisible(boolean isVisible, boolean ignoreError) {#setVisible-boolean-boolean-}
```
public void setVisible(boolean isVisible, boolean ignoreError)
```


Imposta le opzioni visibili.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isVisible | boolean | Se il foglio di lavoro è visibile |
| ignoreError | boolean | Se ignorare l'errore se questa opzione non è valida. |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400.

**Remarks**

Si prega di impostare prima il tipo di visualizzazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### split() {#split--}
```
public void split()
```


Dividi la finestra.

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Avvia la sessione che utilizza le cache per accedere ai dati in questo foglio di lavoro.

**Remarks**

Dopo aver terminato l'accesso ai dati, [closeAccessCache(int)](../../com.aspose.cells/worksheet\#closeAccessCache-int-) dovrebbe essere invocato con le stesse opzioni per cancellare tutte le cache e ripristinare la modalità di accesso normale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). opzioni di accesso ai dati |

### toString() {#toString--}
```
public String toString()
```


Restituisce una stringa che rappresenta l'oggetto Worksheet corrente.

**Returns:**
java.lang.String -
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Sblocca i riquadri nel foglio di lavoro.

### unprotect() {#unprotect--}
```
public void unprotect()
```


Rimuove la protezione dal foglio di lavoro.

**Remarks**

Questo metodo rimuove la protezione dal foglio di lavoro che è protetto senza password.

### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Rimuove la protezione dal foglio di lavoro.

**Remarks**

Se il foglio di lavoro è protetto senza password, è possibile impostare un valore null o una stringa vuota al parametro password.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | java.lang.String | Password |

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

### xmlMapQuery(String path, XmlMap xmlMap) {#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public ArrayList xmlMapQuery(String path, XmlMap xmlMap)
```


Interroga le aree di celle mappate/collegate al percorso specifico della mappa XML.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Worksheet.GetAreasOfXmlMapQuery(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | java.lang.String | percorso dell'elemento xml |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Specificare una mappa xml se si desidera interrogare il percorso specifico all'interno di una mappa specifica |

**Returns:**
java.util.ArrayList - [CellArea](../../com.aspose.cells/cellarea) elenco che è stato mappato/collegato al percorso specifico della mappa XML, viene restituito un elenco vuoto se nulla è mappato/collegato.
