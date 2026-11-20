---
title: "ListObject"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta una tabella in un foglio di lavoro."
type: docs
url: /it/java/com.aspose.cells/listobject/
---

**Inheritance:**
java.lang.Object
```
public class ListObject
```

Rappresenta una tabella in un foglio di lavoro.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         table.getListColumns().get(4).setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         workbook.save("Book1.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [applyStyleToRange()](#applyStyleToRange--) | Applica lo stile della tabella all'intervallo. |
| [convertToRange()](#convertToRange--) | Converti la tabella in intervallo. |
| [convertToRange(TableToRangeOptions options)](#convertToRange-com.aspose.cells.TableToRangeOptions-) | Converti la tabella in intervallo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter()](#filter--) | Filtra la tabella. |
| [getAlternativeDescription()](#getAlternativeDescription--) | Ottiene la descrizione alternativa. |
| [getAlternativeText()](#getAlternativeText--) | Ottiene il testo alternativo. |
| [getAutoFilter()](#getAutoFilter--) | Ottiene il filtro automatico di questa tabella. |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Ottiene il commento della tabella. |
| [getDataRange()](#getDataRange--) | Ottiene l'intervallo dati della tabella. |
| [getDataSourceType()](#getDataSourceType--) | Ottiene il tipo di origine dati della tabella. |
| [getDisplayName()](#getDisplayName--) | Ottiene il nome visualizzato della tabella. |
| [getEndColumn()](#getEndColumn--) | Restituisce la colonna finale dell'intervallo. |
| [getEndRow()](#getEndRow--) | Restituisce la riga finale dell'intervallo. |
| [getListColumns()](#getListColumns--) | Restituisce l'elenco [ListColumn](../../com.aspose.cells/listcolumn) di questa tabella. |
| [getQueryTable()](#getQueryTable--) | Restituisce la QueryTable collegata. |
| [getShowHeaderRow()](#getShowHeaderRow--) | Restituisce se questa Table mostra la riga di intestazione. |
| [getShowTableStyleColumnStripes()](#getShowTableStyleColumnStripes--) | Indica se la formattazione a strisce di colonna è applicata. |
| [getShowTableStyleFirstColumn()](#getShowTableStyleFirstColumn--) | Indica se la prima colonna nella tabella è lo stile applicato. |
| [getShowTableStyleLastColumn()](#getShowTableStyleLastColumn--) | Indica se l'ultima colonna nella tabella è lo stile applicato. |
| [getShowTableStyleRowStripes()](#getShowTableStyleRowStripes--) | Indica se la formattazione a strisce di riga è applicata. |
| [getShowTotals()](#getShowTotals--) | Restituisce se questa TAble mostra la riga totale. |
| [getStartColumn()](#getStartColumn--) | Restituisce la colonna iniziale dell'intervallo. |
| [getStartRow()](#getStartRow--) | Restituisce la riga iniziale dell'intervallo. |
| [getTableStyleName()](#getTableStyleName--) | Restituisce il nome dello stile della tabella. |
| [getTableStyleType()](#getTableStyleType--) | Restituisce lo stile di tabella incorporato. |
| [getXmlMap()](#getXmlMap--) | Restituisce un [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) utilizzato per questo elenco. |
| [hasAutoFilter()](#hasAutoFilter--) | Indica se il filtro automatico è applicato a questa tabella. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putCellFormula(int rowOffset, int columnOffset, String formula)](#putCellFormula-int-int-java.lang.String-) | Inserisci la formula nella cella della tabella. |
| [putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)](#putCellFormula-int-int-java.lang.String-boolean-) | Inserisci la formula nella cella della tabella. |
| [putCellValue(int rowOffset, int columnOffset, Object value)](#putCellValue-int-int-java.lang.Object-) | Inserisci il valore nella cella. |
| [putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)](#putCellValue-int-int-java.lang.Object-boolean-) | Inserisci il valore nella cella. |
| [removeAutoFilter()](#removeAutoFilter--) | Rimuove il filtro automatico applicato a questa tabella. |
| [resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#resize-int-int-int-int-boolean-) | Ridimensiona l'intervallo dell'oggetto elenco. |
| [setAlternativeDescription(String value)](#setAlternativeDescription-java.lang.String-) | Imposta la descrizione alternativa. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Imposta il testo alternativo. |
| [setComment(String value)](#setComment-java.lang.String-) | Imposta il commento della tabella. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Imposta il nome visualizzato della tabella. |
| [setHasAutoFilter(boolean value)](#setHasAutoFilter-boolean-) | Indica se il filtro automatico è applicato a questa tabella. |
| [setShowHeaderRow(boolean value)](#setShowHeaderRow-boolean-) | Imposta se questa Table mostra la riga di intestazione. |
| [setShowTableStyleColumnStripes(boolean value)](#setShowTableStyleColumnStripes-boolean-) | Indica se la formattazione a strisce di colonna è applicata. |
| [setShowTableStyleFirstColumn(boolean value)](#setShowTableStyleFirstColumn-boolean-) | Indica se la prima colonna nella tabella è lo stile applicato. |
| [setShowTableStyleLastColumn(boolean value)](#setShowTableStyleLastColumn-boolean-) | Indica se l'ultima colonna nella tabella è lo stile applicato. |
| [setShowTableStyleRowStripes(boolean value)](#setShowTableStyleRowStripes-boolean-) | Indica se la formattazione a strisce di riga è applicata. |
| [setShowTotals(boolean value)](#setShowTotals-boolean-) | Imposta se questa TAble mostra la riga totale. |
| [setTableStyleName(String value)](#setTableStyleName-java.lang.String-) | Imposta il nome dello stile della tabella. |
| [setTableStyleType(int value)](#setTableStyleType-int-) | Restituisce lo stile di tabella incorporato. |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | Aggiorna i nomi di tutte le colonne dell'elenco nelle celle della tabella. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyleToRange() {#applyStyleToRange--}
```
public void applyStyleToRange()
```


Applica lo stile della tabella all'intervallo.

### convertToRange() {#convertToRange--}
```
public void convertToRange()
```


Converti la tabella in intervallo.

### convertToRange(TableToRangeOptions options) {#convertToRange-com.aspose.cells.TableToRangeOptions-}
```
public void convertToRange(TableToRangeOptions options)
```


Converti la tabella in intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | [TableToRangeOptions](../../com.aspose.cells/tabletorangeoptions) | le opzioni quando si converte la tabella in un intervallo. |

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
### filter() {#filter--}
```
public AutoFilter filter()
```


Filtra la tabella.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, impostare la proprietà ListObject.HasAutoFilter./// Questa proprietà sarà rimossa 12 mesi dopo, a partire da ottobre 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getAlternativeDescription() {#getAlternativeDescription--}
```
public String getAlternativeDescription()
```


Ottiene la descrizione alternativa.

**Returns:**
java.lang.String
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Ottiene il testo alternativo.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Ottiene il filtro automatico di questa tabella.

**Remarks**

Funziona solo quando [hasAutoFilter()](../../com.aspose.cells/listobject\#hasAutoFilter--) è false.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComment() {#getComment--}
```
public String getComment()
```


Ottiene il commento della tabella.

**Returns:**
java.lang.String
### getDataRange() {#getDataRange--}
```
public Range getDataRange()
```


Ottiene l'intervallo dati della tabella.

**Returns:**
[Range](../../com.aspose.cells/range)
### getDataSourceType() {#getDataSourceType--}
```
public int getDataSourceType()
```


Ottiene il tipo di origine dati della tabella.

Vedi [TableDataSourceType](../../com.aspose.cells/tabledatasourcetype).

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Ottiene il nome visualizzato della tabella.

**Returns:**
java.lang.String
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Restituisce la colonna finale dell'intervallo.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Restituisce la riga finale dell'intervallo.

**Returns:**
int
### getListColumns() {#getListColumns--}
```
public ListColumnCollection getListColumns()
```


Restituisce l'elenco [ListColumn](../../com.aspose.cells/listcolumn) di questa tabella.

**Returns:**
[ListColumnCollection](../../com.aspose.cells/listcolumncollection)
### getQueryTable() {#getQueryTable--}
```
public QueryTable getQueryTable()
```


Restituisce la QueryTable collegata.

**Returns:**
[QueryTable](../../com.aspose.cells/querytable)
### getShowHeaderRow() {#getShowHeaderRow--}
```
public boolean getShowHeaderRow()
```


Restituisce se questa Table mostra la riga di intestazione.

**Returns:**
boolean
### getShowTableStyleColumnStripes() {#getShowTableStyleColumnStripes--}
```
public boolean getShowTableStyleColumnStripes()
```


Indica se la formattazione a strisce di colonna è applicata.

**Returns:**
boolean
### getShowTableStyleFirstColumn() {#getShowTableStyleFirstColumn--}
```
public boolean getShowTableStyleFirstColumn()
```


Indica se la prima colonna nella tabella è lo stile applicato.

**Returns:**
boolean
### getShowTableStyleLastColumn() {#getShowTableStyleLastColumn--}
```
public boolean getShowTableStyleLastColumn()
```


Indica se l'ultima colonna nella tabella è lo stile applicato.

**Returns:**
boolean
### getShowTableStyleRowStripes() {#getShowTableStyleRowStripes--}
```
public boolean getShowTableStyleRowStripes()
```


Indica se la formattazione a strisce di riga è applicata.

**Returns:**
boolean
### getShowTotals() {#getShowTotals--}
```
public boolean getShowTotals()
```


Restituisce se questa TAble mostra la riga totale.

**Returns:**
boolean
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Restituisce la colonna iniziale dell'intervallo.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Restituisce la riga iniziale dell'intervallo.

**Returns:**
int
### getTableStyleName() {#getTableStyleName--}
```
public String getTableStyleName()
```


Restituisce il nome dello stile della tabella.

**Returns:**
java.lang.String
### getTableStyleType() {#getTableStyleType--}
```
public int getTableStyleType()
```


Restituisce lo stile di tabella incorporato.

Vedi [TableStyleType](../../com.aspose.cells/tablestyletype).

**Example**

```
         Workbook workbook = new Workbook("Book1.xlsx");
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setTableStyleType(TableStyleType.TABLE_STYLE_DARK_2);
          workbook.save("TableStyle.xlsx");
```

**Returns:**
int
### getXmlMap() {#getXmlMap--}
```
public XmlMap getXmlMap()
```


Restituisce un [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) utilizzato per questo elenco.

**Returns:**
[XmlMap](../../com.aspose.cells/xmlmap)
### hasAutoFilter() {#hasAutoFilter--}
```
public boolean hasAutoFilter()
```


Indica se il filtro automatico è applicato a questa tabella.

**Returns:**
boolean
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




### putCellFormula(int rowOffset, int columnOffset, String formula) {#putCellFormula-int-int-java.lang.String-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula)
```


Inserisci la formula nella cella della tabella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | int | L'offset di riga nella tabella. |
| columnOffset | int | L'offset di colonna nella tabella. |
| formula | java.lang.String | La formula della cella. |

### putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula) {#putCellFormula-int-int-java.lang.String-boolean-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)
```


Inserisci la formula nella cella della tabella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | int | L'offset di riga nella tabella. |
| columnOffset | int | L'offset di colonna nella tabella. |
| formula | java.lang.String | La formula della cella. |
| isTotalsRowFormula | boolean |  |

### putCellValue(int rowOffset, int columnOffset, Object value) {#putCellValue-int-int-java.lang.Object-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value)
```


Inserisci il valore nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | int | L'offset di riga nella tabella. |
| columnOffset | int | L'offset di colonna nella tabella. |
| valore | java.lang.Object | Il valore della cella. |

### putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel) {#putCellValue-int-int-java.lang.Object-boolean-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)
```


Inserisci il valore nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | int | L'offset di riga nella tabella. |
| columnOffset | int | L'offset di colonna nella tabella. |
| valore | java.lang.Object | Il valore della cella. |
| isTotalsRowLabel | boolean | Indica se è un'etichetta per la riga totale, funziona solo per la riga totale. Se False e questa riga è la riga totale, verrà inserita una nuova riga. |

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Rimuove il filtro automatico applicato a questa tabella.

### resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#resize-int-int-int-int-boolean-}
```
public void resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


Ridimensiona l'intervallo dell'oggetto elenco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | L'indice di riga iniziale del nuovo intervallo. |
| startColumn | int | L'indice di colonna iniziale del nuovo intervallo. |
| endRow | int | L'indice di riga finale del nuovo intervallo. |
| endColumn | int | L'indice di colonna finale del nuovo intervallo. |
| hasHeaders | boolean | Se questa tabella ha intestazioni. |

### setAlternativeDescription(String value) {#setAlternativeDescription-java.lang.String-}
```
public void setAlternativeDescription(String value)
```


Imposta la descrizione alternativa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Imposta il testo alternativo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Imposta il commento della tabella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Imposta il nome visualizzato della tabella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setHasAutoFilter(boolean value) {#setHasAutoFilter-boolean-}
```
public void setHasAutoFilter(boolean value)
```


Indica se il filtro automatico è applicato a questa tabella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowHeaderRow(boolean value) {#setShowHeaderRow-boolean-}
```
public void setShowHeaderRow(boolean value)
```


Imposta se questa Table mostra la riga di intestazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowTableStyleColumnStripes(boolean value) {#setShowTableStyleColumnStripes-boolean-}
```
public void setShowTableStyleColumnStripes(boolean value)
```


Indica se la formattazione a strisce di colonna è applicata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowTableStyleFirstColumn(boolean value) {#setShowTableStyleFirstColumn-boolean-}
```
public void setShowTableStyleFirstColumn(boolean value)
```


Indica se la prima colonna nella tabella è lo stile applicato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowTableStyleLastColumn(boolean value) {#setShowTableStyleLastColumn-boolean-}
```
public void setShowTableStyleLastColumn(boolean value)
```


Indica se l'ultima colonna nella tabella è lo stile applicato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowTableStyleRowStripes(boolean value) {#setShowTableStyleRowStripes-boolean-}
```
public void setShowTableStyleRowStripes(boolean value)
```


Indica se la formattazione a strisce di riga è applicata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowTotals(boolean value) {#setShowTotals-boolean-}
```
public void setShowTotals(boolean value)
```


Imposta se questa TAble mostra la riga totale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTableStyleName(String value) {#setTableStyleName-java.lang.String-}
```
public void setTableStyleName(String value)
```


Imposta il nome dello stile della tabella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTableStyleType(int value) {#setTableStyleType-int-}
```
public void setTableStyleType(int value)
```


Restituisce lo stile di tabella incorporato.

Vedi [TableStyleType](../../com.aspose.cells/tablestyletype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


Aggiorna i nomi di tutte le colonne dell'elenco nelle celle della tabella.

**Remarks**

Il valore delle celle nella riga di intestazione della tabella deve essere lo stesso del nome della ListColumn; Cell.PutValue non modifica automaticamente il nome della ListColumn per motivi di prestazioni.

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

