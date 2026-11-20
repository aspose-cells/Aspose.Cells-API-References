---
title: "GridPicture"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta un'unica immagine in un foglio di calcolo."
type: docs
url: /it/java/com.aspose.gridweb/gridpicture/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridPicture implements IGridSave
```

Incapsula l'oggetto che rappresenta un'unica immagine in un foglio di calcolo.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Aggiunge un collegamento ipertestuale alla forma. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Sposta l'immagine nell'angolo in alto a destra. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto [GridShape](../../com.aspose.gridweb/gridshape). |
| [getBorderLineColor()](#getBorderLineColor--) | Rappresenta il [Color](../../com.aspose.cells/color) della linea di bordo di un'immagine. |
| [getBorderWeight()](#getBorderWeight--) | Recupera lo spessore della linea di bordo di un'immagine in unità di pt. |
| [getBottom()](#getBottom--) | Rappresenta la larghezza dello spostamento verticale della forma dalla sua riga d'angolo inferiore, in unità di pixel. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Ottiene i dati dell'immagine. |
| [getHeight()](#getHeight--) | Rappresenta l'altezza della forma, in unità di pixel. |
| [getHeightCM()](#getHeightCM--) | Rappresenta l'altezza della forma, in unità di pollici. |
| [getHeightInch()](#getHeightInch--) | Rappresenta l'altezza della forma, in unità di pollici. |
| [getHeightPt()](#getHeightPt--) | Rappresenta l'altezza della forma, in unità di punti. |
| [getHeightScale()](#getHeightScale--) | Ottiene la scala di altezza, in unità di percentuale dell'altezza originale dell'immagine. |
| [getHtmlText()](#getHtmlText--) | Ottiene la stringa HTML che contiene dati e alcune formattazioni in questa casella di testo. |
| [getHyperlink()](#getHyperlink--) | Ottiene il collegamento ipertestuale della forma. |
| [getID()](#getID--) | Ottiene / imposta l'ID dell'immagine. |
| [getImageFormat()](#getImageFormat--) | Recupera il formato immagine dell'immagine. |
| [getLeft()](#getLeft--) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel. |
| [getLeftCM()](#getLeftCM--) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di centimetri. |
| [getLeftInch()](#getLeftInch--) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pollici. |
| [getLeftToCorner()](#getLeftToCorner--) | Rappresenta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel. |
| [getLinkedCell()](#getLinkedCell--) | Ottiene l'intervallo del foglio di lavoro collegato al valore del controllo. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Ottiene lo spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Ottiene lo spostamento verticale della forma dalla riga dell'angolo inferiore destro. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Rappresenta l'indice della colonna dell'angolo inferiore destro. |
| [getLowerRightRow()](#getLowerRightRow--) | Rappresenta l'indice della riga dell'angolo inferiore destro. |
| [getName()](#getName--) | Ottiene il nome della forma. |
| [getOriginalHeight()](#getOriginalHeight--) | Recupera l'altezza originale dell'immagine. |
| [getOriginalHeightCM()](#getOriginalHeightCM--) | Recupera l'altezza originale dell'immagine, in unità di centimetri. |
| [getOriginalHeightInch()](#getOriginalHeightInch--) | Restituisce l'altezza originale dell'immagine, in unità di pollici. |
| [getOriginalWidth()](#getOriginalWidth--) | Restituisce la larghezza originale dell'immagine. |
| [getOriginalWidthCM()](#getOriginalWidthCM--) | Restituisce la larghezza originale dell'immagine, in unità di centimetri. |
| [getOriginalWidthInch()](#getOriginalWidthInch--) | Restituisce la larghezza originale dell'immagine, in unità di pollici. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Indica se la forma è relativa alle dimensioni originali dell'immagine. |
| [getRight()](#getRight--) | Rappresenta la larghezza dello spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro, in unità di pixel. |
| [getRotationAngle()](#getRotationAngle--) | Ottiene la rotazione della forma. |
| [getSourceFullName()](#getSourceFullName--) | Restituisce il percorso e il nome del file sorgente per l'immagine collegata. |
| [getText()](#getText--) | Rappresenta la stringa in questo oggetto TextBox. |
| [getTitle()](#getTitle--) | Specifica il titolo (didascalia) dell'oggetto forma corrente. |
| [getTop()](#getTop--) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pixel. |
| [getTopCM()](#getTopCM--) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di centimetri. |
| [getTopInch()](#getTopInch--) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pollici. |
| [getTopToCorner()](#getTopToCorner--) | Rappresenta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Restituisce lo spostamento orizzontale della forma dalla colonna dell'angolo superiore sinistro. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Restituisce lo spostamento verticale della forma dalla riga dell'angolo superiore sinistro. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Rappresenta l'indice della colonna dell'angolo superiore sinistro. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Rappresenta l'indice di riga dell'angolo in alto a sinistra. |
| [getWidth()](#getWidth--) | Rappresenta la larghezza della forma, in unità di pixel. |
| [getWidthCM()](#getWidthCM--) | Rappresenta la larghezza della forma, in unità di centimetri. |
| [getWidthInch()](#getWidthInch--) | Rappresenta la larghezza della forma, in unità di pollice. |
| [getWidthPt()](#getWidthPt--) | Rappresenta la larghezza della forma, in unità di punto. |
| [getWidthScale()](#getWidthScale--) | Ottiene la scala di larghezza, in unità di percentuale della larghezza originale dell'immagine. |
| [getX()](#getX--) | Ottiene lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel. |
| [getY()](#getY--) | Ottiene lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel. |
| [getZOrderPosition()](#getZOrderPosition--) | Restituisce la posizione di una forma nell'ordine Z. |
| [hasLine()](#hasLine--) | Ottiene se il bordo della linea della forma è visibile. |
| [hashCode()](#hashCode--) |  |
| [isFlippedVertically()](#isFlippedVertically--) | Ottiene se la forma è capovolta verticalmente . |
| [isGroup()](#isGroup--) | Indica se la forma è un gruppo. |
| [isHidden()](#isHidden--) | Indica se l'oggetto è visibile. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True indica che non è consentito modificare le proporzioni. |
| [isLocked()](#isLocked--) | True se l'oggetto è bloccato, False se l'oggetto può essere modificato quando il foglio è protetto. |
| [isTextWrapped()](#isTextWrapped--) | Ottiene il tipo di avvolgimento del testo della forma che contiene testo. |
| [move(int upperLeftRow, int upperLeftColumn)](#move-int-int-) | Sposta l'immagine in una posizione specificata. |
| [moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#moveToRange-int-int-int-int-) | Sposta la forma in un intervallo specificato. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeHyperlink()](#removeHyperlink--) | Rimuovi il collegamento ipertestuale della forma. |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Crea l'immagine e la salva in uno stream. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto [GridShape](../../com.aspose.gridweb/gridshape). |
| [setBorderLineColor(Color value)](#setBorderLineColor-com.aspose.gridweb.Color-) | Rappresenta il [Color](../../com.aspose.cells/color) della linea di bordo di un'immagine. |
| [setBorderWeight(double value)](#setBorderWeight-double-) | Imposta lo spessore della linea di bordo di un'immagine in unità di pt. |
| [setBottom(int value)](#setBottom-int-) | Rappresenta la larghezza dello spostamento verticale della forma dalla sua riga d'angolo inferiore, in unità di pixel. |
| [setData(byte[] value)](#setData-byte---) | Ottiene i dati dell'immagine. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Imposta se la forma è capovolta verticalmente. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Imposta che il bordo della forma sia visibile. |
| [setHeight(int value)](#setHeight-int-) | Rappresenta l'altezza della forma, in unità di pixel. |
| [setHeightCM(double value)](#setHeightCM-double-) | Rappresenta l'altezza della forma, in unità di pollici. |
| [setHeightInch(double value)](#setHeightInch-double-) | Rappresenta l'altezza della forma, in unità di pollici. |
| [setHeightPt(double value)](#setHeightPt-double-) | Rappresenta l'altezza della forma, in unità di punti. |
| [setHeightScale(int value)](#setHeightScale-int-) | Imposta la scala di altezza, in unità di percentuale dell'altezza originale dell'immagine. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indica se l'oggetto è visibile. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Imposta la stringa HTML che contiene dati e alcune formattazioni in questa casella di testo. |
| [setID(String value)](#setID-java.lang.String-) | Ottiene / imposta l'ID dell'immagine. |
| [setLeft(int value)](#setLeft-int-) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel. |
| [setLeftCM(double value)](#setLeftCM-double-) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di centimetri. |
| [setLeftInch(double value)](#setLeftInch-double-) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pollici. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Rappresenta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Imposta l'intervallo del foglio di lavoro collegato al valore del controllo. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True indica che non è consentito modificare le proporzioni. |
| [setLocked(boolean value)](#setLocked-boolean-) | True se l'oggetto è bloccato, False se l'oggetto può essere modificato quando il foglio è protetto. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Imposta lo spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Imposta lo spostamento verticale della forma dalla riga dell'angolo inferiore destro. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Rappresenta l'indice della colonna dell'angolo inferiore destro. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Rappresenta l'indice della riga dell'angolo inferiore destro. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome della forma. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Indica se la forma è relativa alle dimensioni originali dell'immagine. |
| [setRight(int value)](#setRight-int-) | Rappresenta la larghezza dello spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro, in unità di pixel. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Imposta la rotazione della forma. |
| [setSourceFullName(String value)](#setSourceFullName-java.lang.String-) | Imposta il percorso e il nome del file sorgente per l'immagine collegata. |
| [setText(String value)](#setText-java.lang.String-) | Rappresenta la stringa in questo oggetto TextBox. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Imposta il tipo di avvolgimento del testo della forma che contiene testo. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Specifica il titolo (didascalia) dell'oggetto forma corrente. |
| [setTop(int value)](#setTop-int-) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pixel. |
| [setTopCM(double value)](#setTopCM-double-) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di centimetri. |
| [setTopInch(double value)](#setTopInch-double-) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pollici. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Rappresenta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Imposta lo spostamento orizzontale della forma dalla colonna dell'angolo in alto a sinistra. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Imposta lo spostamento verticale della forma dalla riga dell'angolo in alto a sinistra. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Rappresenta l'indice della colonna dell'angolo superiore sinistro. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Rappresenta l'indice di riga dell'angolo in alto a sinistra. |
| [setWidth(int value)](#setWidth-int-) | Rappresenta la larghezza della forma, in unità di pixel. |
| [setWidthCM(double value)](#setWidthCM-double-) | Rappresenta la larghezza della forma, in unità di centimetri. |
| [setWidthInch(double value)](#setWidthInch-double-) | Rappresenta la larghezza della forma, in unità di pollice. |
| [setWidthPt(double value)](#setWidthPt-double-) | Rappresenta la larghezza della forma, in unità di punto. |
| [setWidthScale(int value)](#setWidthScale-int-) | Imposta la scala di larghezza, in unità di percentuale della larghezza originale dell'immagine. |
| [setX(int value)](#setX-int-) | Imposta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel. |
| [setY(int value)](#setY-int-) | Imposta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Restituisce la posizione di una forma nell'ordine Z. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public GridHyperlink addHyperlink(String address)
```


Aggiunge un collegamento ipertestuale alla forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indirizzo | java.lang.String | Indirizzo del collegamento ipertestuale. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - Return the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Sposta l'immagine nell'angolo in alto a destra.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | l'indice della riga. |
| rightColumn | int | l'indice della colonna. |

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto [GridShape](../../com.aspose.gridweb/gridshape).

**Returns:**
java.lang.String
### getBorderLineColor() {#getBorderLineColor--}
```
public Color getBorderLineColor()
```


Rappresenta il [Color](../../com.aspose.cells/color) della linea di bordo di un'immagine.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderWeight() {#getBorderWeight--}
```
public double getBorderWeight()
```


Recupera lo spessore della linea di bordo di un'immagine in unità di pt.

**Returns:**
double
### getBottom() {#getBottom--}
```
public int getBottom()
```


Rappresenta la larghezza dello spostamento verticale della forma dalla sua riga d'angolo inferiore, in unità di pixel.

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


Ottiene i dati dell'immagine.

**Returns:**
byte[]
### getHeight() {#getHeight--}
```
public int getHeight()
```


Rappresenta l'altezza della forma, in unità di pixel.

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Rappresenta l'altezza della forma, in unità di pollici.

**Returns:**
double
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Rappresenta l'altezza della forma, in unità di pollici.

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


Rappresenta l'altezza della forma, in unità di punti.

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


Restituisce la scala dell'altezza, in unità di percentuale dell'altezza originale dell'immagine. Se la forma non è un'immagine, la proprietà HeightScale restituisce solo 100;

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


Ottiene la stringa HTML che contiene dati e alcune formattazioni in questa casella di testo.

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public GridHyperlink getHyperlink()
```


Ottiene il collegamento ipertestuale della forma.

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink)
### getID() {#getID--}
```
public String getID()
```


Ottiene / imposta l'ID dell'immagine.

**Returns:**
java.lang.String
### getImageFormat() {#getImageFormat--}
```
public int getImageFormat()
```


Recupera il formato immagine dell'immagine.

Vedi [GridImageType](../../com.aspose.gridweb/gridimagetype).

**Returns:**
int
### getLeft() {#getLeft--}
```
public int getLeft()
```


Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel.

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di centimetri.

**Returns:**
double
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pollici.

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Rappresenta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel.

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Ottiene l'intervallo del foglio di lavoro collegato al valore del controllo.

**Returns:**
java.lang.String
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Ottiene lo spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro. L'intervallo del valore è da 0 a 1024.

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


Ottiene lo spostamento verticale della forma dalla riga dell'angolo inferiore destro. L'intervallo del valore è da 0 a 256.

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


Rappresenta l'indice della colonna dell'angolo inferiore destro.

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


Rappresenta l'indice della riga dell'angolo inferiore destro.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome della forma.

**Returns:**
java.lang.String
### getOriginalHeight() {#getOriginalHeight--}
```
public int getOriginalHeight()
```


Recupera l'altezza originale dell'immagine.

**Returns:**
int
### getOriginalHeightCM() {#getOriginalHeightCM--}
```
public double getOriginalHeightCM()
```


Recupera l'altezza originale dell'immagine, in unità di centimetri.

**Returns:**
double
### getOriginalHeightInch() {#getOriginalHeightInch--}
```
public double getOriginalHeightInch()
```


Restituisce l'altezza originale dell'immagine, in unità di pollici.

**Returns:**
double
### getOriginalWidth() {#getOriginalWidth--}
```
public int getOriginalWidth()
```


Restituisce la larghezza originale dell'immagine.

**Returns:**
int
### getOriginalWidthCM() {#getOriginalWidthCM--}
```
public double getOriginalWidthCM()
```


Restituisce la larghezza originale dell'immagine, in unità di centimetri.

**Returns:**
double
### getOriginalWidthInch() {#getOriginalWidthInch--}
```
public double getOriginalWidthInch()
```


Restituisce la larghezza originale dell'immagine, in unità di pollici.

**Returns:**
double
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


Indica se la forma è relativa alle dimensioni originali dell'immagine.

**Returns:**
boolean
### getRight() {#getRight--}
```
public int getRight()
```


Rappresenta la larghezza dello spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro, in unità di pixel.

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Ottiene la rotazione della forma.

**Returns:**
double
### getSourceFullName() {#getSourceFullName--}
```
public String getSourceFullName()
```


Restituisce il percorso e il nome del file sorgente per l'immagine collegata.

**Remarks**

Il valore predefinito è una stringa vuota. Se SourceFullName non è una stringa vuota, l'immagine è collegata. Se SourceFullName non è una stringa vuota, ma Data è null, allora l'immagine è collegata e non è memorizzata nel file.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Rappresenta la stringa in questo oggetto TextBox.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Specifica il titolo (didascalia) dell'oggetto forma corrente.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pixel.

**Remarks**

Se la forma è nel grafico, rappresenta lo spostamento verticale della forma dal suo bordo superiore.

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di centimetri.

**Returns:**
double
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pollici.

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Rappresenta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel.

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


Ottiene lo spostamento orizzontale della forma dalla colonna dell'angolo superiore sinistro. L'intervallo del valore è da 0 a 1024.

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


Ottiene lo spostamento verticale della forma dalla riga dell'angolo superiore sinistro. L'intervallo del valore è da 0 a 256.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Rappresenta l'indice della colonna dell'angolo superiore sinistro.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Rappresenta l'indice di riga dell'angolo in alto a sinistra.

**Remarks**

Se la forma è nella forma o nel gruppo, UpperLeftRow verrà ignorato.

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Rappresenta la larghezza della forma, in unità di pixel.

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Rappresenta la larghezza della forma, in unità di centimetri.

**Returns:**
double
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Rappresenta la larghezza della forma, in unità di pollice.

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


Rappresenta la larghezza della forma, in unità di punto.

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


Restituisce la scala della larghezza, in unità di percentuale della larghezza originale dell'immagine. Se la forma non è un'immagine, la proprietà WidthScale restituisce solo 100;

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Ottiene lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Ottiene lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Restituisce la posizione di una forma nell'ordine Z.

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


Ottiene se il bordo della linea della forma è visibile.

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


Ottiene se la forma è capovolta verticalmente .

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


Indica se la forma è un gruppo.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indica se l'oggetto è visibile.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True indica che non è consentito modificare le proporzioni.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


True se l'oggetto è bloccato, False se l'oggetto può essere modificato quando il foglio è protetto.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Ottiene il tipo di avvolgimento del testo della forma che contiene testo.

**Returns:**
boolean
### move(int upperLeftRow, int upperLeftColumn) {#move-int-int-}
```
public void move(int upperLeftRow, int upperLeftColumn)
```


Sposta l'immagine in una posizione specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| upperLeftRow | int | Indice della riga in alto a sinistra. |
| upperLeftColumn | int | Indice della colonna in alto a sinistra. |

### moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```


Sposta la forma in un intervallo specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| upperLeftRow | int | Indice della riga in alto a sinistra. |
| upperLeftColumn | int | Indice della colonna in alto a sinistra. |
| lowerRightRow | int | Indice della riga in basso a destra |
| lowerRightColumn | int | Indice della colonna in basso a destra |

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


Rimuovi il collegamento ipertestuale della forma.

### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


Crea l'immagine e la salva in uno stream.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto [GridShape](../../com.aspose.gridweb/gridshape).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setBorderLineColor(Color value) {#setBorderLineColor-com.aspose.gridweb.Color-}
```
public void setBorderLineColor(Color value)
```


Rappresenta il [Color](../../com.aspose.cells/color) della linea di bordo di un'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderWeight(double value) {#setBorderWeight-double-}
```
public void setBorderWeight(double value)
```


Imposta lo spessore della linea di bordo di un'immagine in unità di pt.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Rappresenta la larghezza dello spostamento verticale della forma dalla sua riga d'angolo inferiore, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setData(byte[] value) {#setData-byte---}
```
public void setData(byte[] value)
```


Ottiene i dati dell'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte[] |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Imposta se la forma è capovolta verticalmente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasLine(boolean value) {#setHasLine-boolean-}
```
public void setHasLine(boolean value)
```


Imposta che il bordo della forma sia visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Rappresenta l'altezza della forma, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Rappresenta l'altezza della forma, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Rappresenta l'altezza della forma, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setHeightPt(double value) {#setHeightPt-double-}
```
public void setHeightPt(double value)
```


Rappresenta l'altezza della forma, in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setHeightScale(int value) {#setHeightScale-int-}
```
public void setHeightScale(int value)
```


Imposta la scala dell'altezza, in unità di percentuale dell'altezza originale dell'immagine. Se la forma non è un'immagine, la proprietà HeightScale restituisce solo 100;

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indica se l'oggetto è visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


Imposta la stringa HTML che contiene dati e alcune formattazioni in questa casella di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Ottiene / imposta l'ID dell'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setLeft(int value) {#setLeft-int-}
```
public void setLeft(int value)
```


Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLeftCM(double value) {#setLeftCM-double-}
```
public void setLeftCM(double value)
```


Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di centimetri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLeftInch(double value) {#setLeftInch-double-}
```
public void setLeftInch(double value)
```


Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Rappresenta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Imposta l'intervallo del foglio di lavoro collegato al valore del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


True indica che non è consentito modificare le proporzioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True se l'oggetto è bloccato, False se l'oggetto può essere modificato quando il foglio è protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Imposta lo spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro. L'intervallo del valore è da 0 a 1024.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Imposta lo spostamento verticale della forma dalla riga dell'angolo inferiore destro. L'intervallo del valore è da 0 a 256.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLowerRightColumn(int value) {#setLowerRightColumn-int-}
```
public void setLowerRightColumn(int value)
```


Rappresenta l'indice della colonna dell'angolo inferiore destro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLowerRightRow(int value) {#setLowerRightRow-int-}
```
public void setLowerRightRow(int value)
```


Rappresenta l'indice della riga dell'angolo inferiore destro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome della forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setRelativeToOriginalPictureSize(boolean value) {#setRelativeToOriginalPictureSize-boolean-}
```
public void setRelativeToOriginalPictureSize(boolean value)
```


Indica se la forma è relativa alle dimensioni originali dell'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRight(int value) {#setRight-int-}
```
public void setRight(int value)
```


Rappresenta la larghezza dello spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Imposta la rotazione della forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setSourceFullName(String value) {#setSourceFullName-java.lang.String-}
```
public void setSourceFullName(String value)
```


Imposta il percorso e il nome del file sorgente per l'immagine collegata.

**Remarks**

Il valore predefinito è una stringa vuota. Se SourceFullName non è una stringa vuota, l'immagine è collegata. Se SourceFullName non è una stringa vuota, ma Data è null, allora l'immagine è collegata e non è memorizzata nel file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Rappresenta la stringa in questo oggetto TextBox.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Imposta il tipo di avvolgimento del testo della forma che contiene testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Specifica il titolo (didascalia) dell'oggetto forma corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTop(int value) {#setTop-int-}
```
public void setTop(int value)
```


Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pixel.

**Remarks**

Se la forma è nel grafico, rappresenta lo spostamento verticale della forma dal suo bordo superiore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTopCM(double value) {#setTopCM-double-}
```
public void setTopCM(double value)
```


Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di centimetri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setTopInch(double value) {#setTopInch-double-}
```
public void setTopInch(double value)
```


Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pollici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Rappresenta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Imposta lo spostamento orizzontale della forma dalla colonna dell'angolo superiore sinistro. L'intervallo del valore è da 0 a 1024.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Imposta lo spostamento verticale della forma dalla riga dell'angolo superiore sinistro. L'intervallo del valore è da 0 a 256.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setUpperLeftColumn(int value) {#setUpperLeftColumn-int-}
```
public void setUpperLeftColumn(int value)
```


Rappresenta l'indice della colonna dell'angolo superiore sinistro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setUpperLeftRow(int value) {#setUpperLeftRow-int-}
```
public void setUpperLeftRow(int value)
```


Rappresenta l'indice di riga dell'angolo in alto a sinistra.

**Remarks**

Se la forma è nella forma o nel gruppo, UpperLeftRow verrà ignorato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Rappresenta la larghezza della forma, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Rappresenta la larghezza della forma, in unità di centimetri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Rappresenta la larghezza della forma, in unità di pollice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWidthPt(double value) {#setWidthPt-double-}
```
public void setWidthPt(double value)
```


Rappresenta la larghezza della forma, in unità di punto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWidthScale(int value) {#setWidthScale-int-}
```
public void setWidthScale(int value)
```


Imposta la scala della larghezza, in unità di percentuale della larghezza originale dell'immagine. Se la forma non è un'immagine, la proprietà WidthScale restituisce solo 100;

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Imposta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Imposta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Restituisce la posizione di una forma nell'ordine Z.

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

