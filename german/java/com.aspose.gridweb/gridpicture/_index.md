---
title: "GridPicture"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das ein einzelnes Bild in einer Tabellenkalkulation darstellt."
type: docs
url: /de/java/com.aspose.gridweb/gridpicture/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridPicture implements IGridSave
```

Kapselt das Objekt, das ein einzelnes Bild in einer Tabellenkalkulation darstellt.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Fügt dem Shape einen Hyperlink hinzu. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Verschiebt das Bild in die obere rechte Ecke. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Gibt den beschreibenden (alternativen) Textstring des [GridShape](../../com.aspose.gridweb/gridshape)-Objekts zurück oder setzt ihn. |
| [getBorderLineColor()](#getBorderLineColor--) | Stellt die [Color](../../com.aspose.cells/color) der Rahmenlinie eines Bildes dar. |
| [getBorderWeight()](#getBorderWeight--) | Liefert die Stärke der Rahmenlinie eines Bildes in pt. |
| [getBottom()](#getBottom--) | Stellt die Breite des vertikalen Versatzes der Form von ihrer unteren Ecke in Pixeln dar. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Ruft die Daten des Bildes ab. |
| [getHeight()](#getHeight--) | Stellt die Höhe der Form in Pixeln dar. |
| [getHeightCM()](#getHeightCM--) | Stellt die Höhe der Form in Zoll dar. |
| [getHeightInch()](#getHeightInch--) | Stellt die Höhe der Form in Zoll dar. |
| [getHeightPt()](#getHeightPt--) | Stellt die Höhe der Form in Punkt dar. |
| [getHeightScale()](#getHeightScale--) | Ruft die Höhenskalierung in Prozent der ursprünglichen Bildhöhe ab. |
| [getHtmlText()](#getHtmlText--) | Liefert den html-String, der Daten und einige Formatierungen in diesem Textbox enthält. |
| [getHyperlink()](#getHyperlink--) | Ruft den Hyperlink der Form ab. |
| [getID()](#getID--) | Liefert / setzt die ID des Bildes. |
| [getImageFormat()](#getImageFormat--) | Liefert das Bildformat des Bildes. |
| [getLeft()](#getLeft--) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Pixeln. |
| [getLeftCM()](#getLeftCM--) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zentimetern. |
| [getLeftInch()](#getLeftInch--) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zoll. |
| [getLeftToCorner()](#getLeftToCorner--) | Stellt den horizontalen Versatz der shape vom linken Rand des Arbeitsblatts dar, in Pixeln. |
| [getLinkedCell()](#getLinkedCell--) | Ermittelt den Arbeitsblattbereich, der mit dem Wert des Steuerelements verknüpft ist. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Ermittelt den horizontalen Versatz der Form von ihrer unteren rechten Eckspalte. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Ermittelt den vertikalen Versatz der Form von ihrer unteren rechten Eckzeile. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Stellt den Spaltenindex der unteren rechten Ecke dar. |
| [getLowerRightRow()](#getLowerRightRow--) | Stellt den Zeilenindex der unteren rechten Ecke dar. |
| [getName()](#getName--) | Ermittelt den Namen der Form. |
| [getOriginalHeight()](#getOriginalHeight--) | Liefert die ursprüngliche Höhe des Bildes. |
| [getOriginalHeightCM()](#getOriginalHeightCM--) | Liefert die ursprüngliche Höhe des Bildes in Zentimetern. |
| [getOriginalHeightInch()](#getOriginalHeightInch--) | Liefert die ursprüngliche Höhe des Bildes in Zoll. |
| [getOriginalWidth()](#getOriginalWidth--) | Liefert die ursprüngliche Breite des Bildes. |
| [getOriginalWidthCM()](#getOriginalWidthCM--) | Liefert die ursprüngliche Breite des Bildes in Zentimetern. |
| [getOriginalWidthInch()](#getOriginalWidthInch--) | Liefert die ursprüngliche Breite des Bildes in Zoll. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Gibt an, ob die Form relativ zur Originalbildgröße ist. |
| [getRight()](#getRight--) | Stellt die Breite des horizontalen Versatzes der Form von ihrer unteren rechten Eckspalte dar, in Einheiten von Pixeln. |
| [getRotationAngle()](#getRotationAngle--) | Ermittelt die Drehung der Form. |
| [getSourceFullName()](#getSourceFullName--) | Ermittelt den Pfad und den Namen der Quelldatei für das verknüpfte Bild. |
| [getText()](#getText--) | Stellt die Zeichenkette in diesem TextBox-Objekt dar. |
| [getTitle()](#getTitle--) | Gibt den Titel (Beschriftung) des aktuellen Formobjekts an. |
| [getTop()](#getTop--) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Pixeln dar. |
| [getTopCM()](#getTopCM--) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zentimetern dar. |
| [getTopInch()](#getTopInch--) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zoll dar. |
| [getTopToCorner()](#getTopToCorner--) | Stellt den vertikalen Versatz der shape vom oberen Rand des Arbeitsblatts dar, in Pixeln. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Ermittelt den horizontalen Versatz der Form von ihrer oberen linken Eckspalte. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Ermittelt den vertikalen Versatz der Form von ihrer oberen linken Eckzeile. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Stellt den Spaltenindex der oberen linken Ecke dar. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Stellt den Zeilenindex der oberen linken Ecke dar. |
| [getWidth()](#getWidth--) | Stellt die Breite der Form dar, in Einheit Pixel. |
| [getWidthCM()](#getWidthCM--) | Stellt die Breite der Form dar, in Einheit Zentimeter. |
| [getWidthInch()](#getWidthInch--) | Stellt die Breite der Form dar, in Einheit Zoll. |
| [getWidthPt()](#getWidthPt--) | Stellt die Breite der Form dar, in Einheit Punkt. |
| [getWidthScale()](#getWidthScale--) | Ermittelt die Breiten­skalierung, in Prozent der ursprünglichen Bildbreite. |
| [getX()](#getX--) | Liefert den horizontalen Versatz der shape vom linken Rand des Arbeitsblatts, in Pixeln. |
| [getY()](#getY--) | Ermittelt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts, in Einheit Pixel. |
| [getZOrderPosition()](#getZOrderPosition--) | Gibt die Position einer Form in der Z-Reihenfolge zurück. |
| [hasLine()](#hasLine--) | Ermittelt, ob die Linienbegrenzung der Form sichtbar ist. |
| [hashCode()](#hashCode--) |  |
| [isFlippedVertically()](#isFlippedVertically--) | Ermittelt, ob die Form vertikal gespiegelt ist . |
| [isGroup()](#isGroup--) | Gibt an, ob die shape eine Gruppe ist. |
| [isHidden()](#isHidden--) | Gibt an, ob das Objekt sichtbar ist. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True bedeutet, dass Änderungen am Seitenverhältnis nicht erlaubt sind. |
| [isLocked()](#isLocked--) | True, wenn das Objekt gesperrt ist, False, wenn das Objekt geändert werden kann, wenn das Blatt geschützt ist. |
| [isTextWrapped()](#isTextWrapped--) | Ermittelt den Textumbruchtyp der Form, die Text enthält. |
| [move(int upperLeftRow, int upperLeftColumn)](#move-int-int-) | Verschiebt das Bild an einen angegebenen Ort. |
| [moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#moveToRange-int-int-int-int-) | Verschiebt die Form in einen angegebenen Bereich. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeHyperlink()](#removeHyperlink--) | Entfernt den Hyperlink der shape. |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Erstellt das Bild und speichert es in einen Stream. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Gibt den beschreibenden (alternativen) Textstring des [GridShape](../../com.aspose.gridweb/gridshape)-Objekts zurück oder setzt ihn. |
| [setBorderLineColor(Color value)](#setBorderLineColor-com.aspose.gridweb.Color-) | Stellt die [Color](../../com.aspose.cells/color) der Rahmenlinie eines Bildes dar. |
| [setBorderWeight(double value)](#setBorderWeight-double-) | Legt die Stärke der Rahmenlinie eines Bildes in pt fest. |
| [setBottom(int value)](#setBottom-int-) | Stellt die Breite des vertikalen Versatzes der Form von ihrer unteren Ecke in Pixeln dar. |
| [setData(byte[] value)](#setData-byte---) | Ruft die Daten des Bildes ab. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Legt fest, ob die Form vertikal gespiegelt ist. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Legt fest, ob die Linienbegrenzung der Form sichtbar ist. |
| [setHeight(int value)](#setHeight-int-) | Stellt die Höhe der Form in Pixeln dar. |
| [setHeightCM(double value)](#setHeightCM-double-) | Stellt die Höhe der Form in Zoll dar. |
| [setHeightInch(double value)](#setHeightInch-double-) | Stellt die Höhe der Form in Zoll dar. |
| [setHeightPt(double value)](#setHeightPt-double-) | Stellt die Höhe der Form in Punkt dar. |
| [setHeightScale(int value)](#setHeightScale-int-) | Legt die Höhenskala fest, in Prozent der ursprünglichen Bildhöhe. |
| [setHidden(boolean value)](#setHidden-boolean-) | Gibt an, ob das Objekt sichtbar ist. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Setzt den html-String, der Daten und einige Formatierungen in diesem Textbox enthält. |
| [setID(String value)](#setID-java.lang.String-) | Liefert / setzt die ID des Bildes. |
| [setLeft(int value)](#setLeft-int-) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Pixeln. |
| [setLeftCM(double value)](#setLeftCM-double-) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zentimetern. |
| [setLeftInch(double value)](#setLeftInch-double-) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zoll. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Stellt den horizontalen Versatz der shape vom linken Rand des Arbeitsblatts dar, in Pixeln. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Legt den Arbeitsblattbereich fest, der mit dem Wert des Steuerelements verknüpft ist. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True bedeutet, dass Änderungen am Seitenverhältnis nicht erlaubt sind. |
| [setLocked(boolean value)](#setLocked-boolean-) | True, wenn das Objekt gesperrt ist, False, wenn das Objekt geändert werden kann, wenn das Blatt geschützt ist. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Legt den horizontalen Versatz der Form von ihrer unteren rechten Eckspalte fest. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Legt den vertikalen Versatz der Form von ihrer unteren rechten Eckzeile fest. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Stellt den Spaltenindex der unteren rechten Ecke dar. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Stellt den Zeilenindex der unteren rechten Ecke dar. |
| [setName(String value)](#setName-java.lang.String-) | Legt den Namen der Form fest. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Gibt an, ob die Form relativ zur Originalbildgröße ist. |
| [setRight(int value)](#setRight-int-) | Stellt die Breite des horizontalen Versatzes der Form von ihrer unteren rechten Eckspalte dar, in Einheiten von Pixeln. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Legt die Drehung der Form fest. |
| [setSourceFullName(String value)](#setSourceFullName-java.lang.String-) | Legt den Pfad und den Namen der Quelldatei für das verknüpfte Bild fest. |
| [setText(String value)](#setText-java.lang.String-) | Stellt die Zeichenkette in diesem TextBox-Objekt dar. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Legt den Typ des umgebrochenen Textes der Form fest, die Text enthält. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Gibt den Titel (Beschriftung) des aktuellen Formobjekts an. |
| [setTop(int value)](#setTop-int-) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Pixeln dar. |
| [setTopCM(double value)](#setTopCM-double-) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zentimetern dar. |
| [setTopInch(double value)](#setTopInch-double-) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zoll dar. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Stellt den vertikalen Versatz der shape vom oberen Rand des Arbeitsblatts dar, in Pixeln. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Legt den horizontalen Versatz der Form von ihrer oberen linken Spalte fest. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Legt den vertikalen Versatz der Form von ihrer oberen linken Zeile fest. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Stellt den Spaltenindex der oberen linken Ecke dar. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Stellt den Zeilenindex der oberen linken Ecke dar. |
| [setWidth(int value)](#setWidth-int-) | Stellt die Breite der Form dar, in Einheit Pixel. |
| [setWidthCM(double value)](#setWidthCM-double-) | Stellt die Breite der Form dar, in Einheit Zentimeter. |
| [setWidthInch(double value)](#setWidthInch-double-) | Stellt die Breite der Form dar, in Einheit Zoll. |
| [setWidthPt(double value)](#setWidthPt-double-) | Stellt die Breite der Form dar, in Einheit Punkt. |
| [setWidthScale(int value)](#setWidthScale-int-) | Legt die Breiten-Skalierung fest, in Prozent der ursprünglichen Bildbreite. |
| [setX(int value)](#setX-int-) | Setzt den horizontalen Versatz der shape vom linken Rand des Arbeitsblatts, in Pixeln. |
| [setY(int value)](#setY-int-) | Legt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts fest, in Einheit von Pixeln. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Gibt die Position einer Form in der Z-Reihenfolge zurück. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public GridHyperlink addHyperlink(String address)
```


Fügt dem Shape einen Hyperlink hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Adresse | java.lang.String | Adresse des Hyperlinks. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - Return the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Verschiebt das Bild in die obere rechte Ecke.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | der Zeilenindex. |
| rightColumn | int | der Spaltenindex. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Gibt den beschreibenden (alternativen) Textstring des [GridShape](../../com.aspose.gridweb/gridshape)-Objekts zurück oder setzt ihn.

**Returns:**
java.lang.String
### getBorderLineColor() {#getBorderLineColor--}
```
public Color getBorderLineColor()
```


Stellt die [Color](../../com.aspose.cells/color) der Rahmenlinie eines Bildes dar.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderWeight() {#getBorderWeight--}
```
public double getBorderWeight()
```


Liefert die Stärke der Rahmenlinie eines Bildes in pt.

**Returns:**
double
### getBottom() {#getBottom--}
```
public int getBottom()
```


Stellt die Breite des vertikalen Versatzes der Form von ihrer unteren Ecke in Pixeln dar.

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


Ruft die Daten des Bildes ab.

**Returns:**
byte[]
### getHeight() {#getHeight--}
```
public int getHeight()
```


Stellt die Höhe der Form in Pixeln dar.

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Stellt die Höhe der Form in Zoll dar.

**Returns:**
double
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Stellt die Höhe der Form in Zoll dar.

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


Stellt die Höhe der Form in Punkt dar.

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


Ermittelt die Höhenskala, in Prozent der ursprünglichen Bildhöhe. Wenn das Shape kein Bild ist, gibt die HeightScale property nur 100 zurück;

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


Liefert den html-String, der Daten und einige Formatierungen in diesem Textbox enthält.

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public GridHyperlink getHyperlink()
```


Ruft den Hyperlink der Form ab.

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink)
### getID() {#getID--}
```
public String getID()
```


Liefert / setzt die ID des Bildes.

**Returns:**
java.lang.String
### getImageFormat() {#getImageFormat--}
```
public int getImageFormat()
```


Liefert das Bildformat des Bildes.

Siehe [GridImageType](../../com.aspose.gridweb/gridimagetype).

**Returns:**
int
### getLeft() {#getLeft--}
```
public int getLeft()
```


Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Pixeln.

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zentimetern.

**Returns:**
double
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zoll.

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Stellt den horizontalen Versatz der shape vom linken Rand des Arbeitsblatts dar, in Pixeln.

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Ermittelt den Arbeitsblattbereich, der mit dem Wert des Steuerelements verknüpft ist.

**Returns:**
java.lang.String
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Liefert den horizontalen Versatz der shape von ihrer unteren rechten Eckspalte. Der Wertebereich liegt zwischen 0 und 1024.

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


Liefert den vertikalen Versatz der shape von ihrer unteren rechten Eckzeile. Der Wertebereich liegt zwischen 0 und 256.

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


Stellt den Spaltenindex der unteren rechten Ecke dar.

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


Stellt den Zeilenindex der unteren rechten Ecke dar.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Ermittelt den Namen der Form.

**Returns:**
java.lang.String
### getOriginalHeight() {#getOriginalHeight--}
```
public int getOriginalHeight()
```


Liefert die ursprüngliche Höhe des Bildes.

**Returns:**
int
### getOriginalHeightCM() {#getOriginalHeightCM--}
```
public double getOriginalHeightCM()
```


Liefert die ursprüngliche Höhe des Bildes in Zentimetern.

**Returns:**
double
### getOriginalHeightInch() {#getOriginalHeightInch--}
```
public double getOriginalHeightInch()
```


Liefert die ursprüngliche Höhe des Bildes in Zoll.

**Returns:**
double
### getOriginalWidth() {#getOriginalWidth--}
```
public int getOriginalWidth()
```


Liefert die ursprüngliche Breite des Bildes.

**Returns:**
int
### getOriginalWidthCM() {#getOriginalWidthCM--}
```
public double getOriginalWidthCM()
```


Liefert die ursprüngliche Breite des Bildes in Zentimetern.

**Returns:**
double
### getOriginalWidthInch() {#getOriginalWidthInch--}
```
public double getOriginalWidthInch()
```


Liefert die ursprüngliche Breite des Bildes in Zoll.

**Returns:**
double
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


Gibt an, ob die Form relativ zur Originalbildgröße ist.

**Returns:**
boolean
### getRight() {#getRight--}
```
public int getRight()
```


Stellt die Breite des horizontalen Versatzes der Form von ihrer unteren rechten Eckspalte dar, in Einheiten von Pixeln.

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Ermittelt die Drehung der Form.

**Returns:**
double
### getSourceFullName() {#getSourceFullName--}
```
public String getSourceFullName()
```


Ermittelt den Pfad und den Namen der Quelldatei für das verknüpfte Bild.

**Remarks**

Der Standardwert ist ein leerer String. Wenn SourceFullName kein leerer String ist, ist das Bild verknüpft. Wenn SourceFullName kein leerer String ist, aber Data null ist, dann ist das Bild verknüpft und wird nicht in der Datei gespeichert.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Stellt die Zeichenkette in diesem TextBox-Objekt dar.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Gibt den Titel (Beschriftung) des aktuellen Formobjekts an.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Pixeln dar.

**Remarks**

Wenn das Shape im Diagramm ist, stellt es den vertikalen Versatz des Shapes von seiner oberen Kante dar.

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zentimetern dar.

**Returns:**
double
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zoll dar.

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Stellt den vertikalen Versatz der shape vom oberen Rand des Arbeitsblatts dar, in Pixeln.

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


Liefert den horizontalen Versatz der shape von ihrer oberen linken Eckspalte. Der Wertebereich liegt zwischen 0 und 1024.

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


Liefert den vertikalen Versatz der shape von ihrer oberen linken Eckzeile. Der Wertebereich liegt zwischen 0 und 256.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Stellt den Spaltenindex der oberen linken Ecke dar.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Stellt den Zeilenindex der oberen linken Ecke dar.

**Remarks**

Wenn das Shape im Shape oder in der Gruppe ist, wird UpperLeftRow ignoriert.

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Stellt die Breite der Form dar, in Einheit Pixel.

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Stellt die Breite der Form dar, in Einheit Zentimeter.

**Returns:**
double
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Stellt die Breite der Form dar, in Einheit Zoll.

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


Stellt die Breite der Form dar, in Einheit Punkt.

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


Ermittelt die Breiten­skala, in Prozent der ursprünglichen Bildbreite. Wenn das Shape kein Bild ist, gibt die WidthScale property nur 100 zurück;

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Liefert den horizontalen Versatz der shape vom linken Rand des Arbeitsblatts, in Pixeln.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Ermittelt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts, in Einheit Pixel.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Gibt die Position einer Form in der Z-Reihenfolge zurück.

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


Ermittelt, ob die Linienbegrenzung der Form sichtbar ist.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


Ermittelt, ob die Form vertikal gespiegelt ist .

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


Gibt an, ob die shape eine Gruppe ist.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Gibt an, ob das Objekt sichtbar ist.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True bedeutet, dass Änderungen am Seitenverhältnis nicht erlaubt sind.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


True, wenn das Objekt gesperrt ist, False, wenn das Objekt geändert werden kann, wenn das Blatt geschützt ist.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Ermittelt den Textumbruchtyp der Form, die Text enthält.

**Returns:**
boolean
### move(int upperLeftRow, int upperLeftColumn) {#move-int-int-}
```
public void move(int upperLeftRow, int upperLeftColumn)
```


Verschiebt das Bild an einen angegebenen Ort.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | int | Index der oberen linken Zeile. |
| upperLeftColumn | int | Index der oberen linken Spalte. |

### moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```


Verschiebt die Form in einen angegebenen Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | int | Index der oberen linken Zeile. |
| upperLeftColumn | int | Index der oberen linken Spalte. |
| lowerRightRow | int | Index der unteren rechten Zeile |
| lowerRightColumn | int | Index der unteren rechten Spalte |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


Entfernt den Hyperlink der shape.

### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


Erstellt das Bild und speichert es in einen Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Gibt den beschreibenden (alternativen) Textstring des [GridShape](../../com.aspose.gridweb/gridshape)-Objekts zurück oder setzt ihn.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setBorderLineColor(Color value) {#setBorderLineColor-com.aspose.gridweb.Color-}
```
public void setBorderLineColor(Color value)
```


Stellt die [Color](../../com.aspose.cells/color) der Rahmenlinie eines Bildes dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderWeight(double value) {#setBorderWeight-double-}
```
public void setBorderWeight(double value)
```


Legt die Stärke der Rahmenlinie eines Bildes in pt fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Stellt die Breite des vertikalen Versatzes der Form von ihrer unteren Ecke in Pixeln dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setData(byte[] value) {#setData-byte---}
```
public void setData(byte[] value)
```


Ruft die Daten des Bildes ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte[] |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Legt fest, ob die Form vertikal gespiegelt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHasLine(boolean value) {#setHasLine-boolean-}
```
public void setHasLine(boolean value)
```


Legt fest, ob die Linienbegrenzung der Form sichtbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Stellt die Höhe der Form in Pixeln dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Stellt die Höhe der Form in Zoll dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Stellt die Höhe der Form in Zoll dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setHeightPt(double value) {#setHeightPt-double-}
```
public void setHeightPt(double value)
```


Stellt die Höhe der Form in Punkt dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setHeightScale(int value) {#setHeightScale-int-}
```
public void setHeightScale(int value)
```


Legt die Höhenskalierung fest, in Prozent der ursprünglichen Bildhöhe. Wenn die Form kein Bild ist, gibt die Eigenschaft HeightScale nur 100 zurück;

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Gibt an, ob das Objekt sichtbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


Setzt den html-String, der Daten und einige Formatierungen in diesem Textbox enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Liefert / setzt die ID des Bildes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setLeft(int value) {#setLeft-int-}
```
public void setLeft(int value)
```


Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLeftCM(double value) {#setLeftCM-double-}
```
public void setLeftCM(double value)
```


Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zentimetern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setLeftInch(double value) {#setLeftInch-double-}
```
public void setLeftInch(double value)
```


Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Stellt den horizontalen Versatz der shape vom linken Rand des Arbeitsblatts dar, in Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Legt den Arbeitsblattbereich fest, der mit dem Wert des Steuerelements verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


True bedeutet, dass Änderungen am Seitenverhältnis nicht erlaubt sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True, wenn das Objekt gesperrt ist, False, wenn das Objekt geändert werden kann, wenn das Blatt geschützt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Legt den horizontalen Versatz der shape von ihrer unteren rechten Eckspaltenposition fest. Der Wertebereich liegt zwischen 0 und 1024.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Legt den vertikalen Versatz der shape von ihrer unteren rechten Eckzeilenposition fest. Der Wertebereich liegt zwischen 0 und 256.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLowerRightColumn(int value) {#setLowerRightColumn-int-}
```
public void setLowerRightColumn(int value)
```


Stellt den Spaltenindex der unteren rechten Ecke dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLowerRightRow(int value) {#setLowerRightRow-int-}
```
public void setLowerRightRow(int value)
```


Stellt den Zeilenindex der unteren rechten Ecke dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Legt den Namen der Form fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setRelativeToOriginalPictureSize(boolean value) {#setRelativeToOriginalPictureSize-boolean-}
```
public void setRelativeToOriginalPictureSize(boolean value)
```


Gibt an, ob die Form relativ zur Originalbildgröße ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRight(int value) {#setRight-int-}
```
public void setRight(int value)
```


Stellt die Breite des horizontalen Versatzes der Form von ihrer unteren rechten Eckspalte dar, in Einheiten von Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Legt die Drehung der Form fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setSourceFullName(String value) {#setSourceFullName-java.lang.String-}
```
public void setSourceFullName(String value)
```


Legt den Pfad und den Namen der Quelldatei für das verknüpfte Bild fest.

**Remarks**

Der Standardwert ist ein leerer String. Wenn SourceFullName kein leerer String ist, ist das Bild verknüpft. Wenn SourceFullName kein leerer String ist, aber Data null ist, dann ist das Bild verknüpft und wird nicht in der Datei gespeichert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Stellt die Zeichenkette in diesem TextBox-Objekt dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Legt den Typ des umgebrochenen Textes der Form fest, die Text enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Gibt den Titel (Beschriftung) des aktuellen Formobjekts an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTop(int value) {#setTop-int-}
```
public void setTop(int value)
```


Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Pixeln dar.

**Remarks**

Wenn das Shape im Diagramm ist, stellt es den vertikalen Versatz des Shapes von seiner oberen Kante dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTopCM(double value) {#setTopCM-double-}
```
public void setTopCM(double value)
```


Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zentimetern dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setTopInch(double value) {#setTopInch-double-}
```
public void setTopInch(double value)
```


Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zoll dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Stellt den vertikalen Versatz der shape vom oberen Rand des Arbeitsblatts dar, in Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Legt den horizontalen Versatz der shape von ihrer oberen linken Eckspaltenposition fest. Der Wertebereich liegt zwischen 0 und 1024.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Legt den vertikalen Versatz der shape von ihrer oberen linken Eckzeilenposition fest. Der Wertebereich liegt zwischen 0 und 256.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setUpperLeftColumn(int value) {#setUpperLeftColumn-int-}
```
public void setUpperLeftColumn(int value)
```


Stellt den Spaltenindex der oberen linken Ecke dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setUpperLeftRow(int value) {#setUpperLeftRow-int-}
```
public void setUpperLeftRow(int value)
```


Stellt den Zeilenindex der oberen linken Ecke dar.

**Remarks**

Wenn das Shape im Shape oder in der Gruppe ist, wird UpperLeftRow ignoriert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Stellt die Breite der Form dar, in Einheit Pixel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Stellt die Breite der Form dar, in Einheit Zentimeter.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Stellt die Breite der Form dar, in Einheit Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWidthPt(double value) {#setWidthPt-double-}
```
public void setWidthPt(double value)
```


Stellt die Breite der Form dar, in Einheit Punkt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWidthScale(int value) {#setWidthScale-int-}
```
public void setWidthScale(int value)
```


Legt die Breiten­skalierung fest, in Prozent der ursprünglichen Bildbreite. Wenn die Form kein Bild ist, gibt die Eigenschaft WidthScale nur 100 zurück;

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Setzt den horizontalen Versatz der shape vom linken Rand des Arbeitsblatts, in Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Legt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts fest, in Einheit von Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Gibt die Position einer Form in der Z-Reihenfolge zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

