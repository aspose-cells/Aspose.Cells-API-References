---
title: "Zeile"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine einzelne Zeile in einem Arbeitsblatt dar."
type: docs
url: /de/java/com.aspose.cells/row/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Row implements Iterable
```

Stellt eine einzelne Zeile in einem Arbeitsblatt dar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
          //Apply Style to first row
         row.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Wendet Formate für eine gesamte Zeile an. |
| [copySettings(Row source, boolean checkStyle)](#copySettings-com.aspose.cells.Row-boolean-) | Kopiert Einstellungen der Zeile, wie Stil, Höhe, Sichtbarkeit, ...usw. |
| [equals(Row row)](#equals-com.aspose.cells.Row-) | Überprüft, ob dieses Objekt sich auf dieselbe Zeile wie ein anderes Zeilenobjekt bezieht. |
| [equals(Object obj)](#equals-java.lang.Object-) | Überprüft, ob dieses Objekt sich auf dieselbe Zeile wie ein anderes bezieht. |
| [get(int column)](#get-int-) | Liefert die Zelle. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Holen Sie die Zelle anhand eines bestimmten Index in der Zellenkollektion dieser Zeile. |
| [getCellOrNull(int column)](#getCellOrNull-int-) | Liefert die Zelle oder null am angegebenen Index. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Liefert das erste Zellenobjekt in der Zeile. |
| [getFirstDataCell()](#getFirstDataCell--) | Liefert die erste nicht leere Zelle in der Zeile. |
| [getGroupLevel()](#getGroupLevel--) | Liefert die Gruppenebene der Zeile. |
| [getHeight()](#getHeight--) | Ermittelt die Zeilenhöhe in Punkten. |
| [getIndex()](#getIndex--) | Ermittelt den Index dieser Zeile. |
| [getLastCell()](#getLastCell--) | Ermittelt das letzte Zellenobjekt in der Zeile. |
| [getLastDataCell()](#getLastDataCell--) | Ermittelt die letzte nicht leere Zelle in der Zeile. |
| [getStyle()](#getStyle--) | Ermittelt den Stil dieser Zeile. |
| [hasCustomStyle()](#hasCustomStyle--) | Gibt an, ob diese Zeile benutzerdefinierte Stileinstellungen hat (anders als der Standard, der aus der Arbeitsmappe geerbt wird). |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Gibt an, ob die Zeile Daten enthält. |
| [isCollapsed()](#isCollapsed--) | ob die Zeile zusammengeklappt ist |
| [isHeightMatched()](#isHeightMatched--) | Gibt an, ob die Zeilenhöhe mit der aktuellen Standardschriftart-Einstellung der Arbeitsmappe übereinstimmt. |
| [isHidden()](#isHidden--) | Gibt an, ob die Zeile ausgeblendet ist. |
| [iterator()](#iterator--) | Ermittelt den Zellen-Enumerator |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Ermittelt einen Enumerator, der die Zellen dieser Zeile durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | ob die Zeile zusammengeklappt ist |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Liefert die Gruppenebene der Zeile. |
| [setHeight(double value)](#setHeight-double-) | Setzt die Zeilenhöhe in Punkten. |
| [setHeightMatched(boolean value)](#setHeightMatched-boolean-) | Gibt an, ob die Zeilenhöhe mit der aktuellen Standardschriftart-Einstellung der Arbeitsmappe übereinstimmt. |
| [setHidden(boolean value)](#setHidden-boolean-) | Gibt an, ob die Zeile ausgeblendet ist. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Setzt den Stil dieser Zeile. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Wendet Formate für eine gesamte Zeile an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Das Stilobjekt, das angewendet wird. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags, die angewandte Formatierungseigenschaften anzeigen. |

### copySettings(Row source, boolean checkStyle) {#copySettings-com.aspose.cells.Row-boolean-}
```
public void copySettings(Row source, boolean checkStyle)
```


Kopiert Einstellungen der Zeile, wie Stil, Höhe, Sichtbarkeit, ...usw.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [Row](../../com.aspose.cells/row) | die Quellzeile, deren Einstellungen in diese kopiert werden |
| checkStyle | boolean | ob Stil geprüft und gesammelt wird. Wirkt nur und ist nötig, wenn zwei Zeilenobjekte zu unterschiedlichen Arbeitsmappen gehören und die Stile der beiden Arbeitsmappen unterschiedlich sind. |

### equals(Row row) {#equals-com.aspose.cells.Row-}
```
public boolean equals(Row row)
```


Überprüft, ob dieses Objekt sich auf dieselbe Zeile wie ein anderes Zeilenobjekt bezieht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | ein weiteres Zeilenobjekt |

**Returns:**
boolesch – true, wenn zwei Zeilenobjekte auf dieselbe Zeile verweisen.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Überprüft, ob dieses Objekt sich auf dieselbe Zeile wie ein anderes bezieht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | ein weiteres Objekt |

**Returns:**
boolesch – true, wenn zwei Objekte auf dieselbe Zeile verweisen.
### get(int column) {#get-int-}
```
public Cell get(int column)
```


Liefert die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Der Spaltenindex |

**Returns:**
[Cell](../../com.aspose.cells/cell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public Cell getCellByIndex(int index)
```


Holen Sie die Zelle anhand eines bestimmten Index in der Zellenkollektion dieser Zeile.

**Remarks**

Um alle Zellen sequenziell ohne Änderungen zu durchlaufen, liefert die Verwendung von [iterator()](../../com.aspose.cells/row\#iterator--) eine bessere Leistung als die Verwendung dieser Methode, um Zellen einzeln abzurufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index (Position) der Zelle in der Zellsammlung dieser Zeile. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The Cell object at given position.
### getCellOrNull(int column) {#getCellOrNull-int-}
```
public Cell getCellOrNull(int column)
```


Liefert die Zelle oder null am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Der Spaltenindex |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Returns the cell object if the cell exists. Or returns null if the cell object does not exist.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Liefert das erste Zellenobjekt in der Zeile.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataCell() {#getFirstDataCell--}
```
public Cell getFirstDataCell()
```


Liefert die erste nicht leere Zelle in der Zeile.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Liefert die Gruppenebene der Zeile.

**Returns:**
byte
### getHeight() {#getHeight--}
```
public double getHeight()
```


Ermittelt die Zeilenhöhe in Punkten.

**Returns:**
double
### getIndex() {#getIndex--}
```
public int getIndex()
```


Ermittelt den Index dieser Zeile.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Ermittelt das letzte Zellenobjekt in der Zeile.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataCell() {#getLastDataCell--}
```
public Cell getLastDataCell()
```


Ermittelt die letzte nicht leere Zelle in der Zeile.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Ermittelt den Stil dieser Zeile.

**Remarks**

Das direkte Ändern des zurückgegebenen Style-Objekts hat keine Wirkung für diese Zeile oder für Zellen in dieser Zeile. Sie müssen die Methode [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-) oder [setStyle(Style)](../../com.aspose.cells/row\#setStyle-Style-) aufrufen, um die Änderung auf diese Zeile anzuwenden.

Der Style der Zeile ist der Style, der von den Zellen in dieser Zeile geerbt wird (jene Zellen, die keine benutzerdefinierten Style-Einstellungen haben, wie vorhandene Zellen, deren Style nicht explizit gesetzt wurde, oder solche, die noch nicht instanziiert wurden).

**Returns:**
[Style](../../com.aspose.cells/style)
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Gibt an, ob diese Zeile benutzerdefinierte Stileinstellungen hat (anders als der Standard, der aus der Arbeitsmappe geerbt wird).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Gibt an, ob die Zeile Daten enthält.

**Returns:**
boolean
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


ob die Zeile zusammengeklappt ist

**Returns:**
boolean
### isHeightMatched() {#isHeightMatched--}
```
public boolean isHeightMatched()
```


Gibt an, ob die Zeilenhöhe der aktuellen Standardschriftart des Arbeitsbuchs entspricht. Der Wert true für diese Eigenschaft bedeutet zudem, dass die Zeilenhöhe „automatisch“ ist, ohne dass ein benutzerdefinierter Höhenwert festgelegt wurde.

**Remarks**

Wenn diese Eigenschaft true ist und sich der Inhalt dieser Zeile ändert, muss in der Regel die Zeilenhöhe neu berechnet werden (z. B. durch [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)), um dasselbe Ergebnis zu erhalten, das in MS Excel angezeigt wird, wenn Sie das Arbeitsbuch dort öffnen.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Gibt an, ob die Zeile ausgeblendet ist.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ermittelt den Zellen-Enumerator

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().get(1).iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator – Der Zellen-Enumerator, der alle vorhandenen Zellen in dieser Zeile durchläuft.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Ermittelt einen Enumerator, der die Zellen dieser Zeile durchläuft.

**Remarks**

Wenn die Zeile während der Traversierung mit dem Enumerator geändert wird (durch Vorgänge, die dazu führen können, dass neue Zellen instanziiert oder vorhandene Zellen entfernt werden), sollte ein synchronisierter Enumerator anstelle eines normalen Enumerators verwendet werden, damit die Traversierung ab der Position fortgesetzt werden kann, die direkt nach der zuletzt durch MoveNext() durchlaufenen Zelle liegt. Neben dem Vorteil, dass kein Element übersprungen oder mehrfach durchlaufen wird, hat der synchronisierte Enumerator den Nachteil, dass die Leistung im Vergleich zu einem normalen Enumerator etwas reduziert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| umgekehrt | boolean | ob Zellen in umgekehrter Reihenfolge enumeriert werden |
| synchronisieren | boolean | ob der zurückgegebene Enumerator Änderungen an Zellen in dieser Zeile überprüfen und mit ihr synchronisiert bleiben soll. |

**Returns:**
java.util.Iterator – Der Zellen-Enumerator, der alle vorhandenen Zellen in dieser Zeile durchläuft.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


ob die Zeile zusammengeklappt ist

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Liefert die Gruppenebene der Zeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Setzt die Zeilenhöhe in Punkten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setHeightMatched(boolean value) {#setHeightMatched-boolean-}
```
public void setHeightMatched(boolean value)
```


Gibt an, ob die Zeilenhöhe der aktuellen Standardschriftart des Arbeitsbuchs entspricht. Der Wert true für diese Eigenschaft bedeutet zudem, dass die Zeilenhöhe „automatisch“ ist, ohne dass ein benutzerdefinierter Höhenwert festgelegt wurde.

**Remarks**

Wenn diese Eigenschaft true ist und sich der Inhalt dieser Zeile ändert, muss in der Regel die Zeilenhöhe neu berechnet werden (z. B. durch [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)), um dasselbe Ergebnis zu erhalten, das in MS Excel angezeigt wird, wenn Sie das Arbeitsbuch dort öffnen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Gibt an, ob die Zeile ausgeblendet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Setzt den Stil dieser Zeile.

**Remarks**

Diese Methode setzt nur den angegebenen Style als Standard-Style für diese Zeile, ohne die Style-Einstellungen für vorhandene Zellen in dieser Zeile zu ändern. Um die Style-Einstellungen vorhandener Zellen gleichzeitig auf den angegebenen Style zu aktualisieren, verwenden Sie bitte [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | der Style, der als Standard-Style für Zellen in dieser Zeile verwendet werden soll. |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

