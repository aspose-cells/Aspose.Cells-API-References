---
title: "ListBoxActiveXControl"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un controllo ActiveX ListBox."
type: docs
url: /it/java/com.aspose.cells/listboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ListBoxActiveXControl extends ActiveXControl
```

Rappresenta un controllo ActiveX ListBox.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Ottiene il colore ole dello sfondo. |
| [getBorderOleColor()](#getBorderOleColor--) | Ottiene il colore ole dello sfondo. |
| [getBorderStyle()](#getBorderStyle--) | Ottiene il tipo di bordo utilizzato dal controllo. |
| [getBoundColumn()](#getBoundColumn--) | Rappresenta come la proprietà Value viene determinata per un ComboBox o ListBox quando il valore della proprietà MultiSelect è (fmMultiSelectSingle). |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Rappresenta il numero di colonne da visualizzare in un ComboBox o ListBox. |
| [getColumnWidths()](#getColumnWidths--) | Restituisce la larghezza della colonna. |
| [getData()](#getData--) | Restituisce i dati binari del controllo. |
| [getFont()](#getFont--) | Rappresenta il carattere del controllo. |
| [getForeOleColor()](#getForeOleColor--) | Restituisce il colore OLE del primo piano. |
| [getHeight()](#getHeight--) | Restituisce l'altezza del controllo in unità di punti. |
| [getIMEMode()](#getIMEMode--) | Restituisce la modalità di esecuzione predefinita dell'Editor di metodo di input per il controllo quando riceve il fuoco. |
| [getIntegralHeight()](#getIntegralHeight--) | Indica se il controllo mostrerà solo linee di testo complete senza mostrare linee parziali. |
| [getLinkedCell()](#getLinkedCell--) | Restituisce la cella collegata. |
| [getListFillRange()](#getListFillRange--) | Restituisce l'intervallo di riempimento dell'elenco. |
| [getListStyle()](#getListStyle--) | Restituisce l'aspetto visivo. |
| [getListWidth()](#getListWidth--) | Restituisce la larghezza in unità di punti. |
| [getMatchEntry()](#getMatchEntry--) | Indica come una ListBox o ComboBox ricerca la sua lista mentre l'utente digita. |
| [getMouseIcon()](#getMouseIcon--) | Restituisce un'icona personalizzata da visualizzare come puntatore del mouse per il controllo. |
| [getMousePointer()](#getMousePointer--) | Restituisce il tipo di icona visualizzata come puntatore del mouse per il controllo. |
| [getScrollBars()](#getScrollBars--) | Indica se il controllo ha barre di scorrimento verticali, barre di scorrimento orizzontali, entrambe o nessuna. |
| [getSelectionType()](#getSelectionType--) | Indica se il controllo consente selezioni multiple. |
| [getShadow()](#getShadow--) | Indica se mostrare un'ombra. |
| [getShowColumnHeads()](#getShowColumnHeads--) | Indica se le intestazioni di colonna sono visualizzate. |
| [getSpecialEffect()](#getSpecialEffect--) | Restituisce l'effetto speciale del controllo. |
| [getTextAlign()](#getTextAlign--) | Rappresenta come allineare il testo utilizzato dal controllo. |
| [getTextColumn()](#getTextColumn--) | Rappresenta la colonna in una ComboBox o ListBox da visualizzare all'utente. |
| [getType()](#getType--) | Restituisce il tipo del controllo ActiveX. |
| [getValue()](#getValue--) | Ottiene il valore del controllo. |
| [getWidth()](#getWidth--) | Ottiene la larghezza del controllo in unità di punti. |
| [getWorkbook()](#getWorkbook--) | Ottiene l'oggetto [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto. |
| [isEnabled()](#isEnabled--) | Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente. |
| [isLocked()](#isLocked--) | Indica se i dati nel controllo sono bloccati per la modifica. |
| [isTransparent()](#isTransparent--) | Indica se il controllo è trasparente. |
| [isVisible()](#isVisible--) | Indica se questo controllo è visibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Imposta il colore OLE dello sfondo. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Imposta il colore OLE dello sfondo. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Imposta il tipo di bordo utilizzato dal controllo. |
| [setBoundColumn(int value)](#setBoundColumn-int-) | Rappresenta come la proprietà Value viene determinata per un ComboBox o ListBox quando il valore della proprietà MultiSelect è (fmMultiSelectSingle). |
| [setColumnCount(int value)](#setColumnCount-int-) | Rappresenta il numero di colonne da visualizzare in un ComboBox o ListBox. |
| [setColumnWidths(double value)](#setColumnWidths-double-) | Imposta la larghezza della colonna. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Imposta il colore OLE del primo piano. |
| [setHeight(double value)](#setHeight-double-) | Imposta l'altezza del controllo in unità di punti. |
| [setIMEMode(int value)](#setIMEMode-int-) | Imposta la modalità di esecuzione predefinita dell'Input Method Editor per il controllo quando riceve il focus. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | Indica se il controllo mostrerà solo linee di testo complete senza mostrare linee parziali. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Imposta la cella collegata. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Imposta l'intervallo di riempimento dell'elenco. |
| [setListStyle(int value)](#setListStyle-int-) | Imposta l'aspetto visivo. |
| [setListWidth(double value)](#setListWidth-double-) | Imposta la larghezza in unità di punti. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indica se i dati nel controllo sono bloccati per la modifica. |
| [setMatchEntry(int value)](#setMatchEntry-int-) | Indica come una ListBox o ComboBox ricerca la sua lista mentre l'utente digita. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo. |
| [setMousePointer(int value)](#setMousePointer-int-) | Imposta il tipo di icona visualizzata come puntatore del mouse per il controllo. |
| [setScrollBars(int value)](#setScrollBars-int-) | Indica se il controllo ha barre di scorrimento verticali, barre di scorrimento orizzontali, entrambe o nessuna. |
| [setSelectionType(int value)](#setSelectionType-int-) | Indica se il controllo consente selezioni multiple. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indica se mostrare un'ombra. |
| [setShowColumnHeads(boolean value)](#setShowColumnHeads-boolean-) | Indica se le intestazioni di colonna sono visualizzate. |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Imposta l'effetto speciale del controllo. |
| [setTextAlign(int value)](#setTextAlign-int-) | Rappresenta come allineare il testo utilizzato dal controllo. |
| [setTextColumn(int value)](#setTextColumn-int-) | Rappresenta la colonna in una ComboBox o ListBox da visualizzare all'utente. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indica se il controllo è trasparente. |
| [setValue(String value)](#setValue-java.lang.String-) | Imposta il valore del controllo. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indica se questo controllo è visibile. |
| [setWidth(double value)](#setWidth-double-) | Imposta la larghezza del controllo in unità di punti. |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Ottiene il colore ole dello sfondo.

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


Ottiene il colore ole dello sfondo.

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Ottiene il tipo di bordo utilizzato dal controllo.

Vedi [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Returns:**
int
### getBoundColumn() {#getBoundColumn--}
```
public int getBoundColumn()
```


Rappresenta come la proprietà Value viene determinata per un ComboBox o ListBox quando il valore della proprietà MultiSelect è (fmMultiSelectSingle).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Rappresenta il numero di colonne da visualizzare in un ComboBox o ListBox.

**Returns:**
int
### getColumnWidths() {#getColumnWidths--}
```
public double getColumnWidths()
```


Restituisce la larghezza della colonna.

**Returns:**
double
### getData() {#getData--}
```
public byte[] getData()
```


Restituisce i dati binari del controllo.

**Returns:**
byte[]
### getFont() {#getFont--}
```
public Font getFont()
```


Rappresenta il carattere del controllo.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


Restituisce il colore OLE del primo piano.

**Remarks**

Non si applica al controllo Image.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Restituisce l'altezza del controllo in unità di punti.

**Returns:**
double
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


Restituisce la modalità di esecuzione predefinita dell'Editor di metodo di input per il controllo quando riceve il fuoco.

Vedi [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Returns:**
int
### getIntegralHeight() {#getIntegralHeight--}
```
public boolean getIntegralHeight()
```


Indica se il controllo mostrerà solo linee di testo complete senza mostrare linee parziali.

**Returns:**
boolean
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Restituisce la cella collegata.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


Restituisce l'intervallo di riempimento dell'elenco.

**Returns:**
java.lang.String
### getListStyle() {#getListStyle--}
```
public int getListStyle()
```


Restituisce l'aspetto visivo.

Vedi [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Returns:**
int
### getListWidth() {#getListWidth--}
```
public double getListWidth()
```


Restituisce la larghezza in unità di punti.

**Returns:**
double
### getMatchEntry() {#getMatchEntry--}
```
public int getMatchEntry()
```


Indica come una ListBox o ComboBox ricerca la sua lista mentre l'utente digita.

Vedi [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

**Returns:**
int
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


Restituisce un'icona personalizzata da visualizzare come puntatore del mouse per il controllo.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


Restituisce il tipo di icona visualizzata come puntatore del mouse per il controllo.

Vedi [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Returns:**
int
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


Indica se il controllo ha barre di scorrimento verticali, barre di scorrimento orizzontali, entrambe o nessuna.

Vedi [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Returns:**
int
### getSelectionType() {#getSelectionType--}
```
public int getSelectionType()
```


Indica se il controllo consente selezioni multiple.

Vedi [SelectionType](../../com.aspose.cells/selectiontype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indica se mostrare un'ombra.

**Returns:**
boolean
### getShowColumnHeads() {#getShowColumnHeads--}
```
public boolean getShowColumnHeads()
```


Indica se le intestazioni di colonna sono visualizzate.

**Returns:**
boolean
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Restituisce l'effetto speciale del controllo.

Vedi [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Returns:**
int
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Rappresenta come allineare il testo utilizzato dal controllo.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextColumn() {#getTextColumn--}
```
public int getTextColumn()
```


Rappresenta la colonna in una ComboBox o ListBox da visualizzare all'utente.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Restituisce il tipo del controllo ActiveX.

Vedi [ControlType](../../com.aspose.cells/controltype).

**Returns:**
int
### getValue() {#getValue--}
```
public String getValue()
```


Ottiene il valore del controllo.

**Remarks**

Ha effetto solo quando [getSelectionType()](../../com.aspose.cells/listboxactivexcontrol\#getSelectionType--) è SelectionType.Single;

**Returns:**
java.lang.String
### getWidth() {#getWidth--}
```
public double getWidth()
```


Ottiene la larghezza del controllo in unità di punti.

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Ottiene l'oggetto [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--).

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```


Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto.

**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```


Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Indica se i dati nel controllo sono bloccati per la modifica.

**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```


Indica se il controllo è trasparente.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Indica se questo controllo è visibile.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Imposta il colore OLE dello sfondo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


Imposta il colore OLE dello sfondo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Imposta il tipo di bordo utilizzato dal controllo.

Vedi [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBoundColumn(int value) {#setBoundColumn-int-}
```
public void setBoundColumn(int value)
```


Rappresenta come la proprietà Value viene determinata per un ComboBox o ListBox quando il valore della proprietà MultiSelect è (fmMultiSelectSingle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setColumnCount(int value) {#setColumnCount-int-}
```
public void setColumnCount(int value)
```


Rappresenta il numero di colonne da visualizzare in un ComboBox o ListBox.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setColumnWidths(double value) {#setColumnWidths-double-}
```
public void setColumnWidths(double value)
```


Imposta la larghezza della colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


Imposta il colore OLE del primo piano.

**Remarks**

Non si applica al controllo Image.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Imposta l'altezza del controllo in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


Imposta la modalità di esecuzione predefinita dell'Input Method Editor per il controllo quando riceve il focus.

Vedi [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setIntegralHeight(boolean value) {#setIntegralHeight-boolean-}
```
public void setIntegralHeight(boolean value)
```


Indica se il controllo mostrerà solo linee di testo complete senza mostrare linee parziali.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Imposta la cella collegata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


Imposta l'intervallo di riempimento dell'elenco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setListStyle(int value) {#setListStyle-int-}
```
public void setListStyle(int value)
```


Imposta l'aspetto visivo.

Vedi [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setListWidth(double value) {#setListWidth-double-}
```
public void setListWidth(double value)
```


Imposta la larghezza in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Indica se i dati nel controllo sono bloccati per la modifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMatchEntry(int value) {#setMatchEntry-int-}
```
public void setMatchEntry(int value)
```


Indica come una ListBox o ComboBox ricerca la sua lista mentre l'utente digita.

Vedi [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


Imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


Imposta il tipo di icona visualizzata come puntatore del mouse per il controllo.

Vedi [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setScrollBars(int value) {#setScrollBars-int-}
```
public void setScrollBars(int value)
```


Indica se il controllo ha barre di scorrimento verticali, barre di scorrimento orizzontali, entrambe o nessuna.

Vedi [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSelectionType(int value) {#setSelectionType-int-}
```
public void setSelectionType(int value)
```


Indica se il controllo consente selezioni multiple.

Vedi [SelectionType](../../com.aspose.cells/selectiontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Indica se mostrare un'ombra.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowColumnHeads(boolean value) {#setShowColumnHeads-boolean-}
```
public void setShowColumnHeads(boolean value)
```


Indica se le intestazioni di colonna sono visualizzate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


Imposta l'effetto speciale del controllo.

Vedi [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


Rappresenta come allineare il testo utilizzato dal controllo.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextColumn(int value) {#setTextColumn-int-}
```
public void setTextColumn(int value)
```


Rappresenta la colonna in una ComboBox o ListBox da visualizzare all'utente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Indica se il controllo è trasparente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setValue(String value) {#setValue-java.lang.String-}
```
public void setValue(String value)
```


Imposta il valore del controllo.

**Remarks**

Ha effetto solo quando [getSelectionType()](../../com.aspose.cells/listboxactivexcontrol\#getSelectionType--) è SelectionType.Single;

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indica se questo controllo è visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Imposta la larghezza del controllo in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

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

