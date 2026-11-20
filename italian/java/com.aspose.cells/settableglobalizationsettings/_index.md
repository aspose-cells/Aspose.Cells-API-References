---
title: "SettableGlobalizationSettings"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Implementazione di GlobalizationSettings che consente all'utente di impostare/modificare testi predefiniti."
type: docs
url: /it/java/com.aspose.cells/settableglobalizationsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
```
public class SettableGlobalizationSettings extends GlobalizationSettings
```

Implementazione di GlobalizationSettings che consente all'utente di impostare/modificare testi predefiniti.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SettableGlobalizationSettings()](#SettableGlobalizationSettings--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Confronta due valori stringa secondo alcune regole di collazione. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllName()](#getAllName--) | Ottiene il nome dell'etichetta "(All)" nella PivotTable. |
| [getBooleanValueString(boolean bv)](#getBooleanValueString-boolean-) | Ottiene il valore stringa visualizzato per il valore booleano della cella. |
| [getChartSettings()](#getChartSettings--) | Ottiene le impostazioni di globalizzazione per il grafico. |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Trasforma la stringa in un oggetto confrontabile secondo alcune regole di collazione. |
| [getColumnLabelsOfPivotTable()](#getColumnLabelsOfPivotTable--) | Ottiene il nome dell'etichetta "Column Labels" nella PivotTable. |
| [getColumnSeparatorOfFormulaArray()](#getColumnSeparatorOfFormulaArray--) | Ottiene il separatore per gli elementi nei dati di riga dell'array nella formula. |
| [getCommentTitleName(int type)](#getCommentTitleName-int-) | Ottiene il nome del titolo del commento dipendente dalla locale secondo il tipo di titolo del commento. |
| [getDataFieldHeaderNameOfPivotTable()](#getDataFieldHeaderNameOfPivotTable--) | Ottiene il nome dell'intestazione del campo dell'area valori nella PivotTable. |
| [getDefaultSheetName()](#getDefaultSheetName--) | Ottiene il nome del foglio predefinito per aggiungere automaticamente un foglio di lavoro. |
| [getEmptyDataName()](#getEmptyDataName--) | Ottiene il nome dell'etichetta "(blank)" nella tabella pivot. |
| [getErrorValueString(String err)](#getErrorValueString-java.lang.String-) | Ottiene il valore stringa visualizzato per il valore di errore della cella |
| [getGrandTotalName(int functionType)](#getGrandTotalName-int-) | Ottiene il nome del totale generale della funzione. |
| [getListSeparator()](#getListSeparator--) | Ottiene il separatore per elenchi, parametri della funzione, ...ecc. |
| [getLocalBuiltInName(String standardName)](#getLocalBuiltInName-java.lang.String-) | Ottiene il testo dipendente dalla locale per il Nome incorporato in base al testo standard fornito. |
| [getLocalFunctionName(String standardName)](#getLocalFunctionName-java.lang.String-) | Ottiene il nome della funzione dipendente dalla locale in base al nome della funzione standard fornito. |
| [getMultipleItemsName()](#getMultipleItemsName--) | Ottiene il nome dell'etichetta "(Multiple Items)" nella tabella pivot. |
| [getPivotGrandTotalName()](#getPivotGrandTotalName--) | Ottiene il nome dell'etichetta "Grand Total" nella tabella pivot. |
| [getPivotSettings()](#getPivotSettings--) | Ottiene le impostazioni di globalizzazione per la tabella pivot. |
| [getPivotTotalName()](#getPivotTotalName--) | Ottiene il nome dell'etichetta "Total" nella tabella pivot. |
| [getProtectionNameOfPivotTable()](#getProtectionNameOfPivotTable--) | Ottiene il nome della protezione nella tabella pivot. |
| [getRowLabelsNameOfPivotTable()](#getRowLabelsNameOfPivotTable--) | Ottiene il nome dell'etichetta "Row Labels" nella tabella pivot. |
| [getRowSeparatorOfFormulaArray()](#getRowSeparatorOfFormulaArray--) | Ottiene il separatore per le righe nei dati array nella formula. |
| [getStandardBuiltInName(String localName)](#getStandardBuiltInName-java.lang.String-) | Ottiene il testo standard del Nome incorporato in base al testo dipendente dalla locale fornito. |
| [getStandardFunctionName(String localName)](#getStandardFunctionName-java.lang.String-) | Ottiene il nome standard della funzione in base al nome della funzione dipendente dalla locale fornito. |
| [getStandardHeaderFooterFontStyleName(String localfontStyleName)](#getStandardHeaderFooterFontStyleName-java.lang.String-) | Ottiene il nome standard in inglese dello stile di carattere (Regular, Bold, Italic) per Intestazione/Piè di pagina in base al nome dello stile di carattere locale fornito. |
| [getSubTotalName(int subTotalType)](#getSubTotalName-int-) | Ottiene il nome del tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) nella tabella pivot. |
| [getTableRowTypeOfAll()](#getTableRowTypeOfAll--) | Ottiene il nome del tipo di righe della tabella che comprende tutte le righe nella tabella di riferimento. |
| [getTableRowTypeOfCurrent()](#getTableRowTypeOfCurrent--) | Ottiene il nome del tipo di righe della tabella che comprende la riga corrente nella tabella di riferimento. |
| [getTableRowTypeOfData()](#getTableRowTypeOfData--) | Ottiene il nome del tipo di righe della tabella che comprende la regione dati della tabella di riferimento. |
| [getTableRowTypeOfHeaders()](#getTableRowTypeOfHeaders--) | Ottiene il nome del tipo di righe della tabella che comprende l'intestazione della tabella. |
| [getTableRowTypeOfTotals()](#getTableRowTypeOfTotals--) | Ottiene il nome del tipo di righe della tabella che comprende la riga totale della tabella di riferimento. |
| [getTotalName(int functionType)](#getTotalName-int-) | Ottiene il nome totale della funzione specifica. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBooleanValueString(boolean bv, String name)](#setBooleanValueString-boolean-java.lang.String-) | Imposta il valore stringa visualizzato per il valore booleano della cella |
| [setChartSettings(ChartGlobalizationSettings value)](#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-) | Imposta le impostazioni di globalizzazione per il grafico. |
| [setColumnSeparatorOfFormulaArray(char c)](#setColumnSeparatorOfFormulaArray-char-) | Imposta il separatore per gli elementi nei dati di riga dell'array nella formula. |
| [setCommentTitleName(int type, String name)](#setCommentTitleName-int-java.lang.String-) | Ottiene il nome del titolo del commento dipendente dalla locale secondo il tipo di titolo del commento. |
| [setGrandTotalName(int functionType, String name)](#setGrandTotalName-int-java.lang.String-) | Imposta il nome del totale generale di una funzione specifica. |
| [setListSeparator(char c)](#setListSeparator-char-) | Imposta il separatore per l'elenco, i parametri della funzione, ...ecc. |
| [setLocalBuiltInName(String standardName, String localName, boolean bidirectional)](#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-) | Imposta il testo dipendente dalla locale per il nome incorporato con il testo del nome standard fornito. |
| [setLocalFunctionName(String standardName, String localName, boolean bidirectional)](#setLocalFunctionName-java.lang.String-java.lang.String-boolean-) | Imposta il nome della funzione dipendente dalla locale corrispondente al nome della funzione standard fornito. |
| [setPivotSettings(PivotGlobalizationSettings value)](#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-) | Imposta le impostazioni di globalizzazione per la tabella pivot. |
| [setRowSeparatorOfFormulaArray(char c)](#setRowSeparatorOfFormulaArray-char-) | Imposta il separatore per le righe nei dati dell'array nella formula. |
| [setStandardBuiltInName(String localName, String standardName, boolean bidirectional)](#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-) | Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito. |
| [setStandardFunctionName(String localName, String standardName, boolean bidirectional)](#setStandardFunctionName-java.lang.String-java.lang.String-boolean-) | Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito. |
| [setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)](#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-) | Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito. |
| [setTableRowTypeOfAll(String name)](#setTableRowTypeOfAll-java.lang.String-) | Imposta il nome del tipo di righe della tabella che comprende tutte le righe nella tabella di riferimento. |
| [setTableRowTypeOfCurrent(String name)](#setTableRowTypeOfCurrent-java.lang.String-) | Imposta il nome del tipo di righe della tabella che comprende la riga corrente nella tabella di riferimento. |
| [setTableRowTypeOfData(String name)](#setTableRowTypeOfData-java.lang.String-) | Imposta il nome del tipo di righe della tabella che comprende la regione dati della tabella di riferimento. |
| [setTableRowTypeOfHeaders(String name)](#setTableRowTypeOfHeaders-java.lang.String-) | Imposta il nome del tipo di righe della tabella che comprende l'intestazione della tabella. |
| [setTableRowTypeOfTotals(String name)](#setTableRowTypeOfTotals-java.lang.String-) | Imposta il nome del tipo di righe della tabella che comprende la riga totale della tabella di riferimento. |
| [setTotalName(int functionType, String name)](#setTotalName-int-java.lang.String-) | Imposta il nome totale di una funzione specifica. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SettableGlobalizationSettings() {#SettableGlobalizationSettings--}
```
public SettableGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Confronta due valori stringa secondo alcune regole di collazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| v1 | java.lang.String | la prima stringa |
| v2 | java.lang.String | la seconda stringa |
| ignoreCase | boolean | se ignorare la differenza tra maiuscole e minuscole durante il confronto dei valori |

**Returns:**
int - Intero che indica la relazione lessicale tra i due comparandi
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
### getAllName() {#getAllName--}
```
public String getAllName()
```


Ottiene il nome dell'etichetta "(All)" nella PivotTable.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo GlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa tra 12 mesi a partire da dicembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
java.lang.String - Il nome dell'etichetta "(All)"
### getBooleanValueString(boolean bv) {#getBooleanValueString-boolean-}
```
public String getBooleanValueString(boolean bv)
```


Ottiene il valore stringa visualizzato per il valore booleano della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| bv | boolean | valore booleano |

**Returns:**
java.lang.String - Per impostazione predefinita restituisce "TRUE" per il valore vero e "FALSE" per il valore falso.
### getChartSettings() {#getChartSettings--}
```
public ChartGlobalizationSettings getChartSettings()
```


Ottiene le impostazioni di globalizzazione per il grafico.

**Returns:**
[ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Trasforma la stringa in un oggetto confrontabile secondo alcune regole di collazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| v | java.lang.String | Il valore String deve essere confrontato con altri. |
| ignoreCase | boolean | se ignorare la differenza tra maiuscole e minuscole durante il confronto dei valori |

**Returns:**
java.lang.Comparable - L'oggetto può essere usato per confrontare o ordinare valori stringa
### getColumnLabelsOfPivotTable() {#getColumnLabelsOfPivotTable--}
```
public String getColumnLabelsOfPivotTable()
```


Ottiene il nome dell'etichetta "Column Labels" nella PivotTable.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.lang.String - Il nome delle etichette di colonna
### getColumnSeparatorOfFormulaArray() {#getColumnSeparatorOfFormulaArray--}
```
public char getColumnSeparatorOfFormulaArray()
```


Ottiene il separatore per gli elementi nei dati di riga dell'array nella formula.

**Returns:**
char
### getCommentTitleName(int type) {#getCommentTitleName-int-}
```
public String getCommentTitleName(int type)
```


Ottiene il nome del titolo del commento dipendente dalla locale secondo il tipo di titolo del commento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). tipo di titolo del commento |

**Returns:**
java.lang.String - nome del titolo del commento dipendente dalla locale
### getDataFieldHeaderNameOfPivotTable() {#getDataFieldHeaderNameOfPivotTable--}
```
public String getDataFieldHeaderNameOfPivotTable()
```


Ottiene il nome dell'intestazione del campo dell'area valori nella PivotTable.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.lang.String - Il nome dell'intestazione del campo dati
### getDefaultSheetName() {#getDefaultSheetName--}
```
public String getDefaultSheetName()
```


Ottiene il nome del foglio predefinito per aggiungere automaticamente un foglio di lavoro. Il valore predefinito è "Sheet".

**Remarks**

Il nome del foglio aggiunto automaticamente (ad esempio tramite [WorksheetCollection.add()](../../com.aspose.cells/worksheetcollection\#add--)) sarà il nome specificato più un numero di sequenza. Per esempio, un utente tedesco potrebbe volere che il nome del foglio sia "Tabellenblatt2" invece di "Sheet2". In tal caso l'utente può implementare questo metodo per restituire "Tabellenblatt".

**Returns:**
java.lang.String - il nome predefinito del foglio per aggiungere automaticamente un foglio di lavoro
### getEmptyDataName() {#getEmptyDataName--}
```
public String getEmptyDataName()
```


Ottiene il nome dell'etichetta "(blank)" nella tabella pivot.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.lang.String - Il nome dei dati vuoti
### getErrorValueString(String err) {#getErrorValueString-java.lang.String-}
```
public String getErrorValueString(String err)
```


Ottiene il valore stringa visualizzato per il valore di errore della cella

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| err | java.lang.String | valori di errore come \#VALUE!,\#NAME? |

**Returns:**
java.lang.String - Per impostazione predefinita restituisce il valore di errore stesso
### getGrandTotalName(int functionType) {#getGrandTotalName-int-}
```
public String getGrandTotalName(int functionType)
```


Ottiene il nome del totale generale della funzione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Il tipo di funzione. |

**Returns:**
java.lang.String - Il nome del totale generale della funzione.
### getListSeparator() {#getListSeparator--}
```
public char getListSeparator()
```


Ottiene il separatore per elenchi, parametri della funzione, ...ecc.

**Returns:**
char
### getLocalBuiltInName(String standardName) {#getLocalBuiltInName-java.lang.String-}
```
public String getLocalBuiltInName(String standardName)
```


Ottiene il testo dipendente dalla locale per il Nome incorporato in base al testo standard fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| standardName | java.lang.String | Standard (locale en-US) testo del Nome incorporato. |

**Returns:**
java.lang.String - Testo dipendente dalla locale. La locale è stata specificata dalla Cartella di lavoro per la quale queste impostazioni sono utilizzate.
### getLocalFunctionName(String standardName) {#getLocalFunctionName-java.lang.String-}
```
public String getLocalFunctionName(String standardName)
```


Ottiene il nome della funzione dipendente dalla locale in base al nome della funzione standard fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| standardName | java.lang.String | Standard (locale en-US) nome della funzione. |

**Returns:**
java.lang.String - Nome della funzione dipendente dalla locale. La locale è stata specificata dalla Cartella di lavoro per la quale queste impostazioni sono utilizzate.
### getMultipleItemsName() {#getMultipleItemsName--}
```
public String getMultipleItemsName()
```


Ottiene il nome dell'etichetta "(Multiple Items)" nella tabella pivot.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.lang.String - Il nome dell'etichetta "(Multiple Items)"
### getPivotGrandTotalName() {#getPivotGrandTotalName--}
```
public String getPivotGrandTotalName()
```


Ottiene il nome dell'etichetta "Grand Total" nella tabella pivot.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.lang.String - Il nome dell'etichetta "Grand Total"
### getPivotSettings() {#getPivotSettings--}
```
public PivotGlobalizationSettings getPivotSettings()
```


Ottiene le impostazioni di globalizzazione per la tabella pivot.

**Returns:**
[PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
### getPivotTotalName() {#getPivotTotalName--}
```
public String getPivotTotalName()
```


Restituisce il nome dell'etichetta "Total" nella PivotTable. È necessario sovrascrivere questo metodo quando la PivotTable contiene due o più PivotFields nell'area dati.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.lang.String - Il nome dell'etichetta "Total"
### getProtectionNameOfPivotTable() {#getProtectionNameOfPivotTable--}
```
public String getProtectionNameOfPivotTable()
```


Ottiene il nome della protezione nella tabella pivot.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetTextOfProtectedName(string). Questa proprietà verrà rimossa tra 12 mesi a partire da dicembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
java.lang.String - Il nome di protezione della PivotTable
### getRowLabelsNameOfPivotTable() {#getRowLabelsNameOfPivotTable--}
```
public String getRowLabelsNameOfPivotTable()
```


Ottiene il nome dell'etichetta "Row Labels" nella tabella pivot.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.lang.String - Il nome delle etichette di riga
### getRowSeparatorOfFormulaArray() {#getRowSeparatorOfFormulaArray--}
```
public char getRowSeparatorOfFormulaArray()
```


Ottiene il separatore per le righe nei dati array nella formula.

**Returns:**
char
### getStandardBuiltInName(String localName) {#getStandardBuiltInName-java.lang.String-}
```
public String getStandardBuiltInName(String localName)
```


Ottiene il testo standard del Nome incorporato in base al testo dipendente dalla locale fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| localName | java.lang.String | Testo dipendente dalla locale del Nome incorporato. La locale è stata specificata dalla Cartella di lavoro per la quale queste impostazioni sono utilizzate. |

**Returns:**
java.lang.String - Testo standard (locale en-US).
### getStandardFunctionName(String localName) {#getStandardFunctionName-java.lang.String-}
```
public String getStandardFunctionName(String localName)
```


Ottiene il nome standard della funzione in base al nome della funzione dipendente dalla locale fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| localName | java.lang.String | Nome della funzione dipendente dalla locale. La locale è stata specificata dalla Cartella di lavoro per la quale queste impostazioni sono utilizzate. |

**Returns:**
java.lang.String - Nome della funzione standard (locale en-US).
### getStandardHeaderFooterFontStyleName(String localfontStyleName) {#getStandardHeaderFooterFontStyleName-java.lang.String-}
```
public String getStandardHeaderFooterFontStyleName(String localfontStyleName)
```


Ottiene il nome standard in inglese dello stile di carattere (Regular, Bold, Italic) per Intestazione/Piè di pagina in base al nome dello stile di carattere locale fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Nome dello stile di carattere della locale per Intestazione/Piè di pagina. |

**Returns:**
java.lang.String - Nome standard dello stile di carattere inglese (Regular, Bold, Italic)
### getSubTotalName(int subTotalType) {#getSubTotalName-int-}
```
public String getSubTotalName(int subTotalType)
```


Ottiene il nome del tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) nella tabella pivot.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Il tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - Il nome del tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype)
### getTableRowTypeOfAll() {#getTableRowTypeOfAll--}
```
public String getTableRowTypeOfAll()
```


Ottiene il nome del tipo di righe della tabella che comprende tutte le righe nella tabella di riferimento.

**Returns:**
java.lang.String - il nome del tipo di righe della tabella
### getTableRowTypeOfCurrent() {#getTableRowTypeOfCurrent--}
```
public String getTableRowTypeOfCurrent()
```


Ottiene il nome del tipo di righe della tabella che comprende la riga corrente nella tabella di riferimento.

**Returns:**
java.lang.String - il nome del tipo di righe della tabella
### getTableRowTypeOfData() {#getTableRowTypeOfData--}
```
public String getTableRowTypeOfData()
```


Restituisce il nome del tipo di righe della tabella che consiste nella regione dati della tabella di riferimento. Il valore predefinito è "Data", quindi nella formula "\\#Data" rappresenta la regione dati della tabella.

**Returns:**
java.lang.String - il nome del tipo di righe della tabella
### getTableRowTypeOfHeaders() {#getTableRowTypeOfHeaders--}
```
public String getTableRowTypeOfHeaders()
```


Restituisce il nome del tipo di righe della tabella che consiste nell'intestazione della tabella. Il valore predefinito è "Headers", quindi nella formula "\\#Headers" rappresenta l'intestazione della tabella.

**Returns:**
java.lang.String - il nome del tipo di righe della tabella
### getTableRowTypeOfTotals() {#getTableRowTypeOfTotals--}
```
public String getTableRowTypeOfTotals()
```


Ottiene il nome del tipo di righe della tabella che comprende la riga totale della tabella di riferimento.

**Returns:**
java.lang.String - il nome del tipo di righe della tabella
### getTotalName(int functionType) {#getTotalName-int-}
```
public String getTotalName(int functionType)
```


Ottiene il nome totale della funzione specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Il tipo di funzione. |

**Returns:**
java.lang.String - Il nome totale della funzione.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBooleanValueString(boolean bv, String name) {#setBooleanValueString-boolean-java.lang.String-}
```
public void setBooleanValueString(boolean bv, String name)
```


Imposta il valore stringa visualizzato per il valore booleano della cella

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| bv | boolean | valore booleano |
| name | java.lang.String | valore stringa del valore booleano |

### setChartSettings(ChartGlobalizationSettings value) {#setChartSettings-com.aspose.cells.ChartGlobalizationSettings-}
```
public void setChartSettings(ChartGlobalizationSettings value)
```


Imposta le impostazioni di globalizzazione per il grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ChartGlobalizationSettings](../../com.aspose.cells/chartglobalizationsettings) |  |

### setColumnSeparatorOfFormulaArray(char c) {#setColumnSeparatorOfFormulaArray-char-}
```
public void setColumnSeparatorOfFormulaArray(char c)
```


Imposta il separatore per gli elementi nei dati di riga dell'array nella formula.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| c | char | il separatore specificato |

### setCommentTitleName(int type, String name) {#setCommentTitleName-int-java.lang.String-}
```
public void setCommentTitleName(int type, String name)
```


Ottiene il nome del titolo del commento dipendente dalla locale secondo il tipo di titolo del commento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [CommentTitleType](../../com.aspose.cells/commenttitletype). tipo di titolo del commento |
| name | java.lang.String | nome del titolo del commento dipendente dalla locale |

### setGrandTotalName(int functionType, String name) {#setGrandTotalName-int-java.lang.String-}
```
public void setGrandTotalName(int functionType, String name)
```


Imposta il nome del totale generale di una funzione specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Il tipo di funzione. |
| name | java.lang.String | Il nome del totale generale della funzione. |

### setListSeparator(char c) {#setListSeparator-char-}
```
public void setListSeparator(char c)
```


Imposta il separatore per l'elenco, i parametri della funzione, ...ecc.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| c | char | il separatore specificato |

### setLocalBuiltInName(String standardName, String localName, boolean bidirectional) {#setLocalBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalBuiltInName(String standardName, String localName, boolean bidirectional)
```


Imposta il testo dipendente dalla locale per il nome incorporato con il testo del nome standard fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| standardName | java.lang.String | Testo del nome standard (locale en-US) del nome incorporato. |
| localName | java.lang.String | Testo del nome dipendente dalla locale |
| bidirectional | boolean | Indica se mappare automaticamente il testo del nome locale al testo del nome standard. Se vero, il testo del nome locale verrà mappato al testo del nome standard automaticamente così l'utente non dovrà chiamare nuovamente [setStandardBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardBuiltInName-String-String-boolean-) per la stessa coppia di nomi standard e locale. |

### setLocalFunctionName(String standardName, String localName, boolean bidirectional) {#setLocalFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setLocalFunctionName(String standardName, String localName, boolean bidirectional)
```


Imposta il nome della funzione dipendente dalla locale corrispondente al nome della funzione standard fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| standardName | java.lang.String | Standard (locale en-US) nome della funzione. |
| localName | java.lang.String | Nome della funzione dipendente dalla locale |
| bidirectional | boolean | Indica se mappare automaticamente il nome della funzione locale al nome della funzione standard. Se vero, il nome locale verrà mappato al nome standard automaticamente così l'utente non dovrà chiamare nuovamente [setStandardFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setStandardFunctionName-String-String-boolean-) per la stessa coppia di nomi standard e locale. |

### setPivotSettings(PivotGlobalizationSettings value) {#setPivotSettings-com.aspose.cells.PivotGlobalizationSettings-}
```
public void setPivotSettings(PivotGlobalizationSettings value)
```


Imposta le impostazioni di globalizzazione per la tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) |  |

### setRowSeparatorOfFormulaArray(char c) {#setRowSeparatorOfFormulaArray-char-}
```
public void setRowSeparatorOfFormulaArray(char c)
```


Imposta il separatore per le righe nei dati dell'array nella formula.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| c | char | il separatore specificato |

### setStandardBuiltInName(String localName, String standardName, boolean bidirectional) {#setStandardBuiltInName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardBuiltInName(String localName, String standardName, boolean bidirectional)
```


Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| localName | java.lang.String | Nome della funzione dipendente dalla locale |
| standardName | java.lang.String | Standard (locale en-US) nome della funzione. |
| bidirectional | boolean | Indica se mappare automaticamente il testo del nome standard al testo del nome locale. Se vero, il testo del nome standard verrà mappato al testo del nome locale automaticamente così l'utente non dovrà chiamare nuovamente [setLocalBuiltInName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalBuiltInName-String-String-boolean-) per la stessa coppia di nomi standard e locale. |

### setStandardFunctionName(String localName, String standardName, boolean bidirectional) {#setStandardFunctionName-java.lang.String-java.lang.String-boolean-}
```
public void setStandardFunctionName(String localName, String standardName, boolean bidirectional)
```


Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| localName | java.lang.String | Nome della funzione dipendente dalla locale |
| standardName | java.lang.String | Standard (locale en-US) nome della funzione. |
| bidirectional | boolean | Indica se mappare automaticamente il nome della funzione standard al nome della funzione locale. Se vero, il nome standard verrà mappato al nome locale automaticamente così l'utente non dovrà chiamare nuovamente [setLocalFunctionName(String,String,boolean)](../../com.aspose.cells/settableglobalizationsettings\#setLocalFunctionName-String-String-boolean-) per la stessa coppia di nomi standard e locale. |

### setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName) {#setStandardHeaderFooterFontStyleName-java.lang.String-java.lang.String-}
```
public void setStandardHeaderFooterFontStyleName(String localfontStyleName, String standardName)
```


Imposta il nome della funzione dipendente dalla locale secondo il nome della funzione standard fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| localfontStyleName | java.lang.String | Nome dello stile di carattere della locale per Intestazione/Piè di pagina. |
| standardName | java.lang.String | Standard (locale en-US) nome della funzione. |

### setTableRowTypeOfAll(String name) {#setTableRowTypeOfAll-java.lang.String-}
```
public void setTableRowTypeOfAll(String name)
```


Imposta il nome del tipo di righe della tabella che comprende tutte le righe nella tabella di riferimento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | il nome del tipo di righe della tabella |

### setTableRowTypeOfCurrent(String name) {#setTableRowTypeOfCurrent-java.lang.String-}
```
public void setTableRowTypeOfCurrent(String name)
```


Imposta il nome del tipo di righe della tabella che comprende la riga corrente nella tabella di riferimento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | il nome del tipo di righe della tabella |

### setTableRowTypeOfData(String name) {#setTableRowTypeOfData-java.lang.String-}
```
public void setTableRowTypeOfData(String name)
```


Imposta il nome del tipo di righe della tabella che comprende la regione dati della tabella di riferimento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | il nome del tipo di righe della tabella |

### setTableRowTypeOfHeaders(String name) {#setTableRowTypeOfHeaders-java.lang.String-}
```
public void setTableRowTypeOfHeaders(String name)
```


Imposta il nome del tipo di righe della tabella che comprende l'intestazione della tabella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | il nome del tipo di righe della tabella |

### setTableRowTypeOfTotals(String name) {#setTableRowTypeOfTotals-java.lang.String-}
```
public void setTableRowTypeOfTotals(String name)
```


Imposta il nome del tipo di righe della tabella che comprende la riga totale della tabella di riferimento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | il nome del tipo di righe della tabella |

### setTotalName(int functionType, String name) {#setTotalName-int-java.lang.String-}
```
public void setTotalName(int functionType, String name)
```


Imposta il nome totale di una funzione specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| functionType | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). Il tipo di funzione. |
| name | java.lang.String | Il nome totale della funzione. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
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

