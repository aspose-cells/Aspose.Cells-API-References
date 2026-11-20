---
title: "SettablePivotGlobalizationSettings"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Implementazione di PivotGlobalizationSettings che consente all'utente di impostare/modificare testi predefiniti."
type: docs
url: /it/java/com.aspose.cells/settablepivotglobalizationsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
```
public class SettablePivotGlobalizationSettings extends PivotGlobalizationSettings
```

Implementazione di PivotGlobalizationSettings che consente all'utente di impostare/modificare testi predefiniti.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SettablePivotGlobalizationSettings()](#SettablePivotGlobalizationSettings--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatOfDayGroup()](#getFormatOfDayGroup--) | Ottiene il formato numerico del gruppo giorno del pivot. |
| [getNameOfDataField(int function, String name)](#getNameOfDataField-int-java.lang.String-) | Ottiene il nome visualizzato del campo pivot dei dati. |
| [getShortTextOf12Months()](#getShortTextOf12Months--) | Ottiene tutte le stringhe formattate brevemente dei 12 mesi. |
| [getTextOf24Hours()](#getTextOf24Hours--) | Ottiene tutte le stringhe formattate localmente delle 24 ore. |
| [getTextOf4Quarters()](#getTextOf4Quarters--) | Ottiene il testo locale dei 4 trimestri. |
| [getTextOf4Quaters()](#getTextOf4Quaters--) | Ottiene il testo locale dei 4 trimestri. |
| [getTextOfAll()](#getTextOfAll--) | Ottiene il testo dell\"(All)\" etichetta nella Tabella Pivot. |
| [getTextOfAllPeriods()](#getTextOfAllPeriods--) | Ottiene il testo localizzato di \"All Periods\". |
| [getTextOfColumnLabels()](#getTextOfColumnLabels--) | Ottiene il testo dell\"Column Labels\" etichetta nella Tabella Pivot. |
| [getTextOfDataFieldHeader()](#getTextOfDataFieldHeader--) | Restituisce il testo dell'intestazione del campo area valore nella Tabella pivot. |
| [getTextOfDays()](#getTextOfDays--) | Restituisce il testo locale di "Days". |
| [getTextOfEmptyData()](#getTextOfEmptyData--) | Restituisce il testo dell'etichetta "(blank)" nella Tabella pivot. |
| [getTextOfGrandTotal()](#getTextOfGrandTotal--) | Restituisce il testo dell'etichetta "Grand Total" nella Tabella pivot. |
| [getTextOfHours()](#getTextOfHours--) | Restituisce il testo locale di "Hours". |
| [getTextOfMinutes()](#getTextOfMinutes--) | Restituisce il testo locale di "Minutes". |
| [getTextOfMonths()](#getTextOfMonths--) | Restituisce il testo locale di "Months". |
| [getTextOfMultipleItems()](#getTextOfMultipleItems--) | Restituisce il testo dell'etichetta "(Multiple Items)" nella Tabella pivot. |
| [getTextOfOr()](#getTextOfOr--) | Restituisce tutte le stringhe formattate localmente di "or". |
| [getTextOfProtectedName(String protectedName)](#getTextOfProtectedName-java.lang.String-) | Restituisce il testo per il nome protetto specificato. |
| [getTextOfProtection()](#getTextOfProtection--) | Ottiene il nome della protezione nella tabella pivot. |
| [getTextOfQuarters()](#getTextOfQuarters--) | Restituisce il testo locale di "Quarters". |
| [getTextOfRange()](#getTextOfRange--) | Restituisce il testo locale di "Range" |
| [getTextOfRowLabels()](#getTextOfRowLabels--) | Restituisce il testo dell'etichetta "Row Labels" nella Tabella pivot. |
| [getTextOfSeconds()](#getTextOfSeconds--) | Restituisce il testo locale di "Seconds" |
| [getTextOfSubTotal(int subTotalType)](#getTextOfSubTotal-int-) | Restituisce il testo del tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) nella Tabella pivot. |
| [getTextOfTotal()](#getTextOfTotal--) | Restituisce il testo dell'etichetta "Total" nella Tabella pivot. |
| [getTextOfYears()](#getTextOfYears--) | Restituisce il testo locale di "Years". |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setTextOfAll(String text)](#setTextOfAll-java.lang.String-) | Imposta il testo dell'etichetta "(All)" nella PivotTable. |
| [setTextOfColumnLabels(String text)](#setTextOfColumnLabels-java.lang.String-) | Ottiene il testo dell\"Column Labels\" etichetta nella Tabella Pivot. |
| [setTextOfDataFieldHeader(String text)](#setTextOfDataFieldHeader-java.lang.String-) | Imposta il testo dell'intestazione del campo dell'area valori nella PivotTable. |
| [setTextOfEmptyData(String text)](#setTextOfEmptyData-java.lang.String-) | Imposta il testo dell'etichetta "(blank)" nella PivotTable. |
| [setTextOfGrandTotal(String text)](#setTextOfGrandTotal-java.lang.String-) | Imposta il testo dell'etichetta "Grand Total" nella PivotTable. |
| [setTextOfMultipleItems(String text)](#setTextOfMultipleItems-java.lang.String-) | Imposta il testo dell'etichetta "(Multiple Items)" nella PivotTable. |
| [setTextOfProtectedName(String protectedName, String text)](#setTextOfProtectedName-java.lang.String-java.lang.String-) | Imposta il testo per un nome protetto specifico. |
| [setTextOfRowLabels(String text)](#setTextOfRowLabels-java.lang.String-) | Imposta il testo dell'etichetta "Row Labels" nella Tabella pivot. |
| [setTextOfSubTotal(int subTotalType, String text)](#setTextOfSubTotal-int-java.lang.String-) | Imposta il testo del tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) nella Tabella pivot. |
| [setTextOfTotal(String text)](#setTextOfTotal-java.lang.String-) | Imposta il testo dell'etichetta "Total" nella Tabella pivot. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SettablePivotGlobalizationSettings() {#SettablePivotGlobalizationSettings--}
```
public SettablePivotGlobalizationSettings()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFormatOfDayGroup() {#getFormatOfDayGroup--}
```
public String getFormatOfDayGroup()
```


Restituisce il formato numerico del gruppo giorno della tabella pivot. Utilizzato solo quando si raggruppa il campo pivot per giorni. Il valore predefinito è "d-MMM";

**Returns:**
java.lang.String -
### getNameOfDataField(int function, String name) {#getNameOfDataField-int-java.lang.String-}
```
public String getNameOfDataField(int function, String name)
```


Restituisce il nome visualizzato del campo dati della tabella pivot. Il formato predefinito è "Sum Of Field".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). La funzione è usata per riepilogare i valori del campo pivot. |
| name | java.lang.String | Il nome originale del campo pivot. |

**Returns:**
java.lang.String -
### getShortTextOf12Months() {#getShortTextOf12Months--}
```
public String[] getShortTextOf12Months()
```


Ottiene tutte le stringhe formattate brevemente dei 12 mesi.

**Returns:**
java.lang.String[] -
### getTextOf24Hours() {#getTextOf24Hours--}
```
public String[] getTextOf24Hours()
```


Restituisce tutte le stringhe formattate localmente delle 24 ore. Il valore predefinito è 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM.

**Returns:**
java.lang.String[] -
### getTextOf4Quarters() {#getTextOf4Quarters--}
```
public String[] getTextOf4Quarters()
```


Ottiene il testo locale dei 4 trimestri.

**Remarks**

Restituisce di default Quarter1, Quarter2, Quarter3, Quarter4 prima della versione 26.9. Restituisce di default Qtr1, Qtr2, Qtr3, Qtr4 dalla versione 26.9.

**Returns:**
java.lang.String[] -
### getTextOf4Quaters() {#getTextOf4Quaters--}
```
public String[] getTextOf4Quaters()
```


Ottiene il testo locale dei 4 trimestri.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetTextOf4Quarters(). Questa proprietà sarà rimossa 12 mesi dopo a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Returns:**
java.lang.String[] -
### getTextOfAll() {#getTextOfAll--}
```
public String getTextOfAll()
```


Ottiene il testo dell\"(All)\" etichetta nella Tabella Pivot.

**Returns:**
java.lang.String - Il testo dell'etichetta "(All)"
### getTextOfAllPeriods() {#getTextOfAllPeriods--}
```
public String getTextOfAllPeriods()
```


Ottiene il testo localizzato di \"All Periods\".

**Returns:**
java.lang.String -
### getTextOfColumnLabels() {#getTextOfColumnLabels--}
```
public String getTextOfColumnLabels()
```


Ottiene il testo dell\"Column Labels\" etichetta nella Tabella Pivot.

**Returns:**
java.lang.String - Il testo delle etichette di colonna
### getTextOfDataFieldHeader() {#getTextOfDataFieldHeader--}
```
public String getTextOfDataFieldHeader()
```


Restituisce il testo dell'intestazione del campo area valore nella Tabella pivot.

**Returns:**
java.lang.String - Il testo del nome dell'intestazione del campo dati
### getTextOfDays() {#getTextOfDays--}
```
public String getTextOfDays()
```


Restituisce il testo locale di "Days".

**Returns:**
java.lang.String -
### getTextOfEmptyData() {#getTextOfEmptyData--}
```
public String getTextOfEmptyData()
```


Restituisce il testo dell'etichetta "(blank)" nella Tabella pivot.

**Returns:**
java.lang.String - Il testo dei dati vuoti
### getTextOfGrandTotal() {#getTextOfGrandTotal--}
```
public String getTextOfGrandTotal()
```


Restituisce il testo dell'etichetta "Grand Total" nella Tabella pivot.

**Returns:**
java.lang.String - Il testo dell'etichetta "Grand Total"
### getTextOfHours() {#getTextOfHours--}
```
public String getTextOfHours()
```


Restituisce il testo locale di "Hours".

**Returns:**
java.lang.String -
### getTextOfMinutes() {#getTextOfMinutes--}
```
public String getTextOfMinutes()
```


Restituisce il testo locale di "Minutes".

**Returns:**
java.lang.String -
### getTextOfMonths() {#getTextOfMonths--}
```
public String getTextOfMonths()
```


Restituisce il testo locale di "Months".

**Returns:**
java.lang.String -
### getTextOfMultipleItems() {#getTextOfMultipleItems--}
```
public String getTextOfMultipleItems()
```


Restituisce il testo dell'etichetta "(Multiple Items)" nella Tabella pivot.

**Returns:**
java.lang.String - Il testo dell'etichetta "(Multiple Items)"
### getTextOfOr() {#getTextOfOr--}
```
public String getTextOfOr()
```


Restituisce tutte le stringhe formattate localmente di "or".

**Returns:**
java.lang.String -
### getTextOfProtectedName(String protectedName) {#getTextOfProtectedName-java.lang.String-}
```
public String getTextOfProtectedName(String protectedName)
```


Restituisce il testo per il nome protetto specificato.

**Remarks**

In Ms Excel, alcuni nomi non possono essere usati come nome dei PivotField in una PivotTable. Sono diversi a seconda della regione; l'utente può specificarli esplicitamente in base alla regione utilizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| protectedName | java.lang.String | Il nome protetto nella PivotTable. |

**Returns:**
java.lang.String - I nomi protetti locali della PivotTable.
### getTextOfProtection() {#getTextOfProtection--}
```
public String getTextOfProtection()
```


Ottiene il nome della protezione nella tabella pivot.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo PivotGlobalizationSettings.GetTextOfProtectedName(string). Questa proprietà sarà rimossa 12 mesi dopo a partire da marzo 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Returns:**
java.lang.String - Il nome di protezione della PivotTable
### getTextOfQuarters() {#getTextOfQuarters--}
```
public String getTextOfQuarters()
```


Restituisce il testo locale di "Quarters".

**Returns:**
java.lang.String -
### getTextOfRange() {#getTextOfRange--}
```
public String getTextOfRange()
```


Restituisce il testo locale di "Range"

**Returns:**
java.lang.String -
### getTextOfRowLabels() {#getTextOfRowLabels--}
```
public String getTextOfRowLabels()
```


Restituisce il testo dell'etichetta "Row Labels" nella Tabella pivot.

**Returns:**
java.lang.String - Il testo delle etichette di riga
### getTextOfSeconds() {#getTextOfSeconds--}
```
public String getTextOfSeconds()
```


Restituisce il testo locale di "Seconds"

**Returns:**
java.lang.String -
### getTextOfSubTotal(int subTotalType) {#getTextOfSubTotal-int-}
```
public String getTextOfSubTotal(int subTotalType)
```


Restituisce il testo del tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) nella Tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Il [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - Il testo del tipo specificato
### getTextOfTotal() {#getTextOfTotal--}
```
public String getTextOfTotal()
```


Ottiene il testo dell'etichetta "Total" nella PivotTable. È necessario sovrascrivere questo metodo quando la PivotTable contiene due o più PivotField nell'area dati.

**Returns:**
java.lang.String - Il testo dell'etichetta "Total"
### getTextOfYears() {#getTextOfYears--}
```
public String getTextOfYears()
```


Restituisce il testo locale di "Years".

**Returns:**
java.lang.String -
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




### setTextOfAll(String text) {#setTextOfAll-java.lang.String-}
```
public void setTextOfAll(String text)
```


Imposta il testo dell'etichetta "(All)" nella PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | testo personalizzato |

### setTextOfColumnLabels(String text) {#setTextOfColumnLabels-java.lang.String-}
```
public void setTextOfColumnLabels(String text)
```


Ottiene il testo dell\"Column Labels\" etichetta nella Tabella Pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | Il testo delle etichette di colonna |

### setTextOfDataFieldHeader(String text) {#setTextOfDataFieldHeader-java.lang.String-}
```
public void setTextOfDataFieldHeader(String text)
```


Imposta il testo dell'intestazione del campo dell'area valori nella PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | Il testo del nome dell'intestazione del campo dati |

### setTextOfEmptyData(String text) {#setTextOfEmptyData-java.lang.String-}
```
public void setTextOfEmptyData(String text)
```


Imposta il testo dell'etichetta "(blank)" nella PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | Il testo dei dati vuoti |

### setTextOfGrandTotal(String text) {#setTextOfGrandTotal-java.lang.String-}
```
public void setTextOfGrandTotal(String text)
```


Imposta il testo dell'etichetta "Grand Total" nella PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | testo personalizzato |

### setTextOfMultipleItems(String text) {#setTextOfMultipleItems-java.lang.String-}
```
public void setTextOfMultipleItems(String text)
```


Imposta il testo dell'etichetta "(Multiple Items)" nella PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | testo personalizzato |

### setTextOfProtectedName(String protectedName, String text) {#setTextOfProtectedName-java.lang.String-java.lang.String-}
```
public void setTextOfProtectedName(String protectedName, String text)
```


Imposta il testo per un nome protetto specifico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| protectedName | java.lang.String | Il nome protetto nella PivotTable. |
| testo | java.lang.String | I nomi protetti locali della Tabella pivot. |

### setTextOfRowLabels(String text) {#setTextOfRowLabels-java.lang.String-}
```
public void setTextOfRowLabels(String text)
```


Imposta il testo dell'etichetta "Row Labels" nella Tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | Il testo delle etichette di riga |

### setTextOfSubTotal(int subTotalType, String text) {#setTextOfSubTotal-int-java.lang.String-}
```
public void setTextOfSubTotal(int subTotalType, String text)
```


Imposta il testo del tipo [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) nella Tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Il [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| testo | java.lang.String | Il testo del tipo specificato |

### setTextOfTotal(String text) {#setTextOfTotal-java.lang.String-}
```
public void setTextOfTotal(String text)
```


Imposta il testo dell'etichetta "Total" nella Tabella pivot.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | java.lang.String | testo personalizzato |

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

