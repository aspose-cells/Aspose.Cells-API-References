---
title: "AutoFiltro"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta l'autofiltraggio per il foglio di lavoro specificato."
type: docs
url: /it/java/com.aspose.cells/autofilter/
---

**Inheritance:**
java.lang.Object
```
public class AutoFilter
```

Rappresenta l'autofiltraggio per il foglio di lavoro specificato.

**Example**

```
         //Creating a file stream containing the Excel file to be opened
         //Instantiating a Workbook object
         Workbook workbook = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating AutoFilter by giving the cells range of the heading row
         worksheet.getAutoFilter().setRange("A1:B1");
         //Filtering columns with specified values
         worksheet.getAutoFilter().filter(1, "Bananas");
         //Saving the modified Excel file.
         workbook.save("output.xls");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#addDateFilter-int-int-int-int-int-int-int-int-) | Aggiunge un filtro data. |
| [addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)](#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-) | Aggiunge un filtro colore di riempimento. |
| [addFilter(int fieldIndex, String criteria)](#addFilter-int-java.lang.String-) | Aggiunge un filtro per una colonna filtro. |
| [addFontColorFilter(int fieldIndex, CellsColor color)](#addFontColorFilter-int-com.aspose.cells.CellsColor-) | Aggiunge un filtro colore carattere. |
| [addIconFilter(int fieldIndex, int iconSetType, int iconId)](#addIconFilter-int-int-int-) | Aggiunge un filtro icona. |
| [custom(int fieldIndex, int operatorType1, Object criteria1)](#custom-int-int-java.lang.Object-) | Filtra un elenco con un criterio personalizzato. |
| [custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-) | Filtra un elenco con criteri personalizzati. |
| [dynamicFilter(int fieldIndex, int dynamicFilterType)](#dynamicFilter-int-int-) | Aggiunge un filtro dinamico. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int fieldIndex, String criteria)](#filter-int-java.lang.String-) | Filtra un elenco con criteri specificati. |
| [filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)](#filterTop10-int-boolean-boolean-int-) | Filtra i primi 10 elementi nell'elenco |
| [getCellArea()](#getCellArea--) | Ottiene il [CellArea](../../com.aspose.cells/cellarea) a cui si applica questo AutoFiltro. |
| [getCellArea(boolean refreshAppliedRange)](#getCellArea-boolean-) | Ottiene il [CellArea](../../com.aspose.cells/cellarea) a cui si applica l'AutoFiltro specificato. |
| [getClass()](#getClass--) |  |
| [getFilterColumns()](#getFilterColumns--) | Ottiene la raccolta delle colonne filtro. |
| [getRange()](#getRange--) | Rappresenta l'intervallo a cui si applica l'AutoFiltro specificato. |
| [getShowFilterButton()](#getShowFilterButton--) | Indica se il pulsante AutoFilter per questa colonna è visibile. |
| [getSorter()](#getSorter--) | Ottiene l'ordinatore dei dati. |
| [hashCode()](#hashCode--) |  |
| [matchBlanks(int fieldIndex)](#matchBlanks-int-) | Corrisponde a tutte le celle vuote nell'elenco. |
| [matchNonBlanks(int fieldIndex)](#matchNonBlanks-int-) | Corrisponde a tutte le celle non vuote nell'elenco. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Aggiorna gli auto filtri per nascondere o mostrare le righe. |
| [refresh(boolean hideRows)](#refresh-boolean-) | Ottiene tutti gli indici delle righe nascoste. |
| [removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#removeDateFilter-int-int-int-int-int-int-int-int-) | Rimuove un filtro data. |
| [removeFilter(int fieldIndex)](#removeFilter-int-) | Rimuove il filtro specifico. |
| [removeFilter(int fieldIndex, String criteria)](#removeFilter-int-java.lang.String-) | Rimuove un filtro per una colonna filtro. |
| [setRange(int row, int startColumn, int endColumn)](#setRange-int-int-int-) | Imposta l'intervallo a cui si applica l'AutoFiltro specificato. |
| [setRange(String value)](#setRange-java.lang.String-) | Rappresenta l'intervallo a cui si applica l'AutoFiltro specificato. |
| [setShowFilterButton(boolean value)](#setShowFilterButton-boolean-) | Indica se il pulsante AutoFilter per questa colonna è visibile. |
| [showAll()](#showAll--) | Mostra tutte le righe. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#addDateFilter-int-int-int-int-int-int-int-int-}
```
public void addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Aggiunge un filtro data.

**Remarks**

Se DateTimeGroupingType è Year, solo il parametro year ha effetto. Se DateTiemGroupingType è Month, solo i parametri year e month hanno effetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Il tipo di raggruppamento |
| anno | int | L'anno. |
| mese | int | Il mese. |
| giorno | int | Il giorno. |
| ora | int | L'ora. |
| minuto | int | Il minuto. |
| secondo | int | Il secondo. |

### addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor) {#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-}
```
public void addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)
```


Aggiunge un filtro colore di riempimento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). Il tipo di motivo di sfondo. |
| foregroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | Il colore di primo piano. |
| backgroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | Il colore di sfondo. |

### addFilter(int fieldIndex, String criteria) {#addFilter-int-java.lang.String-}
```
public void addFilter(int fieldIndex, String criteria)
```


Aggiunge un filtro per una colonna filtro.

**Remarks**

MS Excel 2007 supporta la selezione multipla in una colonna di filtro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |
| criteri | java.lang.String | Il criterio specificato (una stringa; ad esempio, "101"). Può essere solo null o uno dei valori delle celle in questa colonna. |

### addFontColorFilter(int fieldIndex, CellsColor color) {#addFontColorFilter-int-com.aspose.cells.CellsColor-}
```
public void addFontColorFilter(int fieldIndex, CellsColor color)
```


Aggiunge un filtro colore carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |
| color | [CellsColor](../../com.aspose.cells/cellscolor) | L'oggetto [CellsColor](../../com.aspose.cells/cellscolor). |

### addIconFilter(int fieldIndex, int iconSetType, int iconId) {#addIconFilter-int-int-int-}
```
public void addIconFilter(int fieldIndex, int iconSetType, int iconId)
```


Aggiunge un filtro icona.

**Remarks**

Supporta solo l'aggiunta del filtro icona. Non supporta il controllo di quale riga sia visibile se il filtro è un filtro icona.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |
| iconSetType | int | [IconSetType](../../com.aspose.cells/iconsettype). Il tipo di set di icone. |
| iconId | int | L'ID dell'icona. |

### custom(int fieldIndex, int operatorType1, Object criteria1) {#custom-int-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1)
```


Filtra un elenco con un criterio personalizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Il tipo di operatore di filtro |
| criteria1 | java.lang.Object | Il criterio personalizzato |

### custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


Filtra un elenco con criteri personalizzati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Il tipo di operatore di filtro |
| criteria1 | java.lang.Object | Il criterio personalizzato |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Il tipo di operatore di filtro |
| criteria2 | java.lang.Object | Il criterio personalizzato |

### dynamicFilter(int fieldIndex, int dynamicFilterType) {#dynamicFilter-int-int-}
```
public void dynamicFilter(int fieldIndex, int dynamicFilterType)
```


Aggiunge un filtro dinamico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |
| dynamicFilterType | int | [DynamicFilterType](../../com.aspose.cells/dynamicfiltertype). Tipo di filtro dinamico. |

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
### filter(int fieldIndex, String criteria) {#filter-int-java.lang.String-}
```
public void filter(int fieldIndex, String criteria)
```


Filtra un elenco con criteri specificati.

**Remarks**

Aspose.Cells rimuoverà tutte le altre impostazioni di filtro su questo campo come in MS Excel 97-2003.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |
| criteri | java.lang.String | Il criterio specificato (una stringa; ad esempio, "101"). |

### filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount) {#filterTop10-int-boolean-boolean-int-}
```
public void filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)
```


Filtra i primi 10 elementi nell'elenco

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |
| isTop | boolean | Indica se il filtro è dal superiore o dal inferiore |
| isPercent | boolean | Indica se gli elementi sono percentuale o conteggio |
| itemCount | int | Il numero di elementi |

### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Ottiene il [CellArea](../../com.aspose.cells/cellarea) a cui si applica questo AutoFiltro.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getCellArea(boolean refreshAppliedRange) {#getCellArea-boolean-}
```
public CellArea getCellArea(boolean refreshAppliedRange)
```


Ottiene il [CellArea](../../com.aspose.cells/cellarea) a cui si applica l'AutoFiltro specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| refreshAppliedRange | boolean | Indica se aggiornare l'intervallo applicato. Per l'intervallo applicato del filtro automatico, l'ultima riga può cambiare quando i dati delle celle cambiano. Se questo flag è true, allora l'ultima riga dell'intervallo verrà ricalcolata in base ai dati attuali delle celle. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilterColumns() {#getFilterColumns--}
```
public FilterColumnCollection getFilterColumns()
```


Ottiene la raccolta delle colonne filtro.

**Returns:**
[FilterColumnCollection](../../com.aspose.cells/filtercolumncollection)
### getRange() {#getRange--}
```
public String getRange()
```


Rappresenta l'intervallo a cui si applica l'AutoFiltro specificato.

**Returns:**
java.lang.String
### getShowFilterButton() {#getShowFilterButton--}
```
public boolean getShowFilterButton()
```


Indica se il pulsante AutoFilter per questa colonna è visibile.

**Returns:**
boolean
### getSorter() {#getSorter--}
```
public DataSorter getSorter()
```


Ottiene l'ordinatore dei dati.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### matchBlanks(int fieldIndex) {#matchBlanks-int-}
```
public void matchBlanks(int fieldIndex)
```


Corrisponde a tutte le celle vuote nell'elenco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |

### matchNonBlanks(int fieldIndex) {#matchNonBlanks-int-}
```
public void matchNonBlanks(int fieldIndex)
```


Corrisponde a tutte le celle non vuote nell'elenco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int[] refresh()
```


Aggiorna gli auto filtri per nascondere o mostrare le righe.

**Returns:**
int[] - Restituisce tutti gli indici delle righe nascoste.
### refresh(boolean hideRows) {#refresh-boolean-}
```
public int[] refresh(boolean hideRows)
```


Ottiene tutti gli indici delle righe nascoste.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| hideRows | boolean | Se true, nascondi le righe filtrate. |

**Returns:**
int[] - Restituisce tutti gli indici delle righe nascoste.
### removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#removeDateFilter-int-int-int-int-int-int-int-int-}
```
public void removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Rimuove un filtro data.

**Remarks**

Se DateTimeGroupingType è Year, solo il parametro year ha effetto. Se DateTiemGroupingType è Month, solo i parametri year e month hanno effetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Il tipo di raggruppamento |
| anno | int | L'anno. |
| mese | int | Il mese. |
| giorno | int | Il giorno. |
| ora | int | L'ora. |
| minuto | int | Il minuto. |
| secondo | int | Il secondo. |

### removeFilter(int fieldIndex) {#removeFilter-int-}
```
public void removeFilter(int fieldIndex)
```


Rimuove il filtro specifico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'indice del filtro specifico |

### removeFilter(int fieldIndex, String criteria) {#removeFilter-int-java.lang.String-}
```
public void removeFilter(int fieldIndex, String criteria)
```


Rimuove un filtro per una colonna filtro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int | L'offset intero del campo su cui vuoi basare il filtro (da sinistra della lista; il campo più a sinistra è il campo 0). |
| criteri | java.lang.String | Il criterio specificato (una stringa; ad esempio, "101"). Può essere solo null o uno dei valori delle celle in questa colonna. |

### setRange(int row, int startColumn, int endColumn) {#setRange-int-int-int-}
```
public void setRange(int row, int startColumn, int endColumn)
```


Imposta l'intervallo a cui si applica l'AutoFiltro specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| startColumn | int | Indice della colonna di inizio. |
| endColumn | int | Indice della colonna finale. |

### setRange(String value) {#setRange-java.lang.String-}
```
public void setRange(String value)
```


Rappresenta l'intervallo a cui si applica l'AutoFiltro specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setShowFilterButton(boolean value) {#setShowFilterButton-boolean-}
```
public void setShowFilterButton(boolean value)
```


Indica se il pulsante AutoFilter per questa colonna è visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### showAll() {#showAll--}
```
public void showAll()
```


Mostra tutte le righe.

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

