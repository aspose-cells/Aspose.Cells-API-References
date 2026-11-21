---
title: "GridPicture"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar en enskild bild i ett kalkylblad."
type: docs
url: /sv/java/com.aspose.gridweb/gridpicture/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridPicture implements IGridSave
```

Inkapslar objektet som representerar en enskild bild i ett kalkylblad.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Lägger till en hyperlänk till formen. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Flyttar bilden till det övre högra hörnet. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Returnerar eller anger den beskrivande (alternativa) textsträngen för [GridShape](../../com.aspose.gridweb/gridshape)-objektet. |
| [getBorderLineColor()](#getBorderLineColor--) | Representerar [Color](../../com.aspose.cells/color) för bildens kantlinje. |
| [getBorderWeight()](#getBorderWeight--) | Hämtar vikten på bildens kantlinje i enheter av pt. |
| [getBottom()](#getBottom--) | Representerar bredden på formens vertikala förskjutning från dess nedre hörnrad, i enhet pixlar. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Hämtar bildens data. |
| [getHeight()](#getHeight--) | Representerar höjden på formen, i enhet pixlar. |
| [getHeightCM()](#getHeightCM--) | Representerar höjden på formen, i enhet tum. |
| [getHeightInch()](#getHeightInch--) | Representerar höjden på formen, i enhet tum. |
| [getHeightPt()](#getHeightPt--) | Representerar höjden på formen, i enhet punkter. |
| [getHeightScale()](#getHeightScale--) | Hämtar höjds‑skalan, i enhet procent av den ursprungliga bildens höjd. |
| [getHtmlText()](#getHtmlText--) | Hämtar HTML-strängen som innehåller data och viss formatering i den här textrutan. |
| [getHyperlink()](#getHyperlink--) | Hämtar hyperlänken för formen. |
| [getID()](#getID--) | Hämtar / anger ID för bilden. |
| [getImageFormat()](#getImageFormat--) | Hämtar bildformatet för bilden. |
| [getLeft()](#getLeft--) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixlar. |
| [getLeftCM()](#getLeftCM--) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet centimeter. |
| [getLeftInch()](#getLeftInch--) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet tum. |
| [getLeftToCorner()](#getLeftToCorner--) | Representerar den horisontella förskjutningen av formen från kalkylbladets vänstra kant, i enheten pixlar. |
| [getLinkedCell()](#getLinkedCell--) | Hämtar kalkylbladsintervallet som är länkat till kontrollens värde. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Hämtar formens horisontella förskjutning från dess nedre högra hörnkolumn. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Hämtar formens vertikala förskjutning från dess nedre högra hörnrad. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Representerar index för nedre högra hörnkolumn. |
| [getLowerRightRow()](#getLowerRightRow--) | Representerar index för nedre högra hörnrad. |
| [getName()](#getName--) | Hämtar namnet på formen. |
| [getOriginalHeight()](#getOriginalHeight--) | Hämtar bildens ursprungliga höjd. |
| [getOriginalHeightCM()](#getOriginalHeightCM--) | Hämtar bildens ursprungliga höjd i centimeter. |
| [getOriginalHeightInch()](#getOriginalHeightInch--) | Hämtar bildens ursprungliga höjd i tum. |
| [getOriginalWidth()](#getOriginalWidth--) | Hämtar bildens ursprungliga bredd. |
| [getOriginalWidthCM()](#getOriginalWidthCM--) | Hämtar bildens ursprungliga bredd i centimeter. |
| [getOriginalWidthInch()](#getOriginalWidthInch--) | Hämtar bildens ursprungliga bredd i tum. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Indikerar om formen är relativ till originalbildens storlek. |
| [getRight()](#getRight--) | Representerar bredden på formens horisontella förskjutning från dess nedre högra hörnkolumn, i enhet pixlar. |
| [getRotationAngle()](#getRotationAngle--) | Hämtar rotationen av formen. |
| [getSourceFullName()](#getSourceFullName--) | Hämtar sökvägen och namnet på källfilen för den länkade bilden. |
| [getText()](#getText--) | Representerar strängen i detta TextBox-objekt. |
| [getTitle()](#getTitle--) | Anger titeln (rubriken) för det aktuella formobjektet. |
| [getTop()](#getTop--) | Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten pixlar. |
| [getTopCM()](#getTopCM--) | Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten centimeter. |
| [getTopInch()](#getTopInch--) | Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten tum. |
| [getTopToCorner()](#getTopToCorner--) | Representerar det vertikala offsetet för formen från kalkylbladets övre kant, i enhet pixlar. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Hämtar formens horisontella förskjutning från dess övre vänstra kolumn. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Hämtar formens vertikala förskjutning från dess övre vänstra rad. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Representerar index för övre vänstra kolumnen. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Representerar radindex för övre vänstra hörnet. |
| [getWidth()](#getWidth--) | Representerar bredden på shape, i enheten pixlar. |
| [getWidthCM()](#getWidthCM--) | Representerar bredden på shape, i enheten centimeter. |
| [getWidthInch()](#getWidthInch--) | Representerar bredden på shape, i enheten tum. |
| [getWidthPt()](#getWidthPt--) | Representerar bredden på shape, i enheten punkt. |
| [getWidthScale()](#getWidthScale--) | Hämtar breddskalan, i enheten procent av den ursprungliga bildens bredd. |
| [getX()](#getX--) | Hämtar det horisontella offsetet för formen från kalkylbladets vänstra kant, i enhet pixlar. |
| [getY()](#getY--) | Hämtar den vertikala förskjutningen av shape från kalkylbladets övre kant, i enheten pixlar. |
| [getZOrderPosition()](#getZOrderPosition--) | Returnerar positionen för en shape i z-ordningen. |
| [hasLine()](#hasLine--) | Hämtar om linjekanten på shape är synlig. |
| [hashCode()](#hashCode--) |  |
| [isFlippedVertically()](#isFlippedVertically--) | Hämtar om shape är vertikalt speglad. |
| [isGroup()](#isGroup--) | Anger om formen är en grupp. |
| [isHidden()](#isHidden--) | Indikerar om objektet är synligt. |
| [isLockAspectRatio()](#isLockAspectRatio--) | Sant betyder att förändringar i bildförhållandet inte tillåts. |
| [isLocked()](#isLocked--) | Sant om objektet är låst, falskt om objektet kan ändras när bladet är skyddat. |
| [isTextWrapped()](#isTextWrapped--) | Hämtar den typ av textomslag för formen som innehåller text. |
| [move(int upperLeftRow, int upperLeftColumn)](#move-int-int-) | Flyttar bilden till en angiven plats. |
| [moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#moveToRange-int-int-int-int-) | Flyttar formen till ett angivet område. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeHyperlink()](#removeHyperlink--) | Ta bort hyperlänken för formen. |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Skapar bilden och sparar den till en ström. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Returnerar eller anger den beskrivande (alternativa) textsträngen för [GridShape](../../com.aspose.gridweb/gridshape)-objektet. |
| [setBorderLineColor(Color value)](#setBorderLineColor-com.aspose.gridweb.Color-) | Representerar [Color](../../com.aspose.cells/color) för bildens kantlinje. |
| [setBorderWeight(double value)](#setBorderWeight-double-) | Ställer in tjockleken på bildens kantlinje i enheter av pt. |
| [setBottom(int value)](#setBottom-int-) | Representerar bredden på formens vertikala förskjutning från dess nedre hörnrad, i enhet pixlar. |
| [setData(byte[] value)](#setData-byte---) | Hämtar bildens data. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Ställer in om formen är vertikalt speglad. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Ställer in att linjekanten på formen är synlig. |
| [setHeight(int value)](#setHeight-int-) | Representerar höjden på formen, i enhet pixlar. |
| [setHeightCM(double value)](#setHeightCM-double-) | Representerar höjden på formen, i enhet tum. |
| [setHeightInch(double value)](#setHeightInch-double-) | Representerar höjden på formen, i enhet tum. |
| [setHeightPt(double value)](#setHeightPt-double-) | Representerar höjden på formen, i enhet punkter. |
| [setHeightScale(int value)](#setHeightScale-int-) | Ställer in höjds-skalan i procent av den ursprungliga bildens höjd. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indikerar om objektet är synligt. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Ställer in HTML-strängen som innehåller data och viss formatering i den här textrutan. |
| [setID(String value)](#setID-java.lang.String-) | Hämtar / anger ID för bilden. |
| [setLeft(int value)](#setLeft-int-) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixlar. |
| [setLeftCM(double value)](#setLeftCM-double-) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet centimeter. |
| [setLeftInch(double value)](#setLeftInch-double-) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet tum. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Representerar den horisontella förskjutningen av formen från kalkylbladets vänstra kant, i enheten pixlar. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Ställer in kalkylbladsområdet som är länkat till kontrollens värde. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | Sant betyder att förändringar i bildförhållandet inte tillåts. |
| [setLocked(boolean value)](#setLocked-boolean-) | Sant om objektet är låst, falskt om objektet kan ändras när bladet är skyddat. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Ställer in formens horisontella förskjutning från dess nedre högra kolumn. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Ställer in formens vertikala förskjutning från dess nedre högra rad. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Representerar index för nedre högra hörnkolumn. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Representerar index för nedre högra hörnrad. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på formen. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Indikerar om formen är relativ till originalbildens storlek. |
| [setRight(int value)](#setRight-int-) | Representerar bredden på formens horisontella förskjutning från dess nedre högra hörnkolumn, i enhet pixlar. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Ställer in rotationen av formen. |
| [setSourceFullName(String value)](#setSourceFullName-java.lang.String-) | Ställer in sökvägen och namnet på källfilen för den länkade bilden. |
| [setText(String value)](#setText-java.lang.String-) | Representerar strängen i detta TextBox-objekt. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Ställer in typen av textbrytning för formen som innehåller text. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Anger titeln (rubriken) för det aktuella formobjektet. |
| [setTop(int value)](#setTop-int-) | Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten pixlar. |
| [setTopCM(double value)](#setTopCM-double-) | Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten centimeter. |
| [setTopInch(double value)](#setTopInch-double-) | Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten tum. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Representerar det vertikala offsetet för formen från kalkylbladets övre kant, i enhet pixlar. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Ställer in formens horisontella förskjutning från dess övre vänstra kolumn. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Ställer in formens vertikala förskjutning från dess övre vänstra rad. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Representerar index för övre vänstra kolumnen. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Representerar radindex för övre vänstra hörnet. |
| [setWidth(int value)](#setWidth-int-) | Representerar bredden på shape, i enheten pixlar. |
| [setWidthCM(double value)](#setWidthCM-double-) | Representerar bredden på shape, i enheten centimeter. |
| [setWidthInch(double value)](#setWidthInch-double-) | Representerar bredden på shape, i enheten tum. |
| [setWidthPt(double value)](#setWidthPt-double-) | Representerar bredden på shape, i enheten punkt. |
| [setWidthScale(int value)](#setWidthScale-int-) | Ställer in breddskalan, i enheten procent av den ursprungliga bildens bredd. |
| [setX(int value)](#setX-int-) | Ställer in det horisontella offsetet för formen från kalkylbladets vänstra kant, i enhet pixlar. |
| [setY(int value)](#setY-int-) | Ställer in den vertikala förskjutningen för formen från kalkylbladets övre kant, i enheten pixlar. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Returnerar positionen för en shape i z-ordningen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public GridHyperlink addHyperlink(String address)
```


Lägger till en hyperlänk till formen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| adress | java.lang.String | Adress för hyperlänken. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - Return the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Flyttar bilden till det övre högra hörnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | radindexet. |
| rightColumn | int | kolumnens index. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Returnerar eller anger den beskrivande (alternativa) textsträngen för [GridShape](../../com.aspose.gridweb/gridshape)-objektet.

**Returns:**
java.lang.String
### getBorderLineColor() {#getBorderLineColor--}
```
public Color getBorderLineColor()
```


Representerar [Color](../../com.aspose.cells/color) för bildens kantlinje.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderWeight() {#getBorderWeight--}
```
public double getBorderWeight()
```


Hämtar vikten på bildens kantlinje i enheter av pt.

**Returns:**
double
### getBottom() {#getBottom--}
```
public int getBottom()
```


Representerar bredden på formens vertikala förskjutning från dess nedre hörnrad, i enhet pixlar.

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


Hämtar bildens data.

**Returns:**
byte[]
### getHeight() {#getHeight--}
```
public int getHeight()
```


Representerar höjden på formen, i enhet pixlar.

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Representerar höjden på formen, i enhet tum.

**Returns:**
double
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Representerar höjden på formen, i enhet tum.

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


Representerar höjden på formen, i enhet punkter.

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


Hämtar höjds-skalan, i enhet procent av den ursprungliga bildens höjd. Om formen inte är en bild, returnerar HeightScale‑egenskapen endast 100;

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


Hämtar HTML-strängen som innehåller data och viss formatering i den här textrutan.

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public GridHyperlink getHyperlink()
```


Hämtar hyperlänken för formen.

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink)
### getID() {#getID--}
```
public String getID()
```


Hämtar / anger ID för bilden.

**Returns:**
java.lang.String
### getImageFormat() {#getImageFormat--}
```
public int getImageFormat()
```


Hämtar bildformatet för bilden.

Se [GridImageType](../../com.aspose.gridweb/gridimagetype).

**Returns:**
int
### getLeft() {#getLeft--}
```
public int getLeft()
```


Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixlar.

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet centimeter.

**Returns:**
double
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet tum.

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Representerar den horisontella förskjutningen av formen från kalkylbladets vänstra kant, i enheten pixlar.

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Hämtar kalkylbladsintervallet som är länkat till kontrollens värde.

**Returns:**
java.lang.String
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Hämtar formens horisontella offset från dess nedre högra hörnkolumn. Värdeintervallet är 0 till 1024.

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


Hämtar formens vertikala offset från dess nedre högra hörnrad. Värdeintervallet är 0 till 256.

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


Representerar index för nedre högra hörnkolumn.

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


Representerar index för nedre högra hörnrad.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på formen.

**Returns:**
java.lang.String
### getOriginalHeight() {#getOriginalHeight--}
```
public int getOriginalHeight()
```


Hämtar bildens ursprungliga höjd.

**Returns:**
int
### getOriginalHeightCM() {#getOriginalHeightCM--}
```
public double getOriginalHeightCM()
```


Hämtar bildens ursprungliga höjd i centimeter.

**Returns:**
double
### getOriginalHeightInch() {#getOriginalHeightInch--}
```
public double getOriginalHeightInch()
```


Hämtar bildens ursprungliga höjd i tum.

**Returns:**
double
### getOriginalWidth() {#getOriginalWidth--}
```
public int getOriginalWidth()
```


Hämtar bildens ursprungliga bredd.

**Returns:**
int
### getOriginalWidthCM() {#getOriginalWidthCM--}
```
public double getOriginalWidthCM()
```


Hämtar bildens ursprungliga bredd i centimeter.

**Returns:**
double
### getOriginalWidthInch() {#getOriginalWidthInch--}
```
public double getOriginalWidthInch()
```


Hämtar bildens ursprungliga bredd i tum.

**Returns:**
double
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


Indikerar om formen är relativ till originalbildens storlek.

**Returns:**
boolean
### getRight() {#getRight--}
```
public int getRight()
```


Representerar bredden på formens horisontella förskjutning från dess nedre högra hörnkolumn, i enhet pixlar.

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Hämtar rotationen av formen.

**Returns:**
double
### getSourceFullName() {#getSourceFullName--}
```
public String getSourceFullName()
```


Hämtar sökvägen och namnet på källfilen för den länkade bilden.

**Remarks**

Standardvärdet är en tom sträng. Om SourceFullName inte är en tom sträng är bilden länkad. Om SourceFullName inte är en tom sträng, men Data är null, är bilden länkad och lagras inte i filen.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Representerar strängen i detta TextBox-objekt.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Anger titeln (rubriken) för det aktuella formobjektet.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten pixlar.

**Remarks**

Om formen är i diagrammet, representerar den vertikala förskjutningen av formen från dess övre kant.

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten centimeter.

**Returns:**
double
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten tum.

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Representerar det vertikala offsetet för formen från kalkylbladets övre kant, i enhet pixlar.

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


Hämtar formens horisontella offset från dess övre vänstra hörnkolumn. Värdeintervallet är 0 till 1024.

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


Hämtar formens vertikala offset från dess övre vänstra hörnrad. Värdeintervallet är 0 till 256.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Representerar index för övre vänstra kolumnen.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Representerar radindex för övre vänstra hörnet.

**Remarks**

Om formen är i en form eller i en grupp, kommer UpperLeftRow att ignoreras.

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Representerar bredden på shape, i enheten pixlar.

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Representerar bredden på shape, i enheten centimeter.

**Returns:**
double
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Representerar bredden på shape, i enheten tum.

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


Representerar bredden på shape, i enheten punkt.

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


Hämtar breddskalan, i enhet procent av den ursprungliga bildens bredd. Om formen inte är en bild, returnerar WidthScale‑egenskapen endast 100;

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Hämtar det horisontella offsetet för formen från kalkylbladets vänstra kant, i enhet pixlar.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Hämtar den vertikala förskjutningen av shape från kalkylbladets övre kant, i enheten pixlar.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Returnerar positionen för en shape i z-ordningen.

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


Hämtar om linjekanten på shape är synlig.

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


Hämtar om shape är vertikalt speglad.

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


Anger om formen är en grupp.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indikerar om objektet är synligt.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


Sant betyder att förändringar i bildförhållandet inte tillåts.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Sant om objektet är låst, falskt om objektet kan ändras när bladet är skyddat.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Hämtar den typ av textomslag för formen som innehåller text.

**Returns:**
boolean
### move(int upperLeftRow, int upperLeftColumn) {#move-int-int-}
```
public void move(int upperLeftRow, int upperLeftColumn)
```


Flyttar bilden till en angiven plats.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftRow | int | Övre vänstra radindex. |
| upperLeftColumn | int | Övre vänstra kolumnindex. |

### moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```


Flyttar formen till ett angivet område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftRow | int | Övre vänstra radindex. |
| upperLeftColumn | int | Övre vänstra kolumnindex. |
| lowerRightRow | int | Nedre högra radindex |
| lowerRightColumn | int | Nedre högra kolumnindex |

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


Ta bort hyperlänken för formen.

### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


Skapar bilden och sparar den till en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Returnerar eller anger den beskrivande (alternativa) textsträngen för [GridShape](../../com.aspose.gridweb/gridshape)-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setBorderLineColor(Color value) {#setBorderLineColor-com.aspose.gridweb.Color-}
```
public void setBorderLineColor(Color value)
```


Representerar [Color](../../com.aspose.cells/color) för bildens kantlinje.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderWeight(double value) {#setBorderWeight-double-}
```
public void setBorderWeight(double value)
```


Ställer in tjockleken på bildens kantlinje i enheter av pt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Representerar bredden på formens vertikala förskjutning från dess nedre hörnrad, i enhet pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setData(byte[] value) {#setData-byte---}
```
public void setData(byte[] value)
```


Hämtar bildens data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte[] |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Ställer in om formen är vertikalt speglad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasLine(boolean value) {#setHasLine-boolean-}
```
public void setHasLine(boolean value)
```


Ställer in att linjekanten på formen är synlig.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Representerar höjden på formen, i enhet pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Representerar höjden på formen, i enhet tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Representerar höjden på formen, i enhet tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setHeightPt(double value) {#setHeightPt-double-}
```
public void setHeightPt(double value)
```


Representerar höjden på formen, i enhet punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setHeightScale(int value) {#setHeightScale-int-}
```
public void setHeightScale(int value)
```


Ställer in höjds‑skalan, i procentenhet av den ursprungliga bildens höjd. Om formen inte är en bild returnerar HeightScale‑egenskapen endast 100;

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indikerar om objektet är synligt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


Ställer in HTML-strängen som innehåller data och viss formatering i den här textrutan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Hämtar / anger ID för bilden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setLeft(int value) {#setLeft-int-}
```
public void setLeft(int value)
```


Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLeftCM(double value) {#setLeftCM-double-}
```
public void setLeftCM(double value)
```


Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLeftInch(double value) {#setLeftInch-double-}
```
public void setLeftInch(double value)
```


Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Representerar den horisontella förskjutningen av formen från kalkylbladets vänstra kant, i enheten pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Ställer in kalkylbladsområdet som är länkat till kontrollens värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


Sant betyder att förändringar i bildförhållandet inte tillåts.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Sant om objektet är låst, falskt om objektet kan ändras när bladet är skyddat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Ställer in formens horisontella offset från dess nedre högra hörnkolumn. Värdeintervallet är 0 till 1024.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Ställer in formens vertikala offset från dess nedre högra hörnrad. Värdeintervallet är 0 till 256.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLowerRightColumn(int value) {#setLowerRightColumn-int-}
```
public void setLowerRightColumn(int value)
```


Representerar index för nedre högra hörnkolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLowerRightRow(int value) {#setLowerRightRow-int-}
```
public void setLowerRightRow(int value)
```


Representerar index för nedre högra hörnrad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in namnet på formen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setRelativeToOriginalPictureSize(boolean value) {#setRelativeToOriginalPictureSize-boolean-}
```
public void setRelativeToOriginalPictureSize(boolean value)
```


Indikerar om formen är relativ till originalbildens storlek.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRight(int value) {#setRight-int-}
```
public void setRight(int value)
```


Representerar bredden på formens horisontella förskjutning från dess nedre högra hörnkolumn, i enhet pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Ställer in rotationen av formen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setSourceFullName(String value) {#setSourceFullName-java.lang.String-}
```
public void setSourceFullName(String value)
```


Ställer in sökvägen och namnet på källfilen för den länkade bilden.

**Remarks**

Standardvärdet är en tom sträng. Om SourceFullName inte är en tom sträng är bilden länkad. Om SourceFullName inte är en tom sträng, men Data är null, är bilden länkad och lagras inte i filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Representerar strängen i detta TextBox-objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Ställer in typen av textbrytning för formen som innehåller text.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Anger titeln (rubriken) för det aktuella formobjektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTop(int value) {#setTop-int-}
```
public void setTop(int value)
```


Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten pixlar.

**Remarks**

Om formen är i diagrammet, representerar den vertikala förskjutningen av formen från dess övre kant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTopCM(double value) {#setTopCM-double-}
```
public void setTopCM(double value)
```


Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setTopInch(double value) {#setTopInch-double-}
```
public void setTopInch(double value)
```


Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Representerar det vertikala offsetet för formen från kalkylbladets övre kant, i enhet pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Ställer in formens horisontella offset från dess övre vänstra hörnkolumn. Värdeintervallet är 0 till 1024.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Ställer in formens vertikala offset från dess övre vänstra hörnrad. Värdeintervallet är 0 till 256.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setUpperLeftColumn(int value) {#setUpperLeftColumn-int-}
```
public void setUpperLeftColumn(int value)
```


Representerar index för övre vänstra kolumnen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setUpperLeftRow(int value) {#setUpperLeftRow-int-}
```
public void setUpperLeftRow(int value)
```


Representerar radindex för övre vänstra hörnet.

**Remarks**

Om formen är i en form eller i en grupp, kommer UpperLeftRow att ignoreras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Representerar bredden på shape, i enheten pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Representerar bredden på shape, i enheten centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Representerar bredden på shape, i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWidthPt(double value) {#setWidthPt-double-}
```
public void setWidthPt(double value)
```


Representerar bredden på shape, i enheten punkt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWidthScale(int value) {#setWidthScale-int-}
```
public void setWidthScale(int value)
```


Ställer in breddskalan, i procentenhet av den ursprungliga bildens bredd. Om formen inte är en bild returnerar WidthScale‑egenskapen endast 100;

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Ställer in det horisontella offsetet för formen från kalkylbladets vänstra kant, i enhet pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Ställer in den vertikala förskjutningen för formen från kalkylbladets övre kant, i enheten pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Returnerar positionen för en shape i z-ordningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

