---
title: "DataBar"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Descrive la regola di formattazione condizionale DataBar."
type: docs
url: /it/java/com.aspose.cells/databar/
---

**Inheritance:**
java.lang.Object
```
public class DataBar
```

Descrivi la regola di formattazione condizionale DataBar. Questa regola di formattazione condizionale visualizza una barra dati graduale nell'intervallo di celle.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
 
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
 
         ca.StartRow = 0;
 
         ca.EndRow = 2;
 
         ca.StartColumn = 0;
 
         ca.EndColumn = 0;
 
         fcs.addArea(ca);
 
         //Adds condition.
         int idx = fcs.addCondition(FormatConditionType.DATA_BAR);
 
         fcs.addArea(ca);
 
         FormatCondition cond = fcs.get(idx);
 
         //Get Databar
         DataBar dataBar = cond.getDataBar();
 
         dataBar.setColor(Color.getOrange());
 
         //Set Databar properties
         dataBar.getMinCfvo().setType(FormatConditionValueType.PERCENTILE);
 
         dataBar.getMinCfvo().setValue(30);
 
         dataBar.setShowValue(false);
 
         dataBar.getBarBorder().setType(DataBarBorderType.SOLID);
 
         dataBar.getBarBorder().setColor(Color.getPlum());
 
          dataBar.setBarFillType(DataBarFillType.SOLID);
 
          dataBar.setAxisColor(Color.getRed());
 
          dataBar.setAxisPosition(DataBarAxisPosition.MIDPOINT);
 
          dataBar.getNegativeBarFormat().setColorType(DataBarNegativeColorType.COLOR);
 
          dataBar.getNegativeBarFormat().setColor(Color.getWhite());
 
          dataBar.getNegativeBarFormat().setBorderColorType(DataBarNegativeColorType.COLOR);
 
          dataBar.getNegativeBarFormat().setBorderColor(Color.getYellow());
 
         //Put Cell Values
         Cell cell1 = sheet.getCells().get("A1");
 
         cell1.putValue(10);
 
         Cell cell2 = sheet.getCells().get("A2");
 
         cell2.putValue(120);
 
         Cell cell3 = sheet.getCells().get("A3");
 
         cell3.putValue(260);
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisColor()](#getAxisColor--) | Ottiene il colore dell'asse per le celle con formattazione condizionale come barre dati. |
| [getAxisPosition()](#getAxisPosition--) | Ottiene la posizione dell'asse delle barre dati specificate da una regola di formattazione condizionale. |
| [getBarBorder()](#getBarBorder--) | Ottiene un oggetto che specifica il bordo di una barra dati. |
| [getBarFillType()](#getBarFillType--) | Ottiene come una barra dati è riempita di colore. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Ottiene il colore di questo DataBar. |
| [getDirection()](#getDirection--) | Ottiene la direzione in cui la barra dati è visualizzata. |
| [getMaxCfvo()](#getMaxCfvo--) | Ottiene l'oggetto valore massimo di questo DataBar. |
| [getMaxLength()](#getMaxLength--) | Rappresenta la lunghezza massima della barra dati. |
| [getMinCfvo()](#getMinCfvo--) | Ottiene l'oggetto valore minimo di questo DataBar. |
| [getMinLength()](#getMinLength--) | Rappresenta la lunghezza minima della barra dati. |
| [getNegativeBarFormat()](#getNegativeBarFormat--) | Ottiene l'oggetto NegativeBarFormat associato a una regola di formattazione condizionale barra dati. |
| [getShowValue()](#getShowValue--) | Ottiene l'indicatore che indica se mostrare i valori delle celle su cui è applicata questa barra dati. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAxisColor(Color value)](#setAxisColor-com.aspose.cells.Color-) | Ottiene il colore dell'asse per le celle con formattazione condizionale come barre dati. |
| [setAxisPosition(int value)](#setAxisPosition-int-) | Imposta la posizione dell'asse delle barre dati specificate da una regola di formattazione condizionale. |
| [setBarFillType(int value)](#setBarFillType-int-) | Imposta come una barra dati è riempita di colore. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Imposta il colore di questo DataBar. |
| [setDirection(int value)](#setDirection-int-) | Imposta la direzione in cui la barra dati è visualizzata. |
| [setMaxLength(int value)](#setMaxLength-int-) | Rappresenta la lunghezza massima della barra dati. |
| [setMinLength(int value)](#setMinLength-int-) | Rappresenta la lunghezza minima della barra dati. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Imposta l'indicatore che indica se mostrare i valori delle celle su cui è applicata questa barra dati. |
| [toImage(Cell cell, ImageOrPrintOptions imgOpts)](#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-) | Renderizza la barra dati nella cella in un array di byte dell'immagine. |
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
### getAxisColor() {#getAxisColor--}
```
public Color getAxisColor()
```


Ottiene il colore dell'asse per le celle con formattazione condizionale come barre dati.

**Returns:**
[Color](../../com.aspose.cells/color)
### getAxisPosition() {#getAxisPosition--}
```
public int getAxisPosition()
```


Ottiene la posizione dell'asse delle barre dati specificate da una regola di formattazione condizionale.

Vedi [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Returns:**
int
### getBarBorder() {#getBarBorder--}
```
public DataBarBorder getBarBorder()
```


Ottiene un oggetto che specifica il bordo di una barra dati.

**Returns:**
[DataBarBorder](../../com.aspose.cells/databarborder)
### getBarFillType() {#getBarFillType--}
```
public int getBarFillType()
```


Ottiene come una barra dati è riempita di colore.

Vedi [DataBarFillType](../../com.aspose.cells/databarfilltype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Ottiene il colore di questo DataBar.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDirection() {#getDirection--}
```
public int getDirection()
```


Ottiene la direzione in cui la barra dati è visualizzata.

Vedi [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```


Ottiene l'oggetto valore massimo di questo DataBar. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Min.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Rappresenta la lunghezza massima della barra dati.

**Returns:**
int
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```


Ottiene l'oggetto valore minimo di questo DataBar. Non è possibile impostare null o CFValueObject con tipo FormatConditionValueType.Max.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinLength() {#getMinLength--}
```
public int getMinLength()
```


Rappresenta la lunghezza minima della barra dati.

**Returns:**
int
### getNegativeBarFormat() {#getNegativeBarFormat--}
```
public NegativeBarFormat getNegativeBarFormat()
```


Ottiene l'oggetto NegativeBarFormat associato a una regola di formattazione condizionale barra dati.

**Returns:**
[NegativeBarFormat](../../com.aspose.cells/negativebarformat)
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Ottiene l'indicatore che indica se mostrare i valori delle celle su cui è applicata questa barra dati. Il valore predefinito è true.

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




### setAxisColor(Color value) {#setAxisColor-com.aspose.cells.Color-}
```
public void setAxisColor(Color value)
```


Ottiene il colore dell'asse per le celle con formattazione condizionale come barre dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setAxisPosition(int value) {#setAxisPosition-int-}
```
public void setAxisPosition(int value)
```


Imposta la posizione dell'asse delle barre dati specificate da una regola di formattazione condizionale.

Vedi [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBarFillType(int value) {#setBarFillType-int-}
```
public void setBarFillType(int value)
```


Imposta come una barra dati è riempita di colore.

Vedi [DataBarFillType](../../com.aspose.cells/databarfilltype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Imposta il colore di questo DataBar.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDirection(int value) {#setDirection-int-}
```
public void setDirection(int value)
```


Imposta la direzione in cui la barra dati è visualizzata.

Vedi [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Rappresenta la lunghezza massima della barra dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMinLength(int value) {#setMinLength-int-}
```
public void setMinLength(int value)
```


Rappresenta la lunghezza minima della barra dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Imposta il flag che indica se mostrare i valori delle celle su cui è applicata questa barra dei dati. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### toImage(Cell cell, ImageOrPrintOptions imgOpts) {#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(Cell cell, ImageOrPrintOptions imgOpts)
```


Renderizza la barra dati nella cella in un array di byte dell'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Indica la barra dei dati nella cella da renderizzare |
| imgOpts | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions contiene alcune proprietà dell'immagine di output |

**Returns:**
byte[] -
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

