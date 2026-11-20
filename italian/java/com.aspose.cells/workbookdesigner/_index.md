---
title: "WorkbookDesigner"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta un foglio di calcolo del designer."
type: docs
url: /it/java/com.aspose.cells/workbookdesigner/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookDesigner
```

Incapsula l'oggetto che rappresenta un foglio di calcolo del designer.

**Example**

```
         //Create WorkbookDesigner object.
         WorkbookDesigner wd = new WorkbookDesigner();
         //Open the template file (which contains smart markers).
         wd.setWorkbook(new Workbook("SmartMarker_Designer.xls"));
 
         //Initialize your data from data source
         //DataSet ds = new DataSet();
 
 
         //Set the datatable as the data source.
         //wd.SetDataSource(dt);
         //Process the smart markers to fill the data into the worksheets.
         wd.process(true);
         //Save the excel file.
         wd.getWorkbook().save("outSmartMarker_Designer.xls");
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [WorkbookDesigner()](#WorkbookDesigner--) | Inizializza una nuova istanza della classe [WorkbookDesigner](../../com.aspose.cells/workbookdesigner). |
| [WorkbookDesigner(Workbook workbook)](#WorkbookDesigner-com.aspose.cells.Workbook-) | Inizializza una nuova istanza della classe [WorkbookDesigner](../../com.aspose.cells/workbookdesigner). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [clearDataSource()](#clearDataSource--) | Cancella tutte le origini dati. |
| [containsVariables()](#containsVariables--) | Indica se il primo foglio di lavoro contiene variabili personalizzate. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateFormula()](#getCalculateFormula--) | Indica se le formule devono essere calcolate. |
| [getCallBack()](#getCallBack--) | Ottiene l'interfaccia di callback dell'elaborazione di smartmarker. |
| [getClass()](#getClass--) |  |
| [getEnableHeaderFooterMarkers()](#getEnableHeaderFooterMarkers--) | Indica se l'intestazione/piè di pagina contiene smart marker e deve essere elaborata insieme. |
| [getLineByLine()](#getLineByLine--) | Indica se l'elaborazione dello smart marker avviene riga per riga. |
| [getRepeatFormulasWithSubtotal()](#getRepeatFormulasWithSubtotal--) | Indica se le formule ripetute includono una riga di subtotale. |
| [getSmartMarkers()](#getSmartMarkers--) | Restituisce una raccolta di smart marker in un foglio di calcolo. |
| [getSortDataSource()](#getSortDataSource--) | Indica se ordinare l'origine dati. |
| [getUpdateEmptyStringAsNull()](#getUpdateEmptyStringAsNull--) | Se TRUE, Null verrà inserito se il valore è ""; |
| [getUpdateReference()](#getUpdateReference--) | Indica se i riferimenti in altri fogli di lavoro saranno aggiornati. |
| [getVariablesWorksheetName()](#getVariablesWorksheetName--) | Ottiene il nome del foglio di lavoro che contiene lo smart marker variabile. |
| [getWorkbook()](#getWorkbook--) | Ottiene l'oggetto [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process()](#process--) | Elabora gli smart marker e popola i valori dell'origine dati. |
| [process(boolean isPreserved)](#process-boolean-) | Elabora gli smart marker e popola i valori dell'origine dati. |
| [process(Range range, boolean isPreserved)](#process-com.aspose.cells.Range-boolean-) | Elabora gli smart marker e popola i valori dell'origine dati. |
| [process(int sheetIndex, boolean isPreserved)](#process-int-boolean-) | Elabora gli smart marker e popola i valori dell'origine dati. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indica se le formule devono essere calcolate. |
| [setCallBack(ISmartMarkerCallBack value)](#setCallBack-com.aspose.cells.ISmartMarkerCallBack-) | Imposta l'interfaccia di callback per l'elaborazione dello smartmarker. |
| [setContainsVariables(boolean value)](#setContainsVariables-boolean-) | Indica se il primo foglio di lavoro contiene variabili personalizzate. |
| [setDataSource(String dataSource, ICellsDataTable cellsDataTable)](#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-) | Imposta l'origine dati di un oggetto [ICellsDataTable](../../com.aspose.cells/icellsdatatable). |
| [setDataSource(String variable, Object data)](#setDataSource-java.lang.String-java.lang.Object-) | Imposta il binding dei dati a una variabile. |
| [setDataSource(String dataSource, ResultSet rs)](#setDataSource-java.lang.String-java.sql.ResultSet-) | Imposta l'origine dati. |
| [setDataSource(String dataSource, ResultSet rs, int rowCount)](#setDataSource-java.lang.String-java.sql.ResultSet-int-) | Imposta l'origine dati. |
| [setDataSource(ResultSet rs)](#setDataSource-java.sql.ResultSet-) | Imposta l'origine dati. |
| [setEnableHeaderFooterMarkers(boolean value)](#setEnableHeaderFooterMarkers-boolean-) | Indica se l'intestazione/piè di pagina contiene smart marker e deve essere elaborata insieme. |
| [setJsonDataSource(String name, String json)](#setJsonDataSource-java.lang.String-java.lang.String-) | Imposta il valore della stringa JSON come origine dati degli smart marker. |
| [setLineByLine(boolean value)](#setLineByLine-boolean-) | Indica se l'elaborazione dello smart marker avviene riga per riga. |
| [setRepeatFormulasWithSubtotal(boolean value)](#setRepeatFormulasWithSubtotal-boolean-) | Indica se le formule ripetute includono una riga di subtotale. |
| [setSortDataSource(boolean value)](#setSortDataSource-boolean-) | Indica se ordinare l'origine dati. |
| [setUpdateEmptyStringAsNull(boolean value)](#setUpdateEmptyStringAsNull-boolean-) | Se TRUE, Null verrà inserito se il valore è ""; |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Indica se i riferimenti in altri fogli di lavoro saranno aggiornati. |
| [setVariablesWorksheetName(String value)](#setVariablesWorksheetName-java.lang.String-) | Imposta il nome del foglio di lavoro che contiene lo smart marker variabile. |
| [setWorkbook(Workbook value)](#setWorkbook-com.aspose.cells.Workbook-) | Imposta l'oggetto [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookDesigner() {#WorkbookDesigner--}
```
public WorkbookDesigner()
```


Inizializza una nuova istanza della classe [WorkbookDesigner](../../com.aspose.cells/workbookdesigner).

### WorkbookDesigner(Workbook workbook) {#WorkbookDesigner-com.aspose.cells.Workbook-}
```
public WorkbookDesigner(Workbook workbook)
```


Inizializza una nuova istanza della classe [WorkbookDesigner](../../com.aspose.cells/workbookdesigner).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Il file del workbook modello. |

### clearDataSource() {#clearDataSource--}
```
public void clearDataSource()
```


Cancella tutte le origini dati.

### containsVariables() {#containsVariables--}
```
public boolean containsVariables()
```


Indica se il primo foglio di lavoro contiene variabili personalizzate.

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà WorkbookDesigner.VariablesWorksheetName. Questa proprietà sarà rimossa tra 3 mesi a partire da settembre 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
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
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Indica se le formule devono essere calcolate.

**Returns:**
boolean
### getCallBack() {#getCallBack--}
```
public ISmartMarkerCallBack getCallBack()
```


Ottiene l'interfaccia di callback dell'elaborazione di smartmarker.

**Returns:**
[ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableHeaderFooterMarkers() {#getEnableHeaderFooterMarkers--}
```
public boolean getEnableHeaderFooterMarkers()
```


Indica se l'intestazione/piè di pagina contiene smart marker e deve essere elaborata insieme.

**Returns:**
boolean
### getLineByLine() {#getLineByLine--}
```
public boolean getLineByLine()
```


Indica se l'elaborazione dello smart marker avviene riga per riga.

**Remarks**

NOTE: Questa classe è ora obsoleta. Invece, si prega di utilizzare gli smart marker di intervallo. Questa proprietà sarà rimossa tra 12 mesi a partire da luglio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### getRepeatFormulasWithSubtotal() {#getRepeatFormulasWithSubtotal--}
```
public boolean getRepeatFormulasWithSubtotal()
```


Indica se le formule ripetute includono una riga di subtotale.

**Returns:**
boolean
### getSmartMarkers() {#getSmartMarkers--}
```
public String[] getSmartMarkers()
```


Restituisce una raccolta di smart marker in un foglio di calcolo.

**Remarks**

Un array di stringhe viene creato ad ogni chiamata. L'array è ordinato e i valori duplicati vengono rimossi.

**Returns:**
java.lang.String[] - Una raccolta di smart marker
### getSortDataSource() {#getSortDataSource--}
```
public boolean getSortDataSource()
```


Indica se ordinare l'origine dati.

**Remarks**

NOTE: Questa proprietà è ora obsoleta. Questa proprietà sarà rimossa tra 12 mesi a partire da ottobre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato. L'origine dati JSON verrà ordinata se lo smart marker contiene parametri di ordinamento ascendente e discendente.

**Returns:**
boolean
### getUpdateEmptyStringAsNull() {#getUpdateEmptyStringAsNull--}
```
public boolean getUpdateEmptyStringAsNull()
```


Se TRUE, Null verrà inserito se il valore è "";

**Returns:**
boolean
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Indica se i riferimenti in altri fogli di lavoro saranno aggiornati.

**Returns:**
boolean
### getVariablesWorksheetName() {#getVariablesWorksheetName--}
```
public String getVariablesWorksheetName()
```


Ottiene il nome del foglio di lavoro che contiene lo smart marker variabile.

**Returns:**
java.lang.String
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Ottiene l'oggetto [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--).

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
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




### process() {#process--}
```
public void process()
```


Elabora gli smart marker e popola i valori dell'origine dati.

### process(boolean isPreserved) {#process-boolean-}
```
public void process(boolean isPreserved)
```


Elabora gli smart marker e popola i valori dell'origine dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isPreserved | boolean | True se lo smart marker non riconosciuto è preservato. |

### process(Range range, boolean isPreserved) {#process-com.aspose.cells.Range-boolean-}
```
public void process(Range range, boolean isPreserved)
```


Elabora gli smart marker e popola i valori dell'origine dati.

**Remarks**

NOTE: Questa classe è ora obsoleta. Invece, si prega di utilizzare gli smart marker Range. Questa proprietà sarà rimossa tra 12 mesi a partire da luglio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | L'intervallo da elaborare |
| isPreserved | boolean | True se lo smart marker non riconosciuto è preservato. |

### process(int sheetIndex, boolean isPreserved) {#process-int-boolean-}
```
public void process(int sheetIndex, boolean isPreserved)
```


Elabora gli smart marker e popola i valori dell'origine dati.

**Remarks**

Questo metodo funziona a livello di foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | int | Indice del foglio di lavoro. |
| isPreserved | boolean | True se lo smart marker non riconosciuto è preservato. |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Indica se le formule devono essere calcolate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCallBack(ISmartMarkerCallBack value) {#setCallBack-com.aspose.cells.ISmartMarkerCallBack-}
```
public void setCallBack(ISmartMarkerCallBack value)
```


Imposta l'interfaccia di callback per l'elaborazione dello smartmarker.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback) |  |

### setContainsVariables(boolean value) {#setContainsVariables-boolean-}
```
public void setContainsVariables(boolean value)
```


Indica se il primo foglio di lavoro contiene variabili personalizzate.

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà WorkbookDesigner.VariablesWorksheetName. Questa proprietà sarà rimossa tra 3 mesi a partire da settembre 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDataSource(String dataSource, ICellsDataTable cellsDataTable) {#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-}
```
public void setDataSource(String dataSource, ICellsDataTable cellsDataTable)
```


Imposta l'origine dati di un oggetto [ICellsDataTable](../../com.aspose.cells/icellsdatatable).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataSource | java.lang.String | Il nome dell'origine dati. |
| cellsDataTable | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | tabella dati. |

### setDataSource(String variable, Object data) {#setDataSource-java.lang.String-java.lang.Object-}
```
public void setDataSource(String variable, Object data)
```


Imposta il binding dei dati a una variabile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| variabile | java.lang.String | Nome della variabile creato usando lo smart marker. |
| dati | java.lang.Object | Dati di origine. |

### setDataSource(String dataSource, ResultSet rs) {#setDataSource-java.lang.String-java.sql.ResultSet-}
```
public void setDataSource(String dataSource, ResultSet rs)
```


Imposta l'origine dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataSource | java.lang.String | Il nome dell'origine dati. |
| rs | java.sql.ResultSet | Il set di risultati. |

### setDataSource(String dataSource, ResultSet rs, int rowCount) {#setDataSource-java.lang.String-java.sql.ResultSet-int-}
```
public void setDataSource(String dataSource, ResultSet rs, int rowCount)
```


Imposta l'origine dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataSource | java.lang.String | Il nome dell'origine dati. |
| rs | java.sql.ResultSet | Il set di risultati. |
| rowCount | int | Il conteggio dei dati del resultset fornito. Deve essere il conteggio esatto delle righe o -1; se il resultset è solo in avanti, l'utente deve fornire qui il conteggio esatto delle righe, altrimenti lo smart potrebbe non essere elaborato correttamente quando il \"noadd\" dello smart marker non è impostato. |

### setDataSource(ResultSet rs) {#setDataSource-java.sql.ResultSet-}
```
public void setDataSource(ResultSet rs)
```


Imposta l'origine dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rs | java.sql.ResultSet | Il set di risultati. |

### setEnableHeaderFooterMarkers(boolean value) {#setEnableHeaderFooterMarkers-boolean-}
```
public void setEnableHeaderFooterMarkers(boolean value)
```


Indica se l'intestazione/piè di pagina contiene smart marker e deve essere elaborata insieme.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setJsonDataSource(String name, String json) {#setJsonDataSource-java.lang.String-java.lang.String-}
```
public void setJsonDataSource(String name, String json)
```


Imposta il valore della stringa JSON come origine dati degli smart marker.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della tabella. Se il valore del JSON rappresenta un oggetto, potrebbe essere null. |
| json | java.lang.String | Il valore della stringa Json. |

### setLineByLine(boolean value) {#setLineByLine-boolean-}
```
public void setLineByLine(boolean value)
```


Indica se l'elaborazione dello smart marker avviene riga per riga.

**Remarks**

NOTE: Questa classe è ora obsoleta. Invece, si prega di utilizzare gli smart marker di intervallo. Questa proprietà sarà rimossa tra 12 mesi a partire da luglio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRepeatFormulasWithSubtotal(boolean value) {#setRepeatFormulasWithSubtotal-boolean-}
```
public void setRepeatFormulasWithSubtotal(boolean value)
```


Indica se le formule ripetute includono una riga di subtotale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSortDataSource(boolean value) {#setSortDataSource-boolean-}
```
public void setSortDataSource(boolean value)
```


Indica se ordinare l'origine dati.

**Remarks**

NOTE: Questa proprietà è ora obsoleta. Questa proprietà sarà rimossa tra 12 mesi a partire da ottobre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato. L'origine dati JSON verrà ordinata se lo smart marker contiene parametri di ordinamento ascendente e discendente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setUpdateEmptyStringAsNull(boolean value) {#setUpdateEmptyStringAsNull-boolean-}
```
public void setUpdateEmptyStringAsNull(boolean value)
```


Se TRUE, Null verrà inserito se il valore è "";

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Indica se i riferimenti in altri fogli di lavoro saranno aggiornati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setVariablesWorksheetName(String value) {#setVariablesWorksheetName-java.lang.String-}
```
public void setVariablesWorksheetName(String value)
```


Imposta il nome del foglio di lavoro che contiene lo smart marker variabile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setWorkbook(Workbook value) {#setWorkbook-com.aspose.cells.Workbook-}
```
public void setWorkbook(Workbook value)
```


Imposta l'oggetto [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Workbook](../../com.aspose.cells/workbook) |  |

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

