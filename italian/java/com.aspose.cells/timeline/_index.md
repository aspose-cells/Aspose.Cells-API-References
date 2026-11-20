---
title: "Timeline"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Descrizione sommaria della visualizzazione Timeline. A causa di MS Excel 2003 non supporta Timeline."
type: docs
url: /it/java/com.aspose.cells/timeline/
---

**Inheritance:**
java.lang.Object
```
public class Timeline
```

Descrizione sommaria della visualizzazione Timeline. A causa di MS Excel, Excel 2003 non supporta Timeline.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
 
         //Create date style
         Style dateStyle = new CellsFactory().createStyle();
         dateStyle.setCustom("m/d/yyyy");
         cells.get(0, 1).setValue("date");
         cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
         cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
         cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
         cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
         //Set date style
         cells.get(1, 1).setStyle(dateStyle);
         cells.get(2, 1).setStyle(dateStyle);
         cells.get(3, 1).setStyle(dateStyle);
         cells.get(4, 1).setStyle(dateStyle);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
 
         PivotTableCollection pivots = sheet.getPivotTables();
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
         //Add time line based on date field.
         int index = sheet.getTimelines().add(pivot, "E1","date");
         Timeline timeline = sheet.getTimelines().get(index);
 
         //do your business
         book.save("out.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaption()](#getCaption--) | Ottiene la didascalia di questa Timeline. |
| [getClass()](#getClass--) |  |
| [getCurrentLevel()](#getCurrentLevel--) | Il livello temporale corrente della Timeline. |
| [getHeightPixel()](#getHeightPixel--) | Restituisce o imposta l'altezza della timeline specificata, in pixel. |
| [getLeftPixel()](#getLeftPixel--) | Restituisce o imposta lo spostamento orizzontale della forma della timeline dalla sua colonna sinistra, in pixel. |
| [getName()](#getName--) | Restituisce o imposta il nome della Timeline specificata |
| [getSelectedDateTimeRange()](#getSelectedDateTimeRange--) | Ottiene l'intervallo di data/ora selezionato. |
| [getSelectionLevel()](#getSelectionLevel--) | Ottiene il livello temporale al quale è stata effettuata la selezione corrente per la Timeline. |
| [getShape()](#getShape--) | Restituisce l'oggetto [TimelineShape](../../com.aspose.cells/timelineshape) associato a questa Timeline. |
| [getShowHeader()](#getShowHeader--) | Indica se visualizzare l'intestazione di questa timeline. |
| [getShowHorizontalScrollbar()](#getShowHorizontalScrollbar--) | Indica se visualizzare la barra di scorrimento orizzontale. |
| [getShowSelectionLabel()](#getShowSelectionLabel--) | Indica se visualizzare l'etichetta di selezione. |
| [getShowTimeLevel()](#getShowTimeLevel--) | Indica se visualizzare la casella a discesa di selezione del livello temporale. |
| [getStartDate()](#getStartDate--) | Ottiene la data di inizio della posizione di scorrimento dell'intervallo di tempo di questa [Timeline](../../com.aspose.cells/timeline). |
| [getTopPixel()](#getTopPixel--) | Restituisce o imposta lo spostamento verticale della forma della timeline dalla sua riga superiore, in pixel. |
| [getWidthPixel()](#getWidthPixel--) | Restituisce o imposta la larghezza della timeline specificata, in pixel. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(DateTime start, DateTime end, boolean calculate)](#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-) | Seleziona l'elemento tra le date/ore. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Imposta la didascalia di questa Timeline. |
| [setCurrentLevel(int value)](#setCurrentLevel-int-) | Il livello temporale corrente della Timeline. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Restituisce o imposta l'altezza della timeline specificata, in pixel. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Restituisce o imposta lo spostamento orizzontale della forma della timeline dalla sua colonna sinistra, in pixel. |
| [setName(String value)](#setName-java.lang.String-) | Restituisce o imposta il nome della Timeline specificata |
| [setSelectionLevel(int value)](#setSelectionLevel-int-) | Imposta il livello temporale al quale è stata effettuata la selezione corrente per la Timeline. |
| [setShowHeader(boolean value)](#setShowHeader-boolean-) | Indica se visualizzare l'intestazione di questa timeline. |
| [setShowHorizontalScrollbar(boolean value)](#setShowHorizontalScrollbar-boolean-) | Indica se visualizzare la barra di scorrimento orizzontale. |
| [setShowSelectionLabel(boolean value)](#setShowSelectionLabel-boolean-) | Indica se visualizzare l'etichetta di selezione. |
| [setShowTimeLevel(boolean value)](#setShowTimeLevel-boolean-) | Indica se visualizzare la casella a discesa di selezione del livello temporale. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Imposta la data di inizio della posizione di scorrimento dell'intervallo di tempo di questa [Timeline](../../com.aspose.cells/timeline). |
| [setTopPixel(int value)](#setTopPixel-int-) | Restituisce o imposta lo spostamento verticale della forma della timeline dalla sua riga superiore, in pixel. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Restituisce o imposta la larghezza della timeline specificata, in pixel. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCaption() {#getCaption--}
```
public String getCaption()
```


Ottiene la didascalia di questa Timeline.

**Example**

```
         //Set the caption of this Timeline.
         timeline.setCaption("timeline caption test");
```

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentLevel() {#getCurrentLevel--}
```
public int getCurrentLevel()
```


Il livello temporale corrente della Timeline.

Vedi [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Restituisce o imposta l'altezza della timeline specificata, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Height. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Restituisce o imposta lo spostamento orizzontale della forma della timeline dalla sua colonna sinistra, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Left. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Restituisce o imposta il nome della Timeline specificata

**Example**

```
         //Set the name of the specified Timeline.
         timeline.setName("timeline name test");
```

**Returns:**
java.lang.String
### getSelectedDateTimeRange() {#getSelectedDateTimeRange--}
```
public DateTime[] getSelectedDateTimeRange()
```


Ottiene l'intervallo di data/ora selezionato.

**Returns:**
com.aspose.cells.DateTime[] -
### getSelectionLevel() {#getSelectionLevel--}
```
public int getSelectionLevel()
```


Ottiene il livello temporale al quale è stata effettuata la selezione corrente per la Timeline.

Vedi [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getShape() {#getShape--}
```
public TimelineShape getShape()
```


Restituisce l'oggetto [TimelineShape](../../com.aspose.cells/timelineshape) associato a questa Timeline.

**Returns:**
[TimelineShape](../../com.aspose.cells/timelineshape)
### getShowHeader() {#getShowHeader--}
```
public boolean getShowHeader()
```


Indica se visualizzare l'intestazione di questa timeline.

**Returns:**
boolean
### getShowHorizontalScrollbar() {#getShowHorizontalScrollbar--}
```
public boolean getShowHorizontalScrollbar()
```


Indica se visualizzare la barra di scorrimento orizzontale.

**Returns:**
boolean
### getShowSelectionLabel() {#getShowSelectionLabel--}
```
public boolean getShowSelectionLabel()
```


Indica se visualizzare l'etichetta di selezione.

**Returns:**
boolean
### getShowTimeLevel() {#getShowTimeLevel--}
```
public boolean getShowTimeLevel()
```


Indica se visualizzare la casella a discesa di selezione del livello temporale.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Ottiene la data di inizio della posizione di scorrimento dell'intervallo di tempo di questa [Timeline](../../com.aspose.cells/timeline).

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Restituisce o imposta lo spostamento verticale della forma della timeline dalla sua riga superiore, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Top. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Restituisce o imposta la larghezza della timeline specificata, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Width. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Returns:**
int
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




### select(DateTime start, DateTime end, boolean calculate) {#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-}
```
public void select(DateTime start, DateTime end, boolean calculate)
```


Seleziona l'elemento tra le date/ore.

**Remarks**

[getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--) must be set before calling this method. If this method is called, [getSelectionLevel()](../../com.aspose.cells/timeline\#getSelectionLevel--) will be [getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | La data e ora di inizio |
| end | [DateTime](../../com.aspose.cells/datetime) | La data e ora di fine |
| calcolare | boolean | Indica se calcolare le tabelle pivot relative |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Imposta la didascalia di questa Timeline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCurrentLevel(int value) {#setCurrentLevel-int-}
```
public void setCurrentLevel(int value)
```


Il livello temporale corrente della Timeline.

Vedi [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Restituisce o imposta l'altezza della timeline specificata, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Height. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLeftPixel(int value) {#setLeftPixel-int-}
```
public void setLeftPixel(int value)
```


Restituisce o imposta lo spostamento orizzontale della forma della timeline dalla sua colonna sinistra, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Left. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Restituisce o imposta il nome della Timeline specificata

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSelectionLevel(int value) {#setSelectionLevel-int-}
```
public void setSelectionLevel(int value)
```


Imposta il livello temporale al quale è stata effettuata la selezione corrente per la Timeline.

Vedi [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShowHeader(boolean value) {#setShowHeader-boolean-}
```
public void setShowHeader(boolean value)
```


Indica se visualizzare l'intestazione di questa timeline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowHorizontalScrollbar(boolean value) {#setShowHorizontalScrollbar-boolean-}
```
public void setShowHorizontalScrollbar(boolean value)
```


Indica se visualizzare la barra di scorrimento orizzontale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowSelectionLabel(boolean value) {#setShowSelectionLabel-boolean-}
```
public void setShowSelectionLabel(boolean value)
```


Indica se visualizzare l'etichetta di selezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowTimeLevel(boolean value) {#setShowTimeLevel-boolean-}
```
public void setShowTimeLevel(boolean value)
```


Indica se visualizzare la casella a discesa di selezione del livello temporale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Imposta la data di inizio della posizione di scorrimento dell'intervallo di tempo di questa [Timeline](../../com.aspose.cells/timeline).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Restituisce o imposta lo spostamento verticale della forma della timeline dalla sua riga superiore, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Top. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Restituisce o imposta la larghezza della timeline specificata, in pixel.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Width. Questa proprietà sarà rimossa 12 mesi dopo da maggio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

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

