---
title: "TextBoxActiveXControl"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un controllo ActiveX per casella di testo."
type: docs
url: /it/java/com.aspose.cells/textboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class TextBoxActiveXControl extends ActiveXControl
```

Rappresenta un controllo ActiveX per casella di testo.

**Example**

```
         //Initialize a new workbook.
         Workbook book = new Workbook();
 
         //Add a TextBoxActiveXControl.
         Shape shape = book.getWorksheets().get(0).getShapes().addActiveXControl(ControlType.TEXT_BOX, 1, 0, 1, 0, 100, 50);
         TextBoxActiveXControl activeXControl = (TextBoxActiveXControl)shape.getActiveXControl();
 
         //do your business
 
         //Save the excel file.
         book.save("exmaple.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Ottiene il colore ole dello sfondo. |
| [getBorderOleColor()](#getBorderOleColor--) | Ottiene il colore ole dello sfondo. |
| [getBorderStyle()](#getBorderStyle--) | Ottiene il tipo di bordo utilizzato dal controllo. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Restituisce i dati binari del controllo. |
| [getDropButtonStyle()](#getDropButtonStyle--) | Specifica il simbolo visualizzato sul pulsante a discesa |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | Specifica il comportamento di selezione quando si entra nel controllo. |
| [getEnterKeyBehavior()](#getEnterKeyBehavior--) | Specifica il comportamento del tasto ENTER. |
| [getFont()](#getFont--) | Rappresenta il carattere del controllo. |
| [getForeOleColor()](#getForeOleColor--) | Restituisce il colore OLE del primo piano. |
| [getHeight()](#getHeight--) | Restituisce l'altezza del controllo in unità di punti. |
| [getHideSelection()](#getHideSelection--) | Indica se il testo selezionato nel controllo appare evidenziato quando il controllo non ha il fuoco. |
| [getIMEMode()](#getIMEMode--) | Restituisce la modalità di esecuzione predefinita dell'Editor di metodo di input per il controllo quando riceve il fuoco. |
| [getIntegralHeight()](#getIntegralHeight--) | Indica se il controllo mostrerà solo linee di testo complete senza mostrare linee parziali. |
| [getLinkedCell()](#getLinkedCell--) | Restituisce la cella collegata. |
| [getListFillRange()](#getListFillRange--) | Restituisce l'intervallo di riempimento dell'elenco. |
| [getMaxLength()](#getMaxLength--) | Restituisce il numero massimo di caratteri |
| [getMouseIcon()](#getMouseIcon--) | Restituisce un'icona personalizzata da visualizzare come puntatore del mouse per il controllo. |
| [getMousePointer()](#getMousePointer--) | Restituisce il tipo di icona visualizzata come puntatore del mouse per il controllo. |
| [getPasswordChar()](#getPasswordChar--) | Ottiene un carattere da visualizzare al posto dei caratteri inseriti. |
| [getScrollBars()](#getScrollBars--) | Indica se il controllo ha barre di scorrimento verticali, barre di scorrimento orizzontali, entrambe o nessuna. |
| [getShadow()](#getShadow--) | Indica se mostrare un'ombra. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | Specifica il simbolo visualizzato sul pulsante a discesa |
| [getSpecialEffect()](#getSpecialEffect--) | Restituisce l'effetto speciale del controllo. |
| [getTabKeyBehavior()](#getTabKeyBehavior--) | Indica se i caratteri di tabulazione sono consentiti nel testo del controllo. |
| [getText()](#getText--) | Ottiene il testo del controllo. |
| [getTextAlign()](#getTextAlign--) | Rappresenta come allineare il testo utilizzato dal controllo. |
| [getType()](#getType--) | Restituisce il tipo del controllo ActiveX. |
| [getWidth()](#getWidth--) | Ottiene la larghezza del controllo in unità di punti. |
| [getWorkbook()](#getWorkbook--) | Ottiene l'oggetto [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto. |
| [isAutoTab()](#isAutoTab--) | Indica se il focus si sposterà automaticamente al controllo successivo quando l'utente inserisce il numero massimo di caratteri. |
| [isAutoWordSelected()](#isAutoWordSelected--) | Specifica l'unità di base utilizzata per estendere una selezione. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | Indica se il trascinamento è abilitato per il controllo. |
| [isEditable()](#isEditable--) | Indica se l'utente può digitare nel controllo. |
| [isEnabled()](#isEnabled--) | Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente. |
| [isLocked()](#isLocked--) | Indica se i dati nel controllo sono bloccati per la modifica. |
| [isMultiLine()](#isMultiLine--) | Indica se il controllo può visualizzare più di una riga di testo. |
| [isTransparent()](#isTransparent--) | Indica se il controllo è trasparente. |
| [isVisible()](#isVisible--) | Indica se questo controllo è visibile. |
| [isWordWrapped()](#isWordWrapped--) | Indica se il contenuto del controllo va a capo automaticamente alla fine di una riga. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto. |
| [setAutoTab(boolean value)](#setAutoTab-boolean-) | Indica se il focus si sposterà automaticamente al controllo successivo quando l'utente inserisce il numero massimo di caratteri. |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | Specifica l'unità di base utilizzata per estendere una selezione. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Imposta il colore OLE dello sfondo. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Imposta il colore OLE dello sfondo. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Imposta il tipo di bordo utilizzato dal controllo. |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | Indica se il trascinamento è abilitato per il controllo. |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | Specifica il simbolo visualizzato sul pulsante a discesa |
| [setEditable(boolean value)](#setEditable-boolean-) | Indica se l'utente può digitare nel controllo. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente. |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | Specifica il comportamento di selezione quando si entra nel controllo. |
| [setEnterKeyBehavior(boolean value)](#setEnterKeyBehavior-boolean-) | Specifica il comportamento del tasto ENTER. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Imposta il colore OLE del primo piano. |
| [setHeight(double value)](#setHeight-double-) | Imposta l'altezza del controllo in unità di punti. |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | Indica se il testo selezionato nel controllo appare evidenziato quando il controllo non ha il fuoco. |
| [setIMEMode(int value)](#setIMEMode-int-) | Imposta la modalità di esecuzione predefinita dell'Input Method Editor per il controllo quando riceve il focus. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | Indica se il controllo mostrerà solo linee di testo complete senza mostrare linee parziali. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Imposta la cella collegata. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Imposta l'intervallo di riempimento dell'elenco. |
| [setLocked(boolean value)](#setLocked-boolean-) | Indica se i dati nel controllo sono bloccati per la modifica. |
| [setMaxLength(int value)](#setMaxLength-int-) | Imposta il numero massimo di caratteri |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo. |
| [setMousePointer(int value)](#setMousePointer-int-) | Imposta il tipo di icona visualizzata come puntatore del mouse per il controllo. |
| [setMultiLine(boolean value)](#setMultiLine-boolean-) | Indica se il controllo può visualizzare più di una riga di testo. |
| [setPasswordChar(char value)](#setPasswordChar-char-) | Imposta un carattere da visualizzare al posto dei caratteri inseriti. |
| [setScrollBars(int value)](#setScrollBars-int-) | Indica se il controllo ha barre di scorrimento verticali, barre di scorrimento orizzontali, entrambe o nessuna. |
| [setShadow(boolean value)](#setShadow-boolean-) | Indica se mostrare un'ombra. |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | Specifica il simbolo visualizzato sul pulsante a discesa |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Imposta l'effetto speciale del controllo. |
| [setTabKeyBehavior(boolean value)](#setTabKeyBehavior-boolean-) | Indica se i caratteri di tabulazione sono consentiti nel testo del controllo. |
| [setText(String value)](#setText-java.lang.String-) | Imposta il testo del controllo. |
| [setTextAlign(int value)](#setTextAlign-int-) | Rappresenta come allineare il testo utilizzato dal controllo. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indica se il controllo è trasparente. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indica se questo controllo è visibile. |
| [setWidth(double value)](#setWidth-double-) | Imposta la larghezza del controllo in unità di punti. |
| [setWordWrapped(boolean value)](#setWordWrapped-boolean-) | Indica se il contenuto del controllo va a capo automaticamente alla fine di una riga. |
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

**Example**

```
         //excel default color system 12 or green(0x0000FF00)
         activeXControl.setBorderOleColor(/*unchecked*/((int)0x80000012L));
```

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Ottiene il tipo di bordo utilizzato dal controllo.

Vedi [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Example**

```
         activeXControl.setBorderStyle(com.aspose.cells.ControlBorderType.SINGLE);
```

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```


Restituisce i dati binari del controllo.

**Returns:**
byte[]
### getDropButtonStyle() {#getDropButtonStyle--}
```
public int getDropButtonStyle()
```


Specifica il simbolo visualizzato sul pulsante a discesa

Vedi [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Example**

```
         activeXControl.setDropButtonStyle(com.aspose.cells.DropButtonStyle.ARROW);
```

**Returns:**
int
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```
public boolean getEnterFieldBehavior()
```


Specifica il comportamento della selezione all'ingresso del controllo. True specifica che la selezione rimane invariata rispetto all'ultima volta che il controllo era attivo. False specifica che tutto il testo nel controllo verrà selezionato all'ingresso del controllo.

**Example**

```
         if(!activeXControl.getEnterFieldBehavior())
         {
             activeXControl.setEnterFieldBehavior(true);
         }
```

**Returns:**
boolean
### getEnterKeyBehavior() {#getEnterKeyBehavior--}
```
public boolean getEnterKeyBehavior()
```


Specifica il comportamento del tasto ENTER. True specifica che premere ENTER creerà una nuova riga. False specifica che premere ENTER sposterà il focus all'oggetto successivo nell'ordine di tabulazione.

**Example**

```
         if(!activeXControl.getEnterKeyBehavior())
         {
             activeXControl.setEnterKeyBehavior(true);
         }
```

**Returns:**
boolean
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
### getHideSelection() {#getHideSelection--}
```
public boolean getHideSelection()
```


Indica se il testo selezionato nel controllo appare evidenziato quando il controllo non ha il fuoco.

**Example**

```
         if(!activeXControl.getHideSelection())
         {
             activeXControl.setHideSelection(true);
         }
```

**Returns:**
boolean
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

**Example**

```
         if(!activeXControl.getIntegralHeight())
         {
             activeXControl.setIntegralHeight(true);
         }
```

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
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Restituisce il numero massimo di caratteri

**Example**

```
         if(activeXControl.getMaxLength() == 0)
         {
             activeXControl.setMaxLength(30);
         }
```

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
### getPasswordChar() {#getPasswordChar--}
```
public char getPasswordChar()
```


Ottiene un carattere da visualizzare al posto dei caratteri inseriti.

**Example**

```
         activeXControl.setPasswordChar('a');
```

**Returns:**
char
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


Indica se il controllo ha barre di scorrimento verticali, barre di scorrimento orizzontali, entrambe o nessuna.

Vedi [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Example**

```
         activeXControl.setScrollBars(com.aspose.cells.ControlScrollBarType.BARS_VERTICAL);
```

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Indica se mostrare un'ombra.

**Returns:**
boolean
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


Specifica il simbolo visualizzato sul pulsante a discesa

Vedi [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Example**

```
         activeXControl.setShowDropButtonTypeWhen(com.aspose.cells.ShowDropButtonType.FOCUS);
```

**Returns:**
int
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Restituisce l'effetto speciale del controllo.

Vedi [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Example**

```
         activeXControl.setSpecialEffect(com.aspose.cells.ControlSpecialEffectType.BUMP);
```

**Returns:**
int
### getTabKeyBehavior() {#getTabKeyBehavior--}
```
public boolean getTabKeyBehavior()
```


Indica se i caratteri di tabulazione sono consentiti nel testo del controllo.

**Example**

```
         if(!activeXControl.getTabKeyBehavior())
         {
             activeXControl.setTabKeyBehavior(true);
         }
```

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Ottiene il testo del controllo.

**Example**

```
         activeXControl.setText("This is a test.");
```

**Returns:**
java.lang.String
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Rappresenta come allineare il testo utilizzato dal controllo.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Restituisce il tipo del controllo ActiveX.

Vedi [ControlType](../../com.aspose.cells/controltype).

**Example**

```
         /*Aspose.Cells.Drawing.ActiveXControls.ControlType*/int type = activeXControl.getType();
```

**Returns:**
int
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
### isAutoTab() {#isAutoTab--}
```
public boolean isAutoTab()
```


Indica se il focus si sposterà automaticamente al controllo successivo quando l'utente inserisce il numero massimo di caratteri.

**Example**

```
         if(!activeXControl.isAutoTab())
         {
             activeXControl.setAutoTab(true);
         }
```

**Returns:**
boolean
### isAutoWordSelected() {#isAutoWordSelected--}
```
public boolean isAutoWordSelected()
```


Specifica l'unità di base utilizzata per estendere una selezione. True specifica che l'unità di base è un singolo carattere. false specifica che l'unità di base è una parola intera.

**Example**

```
         if(!activeXControl.isAutoWordSelected())
         {
             activeXControl.setAutoWordSelected(true);
         }
```

**Returns:**
boolean
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```
public boolean isDragBehaviorEnabled()
```


Indica se il trascinamento è abilitato per il controllo.

**Example**

```
         if(!activeXControl.isDragBehaviorEnabled())
         {
             activeXControl.setDragBehaviorEnabled(true);
         }
```

**Returns:**
boolean
### isEditable() {#isEditable--}
```
public boolean isEditable()
```


Indica se l'utente può digitare nel controllo.

**Example**

```
         if(!activeXControl.isEditable())
         {
             activeXControl.setEditable(true);
         }
```

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
### isMultiLine() {#isMultiLine--}
```
public boolean isMultiLine()
```


Indica se il controllo può visualizzare più di una riga di testo.

**Example**

```
         if(!activeXControl.isMultiLine())
         {
             activeXControl.setMultiLine(true);
         }
```

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
### isWordWrapped() {#isWordWrapped--}
```
public boolean isWordWrapped()
```


Indica se il contenuto del controllo va a capo automaticamente alla fine di una riga.

**Example**

```
         if(!activeXControl.isWordWrapped())
         {
             activeXControl.setWordWrapped(true);
         }
```

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

### setAutoTab(boolean value) {#setAutoTab-boolean-}
```
public void setAutoTab(boolean value)
```


Indica se il focus si sposterà automaticamente al controllo successivo quando l'utente inserisce il numero massimo di caratteri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoWordSelected(boolean value) {#setAutoWordSelected-boolean-}
```
public void setAutoWordSelected(boolean value)
```


Specifica l'unità di base utilizzata per estendere una selezione. True specifica che l'unità di base è un singolo carattere. false specifica che l'unità di base è una parola intera.

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

### setDragBehaviorEnabled(boolean value) {#setDragBehaviorEnabled-boolean-}
```
public void setDragBehaviorEnabled(boolean value)
```


Indica se il trascinamento è abilitato per il controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDropButtonStyle(int value) {#setDropButtonStyle-int-}
```
public void setDropButtonStyle(int value)
```


Specifica il simbolo visualizzato sul pulsante a discesa

Vedi [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEditable(boolean value) {#setEditable-boolean-}
```
public void setEditable(boolean value)
```


Indica se l'utente può digitare nel controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnterFieldBehavior(boolean value) {#setEnterFieldBehavior-boolean-}
```
public void setEnterFieldBehavior(boolean value)
```


Specifica il comportamento della selezione all'ingresso del controllo. True specifica che la selezione rimane invariata rispetto all'ultima volta che il controllo era attivo. False specifica che tutto il testo nel controllo verrà selezionato all'ingresso del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnterKeyBehavior(boolean value) {#setEnterKeyBehavior-boolean-}
```
public void setEnterKeyBehavior(boolean value)
```


Specifica il comportamento del tasto ENTER. True specifica che premere ENTER creerà una nuova riga. False specifica che premere ENTER sposterà il focus all'oggetto successivo nell'ordine di tabulazione.

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

### setHideSelection(boolean value) {#setHideSelection-boolean-}
```
public void setHideSelection(boolean value)
```


Indica se il testo selezionato nel controllo appare evidenziato quando il controllo non ha il fuoco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Indica se i dati nel controllo sono bloccati per la modifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Imposta il numero massimo di caratteri

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

### setMultiLine(boolean value) {#setMultiLine-boolean-}
```
public void setMultiLine(boolean value)
```


Indica se il controllo può visualizzare più di una riga di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPasswordChar(char value) {#setPasswordChar-char-}
```
public void setPasswordChar(char value)
```


Imposta un carattere da visualizzare al posto dei caratteri inseriti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | char |  |

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

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Indica se mostrare un'ombra.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowDropButtonTypeWhen(int value) {#setShowDropButtonTypeWhen-int-}
```
public void setShowDropButtonTypeWhen(int value)
```


Specifica il simbolo visualizzato sul pulsante a discesa

Vedi [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

### setTabKeyBehavior(boolean value) {#setTabKeyBehavior-boolean-}
```
public void setTabKeyBehavior(boolean value)
```


Indica se i caratteri di tabulazione sono consentiti nel testo del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Imposta il testo del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Indica se il controllo è trasparente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

### setWordWrapped(boolean value) {#setWordWrapped-boolean-}
```
public void setWordWrapped(boolean value)
```


Indica se il contenuto del controllo va a capo automaticamente alla fine di una riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

