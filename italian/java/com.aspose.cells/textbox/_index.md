---
title: "TextBox"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta una casella di testo in un foglio di calcolo."
type: docs
url: /it/java/com.aspose.cells/textbox/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Shape](../../com.aspose.cells/shape)
```
public class TextBox extends Shape
```

Incapsula l'oggetto che rappresenta una casella di testo in un foglio di calcolo.

**Example**

```
         //Instantiate a new Workbook.
         Workbook workbook = new Workbook();
         //Get the first worksheet in the book.
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Add a new textbox to the collection.
         int textboxIndex = worksheet.getTextBoxes().add(2, 1, 160, 200);
         //Get the textbox object.
         TextBox textbox0 = worksheet.getTextBoxes().get(textboxIndex);
         //Fill the text.
         textbox0.setText("ASPOSE______The .NET and JAVA Component Publisher!");
         //Set the textbox to adjust it according to its contents.
         textbox0.getTextBody().getTextAlignment().setAutoSize(true);
         //Set the placement.
         textbox0.setPlacement(PlacementType.FREE_FLOATING);
         //Set the font color.
         textbox0.getFont().setColor(Color.getBlue());
         //Set the font to bold.
         textbox0.getFont().setBold(true);
         //Set the font size.
         textbox0.getFont().setSize(14);
         //Set font attribute to italic.
         textbox0.getFont().setItalic(true);
         //Add a hyperlink to the textbox.
         textbox0.addHyperlink("http://www.aspose.com/");
         //Get the filformat of the textbox.
         FillFormat fillformat = textbox0.getFill();
         //Set the fillcolor.
         fillformat.getSolidFill().setColor(Color.getSilver());
         //Get the lineformat type of the textbox.
         LineFormat lineformat = textbox0.getLine();
         //Set the line style.
         lineformat.setCompoundType(MsoLineStyle.THIN_THICK);
         //Set the line weight.
         lineformat.setWeight(6);
         //Set the dash style to squaredot.
         lineformat.setDashStyle(MsoLineDashStyle.SQUARE_DOT);
         //Add another textbox.
         textboxIndex = worksheet.getTextBoxes().add(15, 4, 85, 120);
         //Get the second textbox.
         TextBox textbox1 = worksheet.getTextBoxes().get(textboxIndex);
         //Input some text to it.
         textbox1.setText("This is another simple text box");
         //Set the placement type as the textbox will move and
         //resize with cells.
         textbox1.setPlacement(PlacementType.MOVE_AND_SIZE);
         //Save the excel file.
         workbook.save("tsttextboxes.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Aggiunge un collegamento ipertestuale alla forma. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Sposta l'immagine nell'angolo in alto a destra. |
| [calculateTextSize()](#calculateTextSize--) | Ricalcola l'area di testo |
| [characters(int startIndex, int length)](#characters-int-int-) | Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fitToTextSize()](#fitToTextSize--) | Ricalcola un'area di testo adatta a visualizzare tutto il contenuto testuale. |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Formatta alcuni caratteri con l'impostazione del carattere. |
| [getActiveXControl()](#getActiveXControl--) | Ottiene il controllo ActiveX. |
| [getActualBox()](#getActualBox--) | Ottieni la posizione e le dimensioni effettive della forma (dopo aver applicato rotazione, capovolgimento, ecc.) |
| [getActualLowerRightRow()](#getActualLowerRightRow--) | Ottieni la riga inferiore effettiva. |
| [getAlternativeText()](#getAlternativeText--) | Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto [Shape](../../com.aspose.cells/shape). |
| [getAnchorType()](#getAnchorType--) | Ottiene il tipo del segnaposto di ancoraggio della forma. |
| [getAutoShapeType()](#getAutoShapeType--) | Ottiene il tipo di forma automatica. |
| [getBottom()](#getBottom--) | Rappresenta la larghezza dello spostamento verticale della forma dalla sua riga d'angolo inferiore, in unità di pixel. |
| [getCharacters()](#getCharacters--) | Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo. |
| [getClass()](#getClass--) |  |
| [getConnectionPoints()](#getConnectionPoints--) | Ottieni i punti di connessione |
| [getControlData()](#getControlData--) | Ottiene i dati del controllo. |
| [getCreateId()](#getCreateId--) | Ottiene l'ID di creazione per questa forma. |
| [getEquationParagraph()](#getEquationParagraph--) | Ottiene il primo paragrafo matematico dalla proprietà TextBody dell'oggetto TextBox. |
| [getEquationParagraph(int index)](#getEquationParagraph-int-) | Ottieni il paragrafo matematico specificato dalla proprietà TextBody dell'oggetto TextBox. |
| [getFill()](#getFill--) | Restituisce un oggetto [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) che contiene le proprietà di formattazione di riempimento per la forma specificata. |
| [getFillFormat()](#getFillFormat--) | Restituisce un oggetto MsoFillFormat che contiene le proprietà di formattazione di riempimento per la forma specificata. |
| [getFont()](#getFont--) | Rappresenta il carattere della forma. |
| [getFormatPicture()](#getFormatPicture--) | Ottiene le opzioni del formato immagine. |
| [getGeometry()](#getGeometry--) | Ottiene la geometria |
| [getGlow()](#getGlow--) | Rappresenta un oggetto [GlowEffect](../../com.aspose.cells/gloweffect) che specifica l'effetto bagliore per l'elemento del grafico o la forma. |
| [getGroup()](#getGroup--) | Ottiene la forma di gruppo che contiene questa forma. |
| [getHeight()](#getHeight--) | Rappresenta l'altezza della forma, in unità di pixel. |
| [getHeightCM()](#getHeightCM--) | Rappresenta l'altezza della forma, in unità di centimetri. |
| [getHeightInShape()](#getHeightInShape--) | Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore, in unità di 1/4000 dell'altezza della forma genitore. |
| [getHeightInch()](#getHeightInch--) | Rappresenta l'altezza della forma, in unità di pollici. |
| [getHeightPt()](#getHeightPt--) | Rappresenta l'altezza della forma, in unità di punti. |
| [getHeightScale()](#getHeightScale--) | Ottiene la scala di altezza, in unità di percentuale dell'altezza originale dell'immagine. |
| [getHtmlText()](#getHtmlText--) | Ottiene la stringa HTML che contiene dati e alcuni formati in questa casella di testo. |
| [getHyperlink()](#getHyperlink--) | Ottiene il collegamento ipertestuale della forma. |
| [getId()](#getId--) | Ottiene l'identificatore di questa forma. |
| [getInputRange()](#getInputRange--) | Ottiene l'intervallo del foglio di lavoro utilizzato per riempire la casella combinata specificata. |
| [getInputRange(boolean isR1C1, boolean isLocal)](#getInputRange-boolean-boolean-) | Ottiene l'intervallo utilizzato per riempire il controllo. |
| [getLeft()](#getLeft--) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel. |
| [getLeftCM()](#getLeftCM--) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di centimetri. |
| [getLeftInShape()](#getLeftInShape--) | Rappresenta lo spostamento orizzontale della forma dal bordo sinistro della forma padre, in unità di 1/4000 della larghezza della forma padre. |
| [getLeftInch()](#getLeftInch--) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pollici. |
| [getLeftToCorner()](#getLeftToCorner--) | Ottiene lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro. |
| [getLine()](#getLine--) | Ottiene lo stile della linea |
| [getLineFormat()](#getLineFormat--) | Restituisce un oggetto MsoLineFormat che contiene le proprietà di formattazione della linea per la forma specificata. |
| [getLinkedCell()](#getLinkedCell--) | Ottiene l'intervallo del foglio di lavoro collegato al valore del controllo. |
| [getLinkedCell(boolean isR1C1, boolean isLocal)](#getLinkedCell-boolean-boolean-) | Ottiene l'intervallo collegato al valore del controllo. |
| [getLockedProperty(int type)](#getLockedProperty-int-) | Ottiene il valore della proprietà locked. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Ottiene lo spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Ottiene lo spostamento verticale della forma dalla riga dell'angolo inferiore destro. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Rappresenta l'indice della colonna dell'angolo inferiore destro. |
| [getLowerRightRow()](#getLowerRightRow--) | Rappresenta l'indice della riga dell'angolo inferiore destro. |
| [getMacroName()](#getMacroName--) | Ottiene il nome della macro. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Ottiene il tipo di disegno. |
| [getName()](#getName--) | Ottiene il nome della forma. |
| [getPaths()](#getPaths--) | Ottiene i percorsi di una forma geometrica personalizzata. |
| [getPlacement()](#getPlacement--) | Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti. |
| [getReflection()](#getReflection--) | Rappresenta un oggetto [ReflectionEffect](../../com.aspose.cells/reflectioneffect) che specifica l'effetto di riflessione per l'elemento del grafico o la forma. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Indica se la forma è relativa alle dimensioni originali dell'immagine. |
| [getResultOfSmartArt()](#getResultOfSmartArt--) | Conversione di smart art in forme raggruppate. |
| [getRichFormattings()](#getRichFormattings--) | Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo. |
| [getRight()](#getRight--) | Rappresenta la larghezza dello spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro, in unità di pixel. |
| [getRotationAngle()](#getRotationAngle--) | Ottiene la rotazione della forma. |
| [getShadowEffect()](#getShadowEffect--) | Rappresenta un oggetto [ShadowEffect](../../com.aspose.cells/shadoweffect) che specifica l'effetto di ombra per l'elemento del grafico o la forma. |
| [getSoftEdges()](#getSoftEdges--) | Restituisce il raggio della sfocatura da applicare ai bordi, in unità di punti. |
| [getSpid()](#getSpid--) | Specifica un identificatore stringa opzionale che un'applicazione può utilizzare per identificare la forma specifica. |
| [getSpt()](#getSpt--) | Specifica un numero opzionale che un'applicazione può utilizzare per associare la forma specifica a un tipo di forma definito. |
| [getText()](#getText--) | Restituisce il testo di questa forma. |
| [getTextBody()](#getTextBody--) | Restituisce l'impostazione del testo della forma. |
| [getTextBoxOptions()](#getTextBoxOptions--) | Restituisce le informazioni testuali nella forma |
| [getTextDirection()](#getTextDirection--) | Restituisce la direzione del flusso di testo per questo oggetto. |
| [getTextEffect()](#getTextEffect--) | Restituisce un oggetto TextEffectFormat che contiene le proprietà di formattazione degli effetti di testo per la forma specificata. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Restituisce il tipo di allineamento orizzontale del testo della forma. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Restituisce il tipo di overflow orizzontale del testo della forma che contiene testo. |
| [getTextOptions()](#getTextOptions--) | Rappresenta le opzioni di testo della forma. |
| [getTextOrientationType()](#getTextOrientationType--) | Restituisce il tipo di orientamento del testo della forma. |
| [getTextShapeType()](#getTextShapeType--) | Restituisce il tipo di forma di testo predefinito. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Restituisce il tipo di allineamento verticale del testo della forma. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Restituisce il tipo di overflow verticale del testo della forma che contiene testo. |
| [getThreeDFormat()](#getThreeDFormat--) | Restituisce il formato 3D della forma. |
| [getTitle()](#getTitle--) | Specifica il titolo (didascalia) dell'oggetto forma corrente. |
| [getTop()](#getTop--) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pixel. |
| [getTopCM()](#getTopCM--) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di centimetri. |
| [getTopInShape()](#getTopInShape--) | Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore, in unità di 1/4000 dell'altezza della forma genitore. |
| [getTopInch()](#getTopInch--) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pollici. |
| [getTopToCorner()](#getTopToCorner--) | Restituisce lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel. |
| [getType()](#getType--) | Ottiene il tipo di forma automatica. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Restituisce lo spostamento orizzontale della forma dalla colonna dell'angolo superiore sinistro. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Restituisce lo spostamento verticale della forma dalla riga dell'angolo superiore sinistro. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Rappresenta l'indice della colonna dell'angolo superiore sinistro. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Rappresenta l'indice della riga superiore. |
| [getWidth()](#getWidth--) | Rappresenta la larghezza della forma, in unità di pixel. |
| [getWidthCM()](#getWidthCM--) | Rappresenta la larghezza della forma, in unità di centimetri. |
| [getWidthInShape()](#getWidthInShape--) | Rappresenta la larghezza della forma, in unità di 1/4000 della forma padre. |
| [getWidthInch()](#getWidthInch--) | Rappresenta la larghezza della forma, in unità di pollice. |
| [getWidthPt()](#getWidthPt--) | Rappresenta la larghezza della forma, in unità di punto. |
| [getWidthScale()](#getWidthScale--) | Ottiene la scala di larghezza, in unità di percentuale della larghezza originale dell'immagine. |
| [getWorksheet()](#getWorksheet--) | Ottiene l'oggetto [Worksheet](../../com.aspose.cells/worksheet) che contiene questa forma. |
| [getX()](#getX--) | Ottiene lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel. |
| [getY()](#getY--) | Ottiene lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel. |
| [getZOrderPosition()](#getZOrderPosition--) | Restituisce la posizione di una forma nell'ordine Z. |
| [hasLine()](#hasLine--) | Ottiene se il bordo della linea della forma è visibile. |
| [hashCode()](#hashCode--) |  |
| [isAspectRatioLocked()](#isAspectRatioLocked--) | True indica che il rapporto d'aspetto della forma è bloccato. |
| [isDecorative()](#isDecorative--) | Indica se l'oggetto è decorativo. |
| [isEquation()](#isEquation--) | Indica se la forma contiene solo un'equazione. |
| [isFilled()](#isFilled--) | Indica se il formato di riempimento è visibile. |
| [isFlippedHorizontally()](#isFlippedHorizontally--) | Ottiene se la forma è capovolta orizzontalmente . |
| [isFlippedVertically()](#isFlippedVertically--) | Ottiene se la forma è capovolta verticalmente . |
| [isGroup()](#isGroup--) | Indica se questa forma è una forma di gruppo. |
| [isHidden()](#isHidden--) | Indica se l'oggetto è visibile. |
| [isInGroup()](#isInGroup--) | Indica se la forma è raggruppata. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True indica che il rapporto d'aspetto della forma è bloccato. |
| [isLocked()](#isLocked--) | True indica che l'oggetto non può essere modificato quando il foglio è protetto. |
| [isPrintable()](#isPrintable--) | Indica se l'oggetto è stampabile. |
| [isRichText()](#isRichText--) | Se il testo è o meno testo formattato. |
| [isSameSetting(Object obj)](#isSameSetting-java.lang.Object-) | Restituisce se la forma è identica. |
| [isSmartArt()](#isSmartArt--) | Indica se la forma è un smart art. |
| [isTextWrapped()](#isTextWrapped--) | Ottiene il tipo di avvolgimento del testo della forma che contiene testo. |
| [isWordArt()](#isWordArt--) | Indica se questa forma è un word art. |
| [moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)](#moveToRange-int-int-int-int-) | Sposta la forma in un intervallo specificato. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeActiveXControl()](#removeActiveXControl--) | Rimuove il controllo ActiveX. |
| [removeHyperlink()](#removeHyperlink--) | Rimuove il collegamento ipertestuale della forma. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto [Shape](../../com.aspose.cells/shape). |
| [setAnchorType(int value)](#setAnchorType-int-) | Imposta il tipo del segnaposto di ancoraggio della forma. |
| [setAspectRatioLocked(boolean value)](#setAspectRatioLocked-boolean-) | True indica che il rapporto d'aspetto della forma è bloccato. |
| [setAutoShapeType(int value)](#setAutoShapeType-int-) | Imposta il tipo di forma automatica. |
| [setBottom(int value)](#setBottom-int-) | Rappresenta la larghezza dello spostamento verticale della forma dalla sua riga d'angolo inferiore, in unità di pixel. |
| [setCreateId(UUID value)](#setCreateId-java.util.UUID-) | Imposta l'ID di creazione per questa forma. |
| [setDecorative(boolean value)](#setDecorative-boolean-) | Indica se l'oggetto è decorativo. |
| [setFilled(boolean value)](#setFilled-boolean-) | Indica se il formato di riempimento è visibile. |
| [setFlippedHorizontally(boolean value)](#setFlippedHorizontally-boolean-) | Imposta se la forma è capovolta orizzontalmente. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Imposta se la forma è capovolta verticalmente. |
| [setFont(Font value)](#setFont-com.aspose.cells.Font-) | Rappresenta il carattere della forma. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Imposta che il bordo della forma sia visibile. |
| [setHeight(int value)](#setHeight-int-) | Rappresenta l'altezza della forma, in unità di pixel. |
| [setHeightCM(double value)](#setHeightCM-double-) | Rappresenta l'altezza della forma, in unità di centimetri. |
| [setHeightInShape(int value)](#setHeightInShape-int-) | Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore, in unità di 1/4000 dell'altezza della forma genitore. |
| [setHeightInch(double value)](#setHeightInch-double-) | Rappresenta l'altezza della forma, in unità di pollici. |
| [setHeightPt(double value)](#setHeightPt-double-) | Rappresenta l'altezza della forma, in unità di punti. |
| [setHeightScale(int value)](#setHeightScale-int-) | Imposta la scala di altezza, in unità di percentuale dell'altezza originale dell'immagine. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indica se l'oggetto è visibile. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Imposta la stringa HTML che contiene dati e alcuni formati in questa casella di testo. |
| [setInputRange(String value)](#setInputRange-java.lang.String-) | Imposta l'intervallo del foglio di lavoro usato per riempire la casella combinata specificata. |
| [setInputRange(String formula, boolean isR1C1, boolean isLocal)](#setInputRange-java.lang.String-boolean-boolean-) | Imposta l'intervallo usato per riempire il controllo. |
| [setLeft(int value)](#setLeft-int-) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel. |
| [setLeftCM(double value)](#setLeftCM-double-) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di centimetri. |
| [setLeftInShape(int value)](#setLeftInShape-int-) | Rappresenta lo spostamento orizzontale della forma dal bordo sinistro della forma padre, in unità di 1/4000 della larghezza della forma padre. |
| [setLeftInch(double value)](#setLeftInch-double-) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pollici. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Imposta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Imposta l'intervallo del foglio di lavoro collegato al valore del controllo. |
| [setLinkedCell(String formula, boolean isR1C1, boolean isLocal)](#setLinkedCell-java.lang.String-boolean-boolean-) | Imposta l'intervallo collegato al valore del controllo. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True indica che il rapporto d'aspetto della forma è bloccato. |
| [setLocked(boolean value)](#setLocked-boolean-) | True indica che l'oggetto non può essere modificato quando il foglio è protetto. |
| [setLockedProperty(int type, boolean value)](#setLockedProperty-int-boolean-) | Imposta la proprietà bloccata. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Imposta lo spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Imposta lo spostamento verticale della forma dalla riga dell'angolo inferiore destro. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Rappresenta l'indice della colonna dell'angolo inferiore destro. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Rappresenta l'indice della riga dell'angolo inferiore destro. |
| [setMacroName(String value)](#setMacroName-java.lang.String-) | Imposta il nome della macro. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome della forma. |
| [setPlacement(int value)](#setPlacement-int-) | Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Indica se l'oggetto è stampabile. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Indica se la forma è relativa alle dimensioni originali dell'immagine. |
| [setRight(int value)](#setRight-int-) | Rappresenta la larghezza dello spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro, in unità di pixel. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Imposta la rotazione della forma. |
| [setSoftEdges(double value)](#setSoftEdges-double-) | Imposta il raggio della sfocatura da applicare ai bordi, in unità di punti. |
| [setText(String value)](#setText-java.lang.String-) | Imposta il testo di questa forma. |
| [setTextDirection(int value)](#setTextDirection-int-) | Imposta la direzione del flusso di testo per questo oggetto. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Imposta il tipo di allineamento orizzontale del testo della forma. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Imposta il tipo di overflow orizzontale del testo della forma che contiene testo. |
| [setTextOptions(TextOptions value)](#setTextOptions-com.aspose.cells.TextOptions-) | Rappresenta le opzioni di testo della forma. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Imposta il tipo di orientamento del testo della forma. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Imposta il tipo di forma di testo predefinito. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Imposta il tipo di allineamento verticale del testo della forma. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Imposta il tipo di overflow verticale del testo della forma che contiene testo. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Imposta il tipo di avvolgimento del testo della forma che contiene testo. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Specifica il titolo (didascalia) dell'oggetto forma corrente. |
| [setTop(int value)](#setTop-int-) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pixel. |
| [setTopCM(double value)](#setTopCM-double-) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di centimetri. |
| [setTopInShape(int value)](#setTopInShape-int-) | Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore, in unità di 1/4000 dell'altezza della forma genitore. |
| [setTopInch(double value)](#setTopInch-double-) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pollici. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Imposta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Imposta lo spostamento orizzontale della forma dalla colonna dell'angolo in alto a sinistra. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Imposta lo spostamento verticale della forma dalla riga dell'angolo in alto a sinistra. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Rappresenta l'indice della colonna dell'angolo superiore sinistro. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Rappresenta l'indice della riga superiore. |
| [setWidth(int value)](#setWidth-int-) | Rappresenta la larghezza della forma, in unità di pixel. |
| [setWidthCM(double value)](#setWidthCM-double-) | Rappresenta la larghezza della forma, in unità di centimetri. |
| [setWidthInShape(int value)](#setWidthInShape-int-) | Rappresenta la larghezza della forma, in unità di 1/4000 della forma padre. |
| [setWidthInch(double value)](#setWidthInch-double-) | Rappresenta la larghezza della forma, in unità di pollice. |
| [setWidthPt(double value)](#setWidthPt-double-) | Rappresenta la larghezza della forma, in unità di punto. |
| [setWidthScale(int value)](#setWidthScale-int-) | Imposta la scala di larghezza, in unità di percentuale della larghezza originale dell'immagine. |
| [setX(int value)](#setX-int-) | Imposta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel. |
| [setY(int value)](#setY-int-) | Imposta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Restituisce la posizione di una forma nell'ordine Z. |
| [toFrontOrBack(int orders)](#toFrontOrBack-int-) | Porta la forma in primo piano o invia la forma sullo sfondo. |
| [toImage(OutputStream stream, ImageFormat imageFormat)](#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-) | Crea l'immagine della forma e la salva in un flusso nel formato specificato. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Salva la forma in un flusso. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Salva la forma in un file. |
| [toString()](#toString--) |  |
| [updateSelectedValue()](#updateSelectedValue--) | Aggiorna il valore selezionato con il valore della cella collegata. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public Hyperlink addHyperlink(String address)
```


Aggiunge un collegamento ipertestuale alla forma.

**Example**

```
         Hyperlink hyperlink = shape.addHyperlink("https://www.aspose.com/");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indirizzo | java.lang.String | Indirizzo del collegamento ipertestuale. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - Returns the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Sposta l'immagine nell'angolo in alto a destra.

**Example**

```
         shape.alignTopRightCorner(2, 5);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | l'indice della riga. |
| rightColumn | int | l'indice della colonna. |

### calculateTextSize() {#calculateTextSize--}
```
public int[] calculateTextSize()
```


Ricalcola l'area di testo

**Example**

```
         //The size of the text area is:w=size[0],h=size[1]
         int[] size = shape.calculateTextSize();
```

**Returns:**
int[] - Dimensione del testo in un array (larghezza e altezza).
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo.

**Remarks**

Questo metodo funziona solo su forme con titolo.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | int | L'indice dell'inizio del carattere. |
| length | int | Il numero di caratteri. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### fitToTextSize() {#fitToTextSize--}
```
public void fitToTextSize()
```


Ricalcola un'area di testo adatta a visualizzare tutto il contenuto testuale.

**Example**

```
         if (shape.getName().startsWith("Your traget"))
         {
             shape.fitToTextSize();
         }
```

### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


Formatta alcuni caratteri con l'impostazione del carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | int | L'indice di inizio. |
| length | int | La lunghezza. |
| font | [Font](../../com.aspose.cells/font) | L'impostazione del carattere. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Il flag dell'impostazione del carattere. |

### getActiveXControl() {#getActiveXControl--}
```
public ActiveXControl getActiveXControl()
```


Ottiene il controllo ActiveX.

**Example**

```
         if(shape.getActiveXControl() != null)
         {
             CheckBoxActiveXControl checkBox1 = (CheckBoxActiveXControl)shape.getActiveXControl();
             //The font name of CheckBox
             String fontName = checkBox1.getFont().getName();
         }
```

**Returns:**
[ActiveXControl](../../com.aspose.cells/activexcontrol)
### getActualBox() {#getActualBox--}
```
public float[] getActualBox()
```


Ottieni la posizione e le dimensioni effettive della forma (dopo aver applicato rotazione, capovolgimento, ecc.)

**Remarks**

Nota: L'interfaccia non è completamente funzionale, soprattutto le informazioni sulla posizione non sono corrette. Si consiglia di non utilizzare questa interfaccia finché la funzione non è completa.

**Example**

```
         float[] box = shape.getActualBox();
         System.out.println("x = " + box[0]);
         System.out.println("y = " + box[1]);
         System.out.println("w = " + box[2]);
         System.out.println("h = " + box[3]);
```

**Returns:**
float[] - Restituisce la posizione e le dimensioni nell'ordine x, y, w, h
### getActualLowerRightRow() {#getActualLowerRightRow--}
```
public int getActualLowerRightRow()
```


Ottieni la riga inferiore effettiva.

**Example**

```
         int rRow = shape.getActualLowerRightRow();
```

**Returns:**
int
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto [Shape](../../com.aspose.cells/shape).

**Example**

```
         shape.setAlternativeText("a rectangle");
```

**Returns:**
java.lang.String
### getAnchorType() {#getAnchorType--}
```
public int getAnchorType()
```


Ottiene il tipo del segnaposto di ancoraggio della forma.

Vedi [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Example**

```
         if (shape.getAnchorType() == ShapeAnchorType.ONE_CELL_ANCHOR)
             shape.setAnchorType(ShapeAnchorType.TWO_CELL_ANCHOR);
```

**Returns:**
int
### getAutoShapeType() {#getAutoShapeType--}
```
public int getAutoShapeType()
```


Ottiene il tipo di forma automatica.

Vedi [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         if (shape.getAutoShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setAutoShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getBottom() {#getBottom--}
```
public int getBottom()
```


Rappresenta la larghezza dello spostamento verticale della forma dalla sua riga d'angolo inferiore, in unità di pixel.

**Example**

```
         if (shape.getBottom() == 3)
             shape.setBottom(1);
```

**Returns:**
int
### getCharacters() {#getCharacters--}
```
public ArrayList getCharacters()
```


Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Shape.GetRichFormattings(). Questo metodo sarà rimosso tra 12 mesi a partire da novembre 2023. Aspose si scusa per qualsiasi inconveniente possa aver subito.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Returns:**
java.util.ArrayList - Tutti gli oggetti Characters
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConnectionPoints() {#getConnectionPoints--}
```
public float[][] getConnectionPoints()
```


Ottieni i punti di connessione

**Example**

```
         float[][] points = shape.getConnectionPoints();
```

**Returns:**
float[][] - Coppie [X,Y] del punto di connessione. Ogni elemento è un array float[2], [0] rappresenta x e [1] rappresenta y.
### getControlData() {#getControlData--}
```
public byte[] getControlData()
```


Ottiene i dati del controllo.

**Example**

```
         if(shape.getControlData() == null)
             System.out.println("No data.");
```

**Returns:**
byte[]
### getCreateId() {#getCreateId--}
```
public UUID getCreateId()
```


Ottiene l'ID di creazione per questa forma.

**Example**

```
         System.out.println(shape.getCreateId());
         java.util.UUID g = java.util.UUID.randomUUID();
         shape.setCreateId(g);
         System.out.println(shape.getCreateId());
```

**Returns:**
java.util.UUID
### getEquationParagraph() {#getEquationParagraph--}
```
public EquationNode getEquationParagraph()
```


Ottiene il primo paragrafo matematico dalla proprietà TextBody dell'oggetto TextBox.

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If there has math paragraph, returns the first one, otherwise returns null.
### getEquationParagraph(int index) {#getEquationParagraph-int-}
```
public EquationNode getEquationParagraph(int index)
```


Ottieni il paragrafo matematico specificato dalla proprietà TextBody dell'oggetto TextBox. Nota: (1) Restituisce NULL quando l'indice è fuori dai limiti o non trovato. (2) Restituisce anche NULL se la posizione dell'indice specificato non è un paragrafo matematico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice di posizione del paragrafo matematico, a partire da 0. |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - Returns the math paragraph specified by index.
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Restituisce un oggetto [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) che contiene le proprietà di formattazione di riempimento per la forma specificata.

**Example**

```
         FillFormat fillFmt = shape.getFill();
```

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getFillFormat() {#getFillFormat--}
```
public MsoFillFormat getFillFormat()
```


Restituisce un oggetto MsoFillFormat che contiene le proprietà di formattazione di riempimento per la forma specificata.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Fill. Questa proprietà sarà rimossa tra 12 mesi a partire da luglio 2016. Aspose si scusa per qualsiasi inconveniente possa aver subito.

**Returns:**
[MsoFillFormat](../../com.aspose.cells/msofillformat)
### getFont() {#getFont--}
```
public Font getFont()
```


Rappresenta il carattere della forma.

**Example**

```
         Font font = shape.getFont();
         font.setName("Arial");
         font.setSize(12);
         font.setColor(Color.getRed());
```

**Returns:**
[Font](../../com.aspose.cells/font)
### getFormatPicture() {#getFormatPicture--}
```
public MsoFormatPicture getFormatPicture()
```


Ottiene le opzioni del formato immagine.

**Example**

```
         MsoFormatPicture msoFormatPicture = shape.getFormatPicture();
```

**Returns:**
[MsoFormatPicture](../../com.aspose.cells/msoformatpicture)
### getGeometry() {#getGeometry--}
```
public Geometry getGeometry()
```


Ottiene la geometria

**Example**

```
         if (shape.getGeometry() != null &&shape.getGeometry().getShapeAdjustValues().getCount() == 0)
             System.out.println("No geometry path.");
```

**Returns:**
[Geometry](../../com.aspose.cells/geometry)
### getGlow() {#getGlow--}
```
public GlowEffect getGlow()
```


Rappresenta un oggetto [GlowEffect](../../com.aspose.cells/gloweffect) che specifica l'effetto bagliore per l'elemento del grafico o la forma.

**Example**

```
         GlowEffect glowEffect = shape.getGlow();
```

**Returns:**
[GlowEffect](../../com.aspose.cells/gloweffect)
### getGroup() {#getGroup--}
```
public GroupShape getGroup()
```


Ottiene la forma di gruppo che contiene questa forma.

**Example**

```
         GroupShape groupShape = shape.getGroup();
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Rappresenta l'altezza della forma, in unità di pixel.

**Example**

```
         if (shape.getHeight() == 3)
             shape.setHeight(1);
```

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Rappresenta l'altezza della forma, in unità di centimetri.

**Example**

```
         if (shape.getHeightCM() == 3)
             shape.setHeightCM(1);
```

**Returns:**
double
### getHeightInShape() {#getHeightInShape--}
```
public int getHeightInShape()
```


Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore, in unità di 1/4000 dell'altezza della forma genitore.

**Remarks**

Si applica solo quando questa forma è nel gruppo o nel grafico.

**Example**

```
         if (shape.isInGroup() &&shape.getHeightInShape() == 4000)
             shape.setHeightInShape(2000);
```

**Returns:**
int
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Rappresenta l'altezza della forma, in unità di pollici.

**Example**

```
         if (shape.getHeightInch() == 3)
             shape.setHeightInch(1);
```

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


Rappresenta l'altezza della forma, in unità di punti.

**Example**

```
         if (shape.getHeightPt() == 3)
             shape.setHeightPt(1);
```

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


Restituisce la scala dell'altezza, in unità di percentuale dell'altezza originale dell'immagine. Se la forma non è un'immagine, la proprietà HeightScale restituisce solo 100;

**Example**

```
         if (shape.getHeightScale() == 3)
             shape.setHeightScale(1);
```

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


Ottiene la stringa HTML che contiene dati e alcuni formati in questa casella di testo.

**Example**

```
         String html = shape.getHtmlText();
         if(html == null || "".equals(html))
         {
             shape.setHtmlText("<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>");
         }
```

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public Hyperlink getHyperlink()
```


Ottiene il collegamento ipertestuale della forma.

**Example**

```
         Hyperlink hyperlink = shape.getHyperlink();
```

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink)
### getId() {#getId--}
```
public int getId()
```


Ottiene l'identificatore di questa forma.

**Example**

```
         int id = shape.getId();
```

**Returns:**
int
### getInputRange() {#getInputRange--}
```
public String getInputRange()
```


Ottiene l'intervallo del foglio di lavoro utilizzato per riempire la casella combinata specificata.

**Example**

```
         if (shape.getInputRange().equals("$B$6:$B10"))
             shape.setInputRange("$A$1:$A$5");
```

**Returns:**
java.lang.String
### getInputRange(boolean isR1C1, boolean isLocal) {#getInputRange-boolean-boolean-}
```
public String getInputRange(boolean isR1C1, boolean isLocal)
```


Ottiene l'intervallo utilizzato per riempire il controllo.

**Example**

```
         String range = shape.getInputRange(false, true);
         //If successful, a value like "$A$1:$A$3" will be returned
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |

**Returns:**
java.lang.String - L'intervallo utilizzato per riempire il controllo.
### getLeft() {#getLeft--}
```
public int getLeft()
```


Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel.

**Example**

```
         if (shape.getLeft() == 3)
             shape.setLeft(1);
```

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di centimetri.

**Example**

```
         if (shape.getLeftCM() == 3)
             shape.setLeftCM(1);
```

**Returns:**
double
### getLeftInShape() {#getLeftInShape--}
```
public int getLeftInShape()
```


Rappresenta lo spostamento orizzontale della forma dal bordo sinistro della forma padre, in unità di 1/4000 della larghezza della forma padre.

**Remarks**

Si applica solo quando questa forma è nel gruppo o nel grafico.

**Example**

```
         if (shape.isInGroup() &&shape.getLeftInShape() == 2000)
             shape.setLeftInShape(4000);
```

**Returns:**
int
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pollici.

**Example**

```
         if (shape.getLeftInch() == 3)
             shape.setLeftInch(1);
```

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Ottiene lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro.

**Example**

```
         if (shape.getLeftToCorner() == 3)
             shape.setLeftToCorner(1);
```

**Returns:**
int
### getLine() {#getLine--}
```
public LineFormat getLine()
```


Ottiene lo stile della linea

**Example**

```
         LineFormat lineFmt = shape.getLine();
```

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getLineFormat() {#getLineFormat--}
```
public MsoLineFormat getLineFormat()
```


Restituisce un oggetto MsoLineFormat che contiene le proprietà di formattazione della linea per la forma specificata.

**Remarks**

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Line. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2016. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[MsoLineFormat](../../com.aspose.cells/msolineformat)
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Ottiene l'intervallo del foglio di lavoro collegato al valore del controllo.

**Example**

```
         if (shape.getLinkedCell().equals("$B$6"))
         {
             shape.setLinkedCell("A1");
         }
         shape.updateSelectedValue();
```

**Returns:**
java.lang.String
### getLinkedCell(boolean isR1C1, boolean isLocal) {#getLinkedCell-boolean-boolean-}
```
public String getLinkedCell(boolean isR1C1, boolean isLocal)
```


Ottiene l'intervallo collegato al valore del controllo.

**Example**

```
         //You may get results like '$A$1'
         String link = shape.getLinkedCell(false, false);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |

**Returns:**
java.lang.String - L'intervallo collegato al valore del controllo.
### getLockedProperty(int type) {#getLockedProperty-int-}
```
public boolean getLockedProperty(int type)
```


Ottiene il valore della proprietà locked.

**Example**

```
         int noAdjustHandles = 0;
         if (shape.getLockedProperty(ShapeLockType.ADJUST_HANDLES))
             noAdjustHandles = 1;
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). Il tipo della proprietà shape locked. |

**Returns:**
boolean - Restituisce il valore della proprietà locked.
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Ottiene lo spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro.

**Remarks**

L'intervallo di valore è da 0 a 1024.

**Example**

```
         if (shape.getLowerDeltaX() == 3)
             shape.setLowerDeltaX(1);
```

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


Ottiene lo spostamento verticale della forma dalla riga dell'angolo inferiore destro.

**Remarks**

L'intervallo di valore è da 0 a 256.

**Example**

```
         if (shape.getLowerDeltaY() == 3)
             shape.setLowerDeltaY(1);
```

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


Rappresenta l'indice della colonna dell'angolo inferiore destro.

**Example**

```
         if (shape.getLowerRightColumn() == 3)
             shape.setLowerRightColumn(1);
```

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


Rappresenta l'indice della riga dell'angolo inferiore destro.

**Example**

```
         if (shape.getLowerRightRow() == 3)
             shape.setLowerRightRow(1);
```

**Returns:**
int
### getMacroName() {#getMacroName--}
```
public String getMacroName()
```


Ottiene il nome della macro.

**Example**

```
         //Sets the name of macro.
         shape.setMacroName("DoWork()");
```

**Returns:**
java.lang.String
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


Ottiene il tipo di disegno.

Vedi [MsoDrawingType](../../com.aspose.cells/msodrawingtype).

**Example**

```
         /*Aspose.Cells.Drawing.MsoDrawingType*/int msoDrawingType = shape.getMsoDrawingType();
```

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome della forma.

**Example**

```
         shape.setName("shape1");
```

**Returns:**
java.lang.String
### getPaths() {#getPaths--}
```
public ShapePathCollection getPaths()
```


Ottiene i percorsi di una forma geometrica personalizzata.

**Example**

```
         //Returns non-null if there is a path to the custom geometry
         if(shape.getPaths() == null)
             System.out.println("No custom geometry path.");
```

**Returns:**
[ShapePathCollection](../../com.aspose.cells/shapepathcollection)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti. La proprietà controlla il posizionamento di un oggetto su un foglio di lavoro.

Vedi [PlacementType](../../com.aspose.cells/placementtype).

**Example**

```
         if (shape.getPlacement() == PlacementType.MOVE)
             shape.setPlacement(PlacementType.MOVE_AND_SIZE);
```

**Returns:**
int
### getReflection() {#getReflection--}
```
public ReflectionEffect getReflection()
```


Rappresenta un oggetto [ReflectionEffect](../../com.aspose.cells/reflectioneffect) che specifica l'effetto di riflessione per l'elemento del grafico o la forma.

**Example**

```
         ReflectionEffect reflectionEffect = shape.getReflection();
```

**Returns:**
[ReflectionEffect](../../com.aspose.cells/reflectioneffect)
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


Indica se la forma è relativa alle dimensioni originali dell'immagine.

**Example**

```
         if(shape.getRelativeToOriginalPictureSize())
             shape.setRelativeToOriginalPictureSize(false);
```

**Returns:**
boolean
### getResultOfSmartArt() {#getResultOfSmartArt--}
```
public GroupShape getResultOfSmartArt()
```


Conversione di smart art in forme raggruppate.

**Example**

```
         if(shape.isSmartArt())
         {
             GroupShape groupShape = shape.getResultOfSmartArt();
         }
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getRichFormattings() {#getRichFormattings--}
```
public FontSetting[] getRichFormattings()
```


Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo.

**Example**

```
         FontSetting[] list = shape.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Tutti gli oggetti Characters
### getRight() {#getRight--}
```
public int getRight()
```


Rappresenta la larghezza dello spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro, in unità di pixel.

**Example**

```
         if (shape.getRight() == 3)
             shape.setRight(1);
```

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Ottiene la rotazione della forma.

**Example**

```
         //Gets rotation angle of the shape.
         double angle = shape.getRotationAngle() ;
 
         //Gets rotation angle of the shape.
          shape.setRotationAngle(60);
```

**Returns:**
double
### getShadowEffect() {#getShadowEffect--}
```
public ShadowEffect getShadowEffect()
```


Rappresenta un oggetto [ShadowEffect](../../com.aspose.cells/shadoweffect) che specifica l'effetto di ombra per l'elemento del grafico o la forma.

**Example**

```
         ShadowEffect shadowEffect = shape.getShadowEffect();
```

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSoftEdges() {#getSoftEdges--}
```
public double getSoftEdges()
```


Restituisce il raggio della sfocatura da applicare ai bordi, in unità di punti.

**Example**

```
         shape.setSoftEdges(0.5d);
```

**Returns:**
double
### getSpid() {#getSpid--}
```
public String getSpid()
```


Specifica un identificatore stringa opzionale che un'applicazione può utilizzare per identificare la forma specifica.

**Example**

```
         String spid = shape.getSpid();
```

**Returns:**
java.lang.String
### getSpt() {#getSpt--}
```
public int getSpt()
```


Specifica un numero opzionale che un'applicazione può utilizzare per associare la forma specifica a un tipo di forma definito.

**Example**

```
         int spt = shape.getSpt();
```

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Restituisce il testo di questa forma.

**Example**

```
         if(shape.getText() == null)
             shape.setText("This is a test.");
```

**Returns:**
java.lang.String
### getTextBody() {#getTextBody--}
```
public FontSettingCollection getTextBody()
```


Restituisce l'impostazione del testo della forma.

**Example**

```
         FontSettingCollection fontSettingCollection = shape.getTextBody();
         fontSettingCollection.setText("This is a test.");
```

**Returns:**
[FontSettingCollection](../../com.aspose.cells/fontsettingcollection)
### getTextBoxOptions() {#getTextBoxOptions--}
```
public TextBoxOptions getTextBoxOptions()
```


Restituisce le informazioni testuali nella forma

**Example**

```
         TextBoxOptions textBoxOpt = shape.getTextBoxOptions();
         textBoxOpt.setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType.LEFT);
         textBoxOpt.setTopMarginPt(0.2d);
         textBoxOpt.setLeftMarginPt(0.2d);
         textBoxOpt.setRightMarginPt(0.2d);
         textBoxOpt.setBottomMarginPt(0.2d);
```

**Returns:**
[TextBoxOptions](../../com.aspose.cells/textboxoptions)
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Restituisce la direzione del flusso di testo per questo oggetto.

Vedi [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Example**

```
         if (shape.getTextDirection() == com.aspose.cells.TextDirectionType.CONTEXT)
             shape.setTextDirection(com.aspose.cells.TextDirectionType.LEFT_TO_RIGHT);
```

**Returns:**
int
### getTextEffect() {#getTextEffect--}
```
public TextEffectFormat getTextEffect()
```


Restituisce un oggetto TextEffectFormat che contiene le proprietà di formattazione degli effetti di testo per la forma specificata. Si applica agli oggetti Shape che rappresentano WordArt.

**Example**

```
         if(shape.isWordArt())
         {
             TextEffectFormat textEffectFormat = shape.getTextEffect();
         }
```

**Returns:**
[TextEffectFormat](../../com.aspose.cells/texteffectformat)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


Restituisce il tipo di allineamento orizzontale del testo della forma.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Example**

```
         if (shape.getTextHorizontalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextHorizontalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```


Restituisce il tipo di overflow orizzontale del testo della forma che contiene testo.

Vedi [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         if (shape.getTextHorizontalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextHorizontalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Rappresenta le opzioni di testo della forma.

**Example**

```
         TextOptions opt = shape.getTextOptions();
         opt.setColor(Color.getBlue());
         opt.setSize(8);
```

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextOrientationType() {#getTextOrientationType--}
```
public int getTextOrientationType()
```


Restituisce il tipo di orientamento del testo della forma.

Vedi [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Example**

```
         if (shape.getTextOrientationType() == com.aspose.cells.TextOrientationType.NO_ROTATION)
             shape.setTextOrientationType(com.aspose.cells.TextOrientationType.TOP_TO_BOTTOM);
```

**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```


Restituisce il tipo di forma di testo predefinito.

Vedi [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         if (shape.getTextShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setTextShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


Restituisce il tipo di allineamento verticale del testo della forma.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Example**

```
         if (shape.getTextVerticalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextVerticalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextVerticalOverflow() {#getTextVerticalOverflow--}
```
public int getTextVerticalOverflow()
```


Restituisce il tipo di overflow verticale del testo della forma che contiene testo.

Vedi [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         if (shape.getTextVerticalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextVerticalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getThreeDFormat() {#getThreeDFormat--}
```
public ThreeDFormat getThreeDFormat()
```


Restituisce il formato 3D della forma.

**Example**

```
         ThreeDFormat threeDFormat = shape.getThreeDFormat();
```

**Returns:**
[ThreeDFormat](../../com.aspose.cells/threedformat)
### getTitle() {#getTitle--}
```
public String getTitle()
```


Specifica il titolo (didascalia) dell'oggetto forma corrente.

**Example**

```
         shape.setTitle("title1");
```

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pixel.

**Remarks**

Se la forma è nel grafico, rappresenta lo spostamento verticale della forma dal suo bordo superiore.

**Example**

```
         if (shape.getTop() == 3)
             shape.setTop(1);
```

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di centimetri.

**Example**

```
         if (shape.getTopCM() == 3)
             shape.setTopCM(1);
```

**Returns:**
double
### getTopInShape() {#getTopInShape--}
```
public int getTopInShape()
```


Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore, in unità di 1/4000 dell'altezza della forma genitore.

**Remarks**

Si applica solo quando questa forma è nel gruppo o nel grafico.

**Example**

```
         if (shape.isInGroup() &&shape.getTopInShape() == 8000)
             shape.setTopInShape(4000);
```

**Returns:**
int
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pollici.

**Example**

```
         if (shape.getTopInch() == 3)
             shape.setTopInch(1);
```

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Restituisce lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel.

**Example**

```
         if (shape.getTopToCorner() == 3)
             shape.setTopToCorner(1);
```

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Ottiene il tipo di forma automatica.

Vedi [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         /*Aspose.Cells.Drawing.AutoShapeType*/int autoShapeType = shape.getType();
```

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


Restituisce lo spostamento orizzontale della forma dalla colonna dell'angolo superiore sinistro.

**Remarks**

L'intervallo di valore è da 0 a 1024.

**Example**

```
         if (shape.getUpperDeltaX() == 3)
             shape.setUpperDeltaX(1);
```

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


Restituisce lo spostamento verticale della forma dalla riga dell'angolo superiore sinistro.

**Remarks**

L'intervallo di valore è da 0 a 256.

**Example**

```
         if (shape.getUpperDeltaY() == 3)
             shape.setUpperDeltaY(1);
```

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Rappresenta l'indice della colonna dell'angolo superiore sinistro.

**Example**

```
         if (shape.getUpperLeftColumn() == 3)
             shape.setUpperLeftColumn(1);
```

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Rappresenta l'indice della riga superiore.

**Remarks**

Se la forma è nella forma o nel gruppo, UpperLeftRow verrà ignorato.

**Example**

```
         if (shape.getUpperLeftRow() == 3)
             shape.setUpperLeftRow(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Rappresenta la larghezza della forma, in unità di pixel.

**Example**

```
         if (shape.getWidth() == 3)
             shape.setWidth(1);
```

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Rappresenta la larghezza della forma, in unità di centimetri.

**Example**

```
         if (shape.getWidthCM() == 3)
             shape.setWidthCM(1);
```

**Returns:**
double
### getWidthInShape() {#getWidthInShape--}
```
public int getWidthInShape()
```


Rappresenta la larghezza della forma, in unità di 1/4000 della forma padre.

**Remarks**

Si applica solo quando questa forma è nel gruppo o nel grafico.

**Example**

```
         if (shape.isInGroup() &&shape.getWidthInShape() == 2000)
             shape.setWidthInShape(4000);
```

**Returns:**
int
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Rappresenta la larghezza della forma, in unità di pollice.

**Example**

```
         if (shape.getWidthInch() == 3)
             shape.setWidthInch(1);
```

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


Rappresenta la larghezza della forma, in unità di punto.

**Example**

```
         if (shape.getWidthPt() == 3)
             shape.setWidthPt(1);
```

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


Restituisce la scala della larghezza, in unità di percentuale della larghezza originale dell'immagine. Se la forma non è un'immagine, la proprietà WidthScale restituisce solo 100;

**Example**

```
         if (shape.getWidthScale() == 3)
             shape.setWidthScale(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Ottiene l'oggetto [Worksheet](../../com.aspose.cells/worksheet) che contiene questa forma.

**Example**

```
         Worksheet worksheet = shape.getWorksheet();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getX() {#getX--}
```
public int getX()
```


Ottiene lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro, in unità di pixel.

**Example**

```
         if (shape.getX() == 3)
             shape.setX(1);
```

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Ottiene lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel.

**Example**

```
         if (shape.getY() == 3)
             shape.setY(1);
```

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Restituisce la posizione di una forma nell'ordine Z.

**Example**

```
         shape.setZOrderPosition(3);
```

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


Ottiene se il bordo della linea della forma è visibile.

**Example**

```
         if(shape.hasLine() == false)
             shape.setHasLine(true);
```

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAspectRatioLocked() {#isAspectRatioLocked--}
```
public boolean isAspectRatioLocked()
```


True indica che il rapporto d'aspetto della forma è bloccato.

**Remarks**

Solo per immagini e oggetti Ole.

**Example**

```
         shape.setAspectRatioLocked(false);
```

**Returns:**
boolean
### isDecorative() {#isDecorative--}
```
public boolean isDecorative()
```


Indica se l'oggetto è decorativo.

**Example**

```
         if (!shape.isDecorative())
             shape.setDecorative(true);
```

**Returns:**
boolean
### isEquation() {#isEquation--}
```
public boolean isEquation()
```


Indica se la forma contiene solo un'equazione.

**Example**

```
         //If true,the shape only contains an equation.
         if(shape.isEquation())
         {
             //The shape contains only an equation
         }
```

**Returns:**
boolean
### isFilled() {#isFilled--}
```
public boolean isFilled()
```


Indica se il formato di riempimento è visibile.

**Example**

```
         if(shape.isFilled() == false)
             shape.setFilled(true);
```

**Returns:**
boolean
### isFlippedHorizontally() {#isFlippedHorizontally--}
```
public boolean isFlippedHorizontally()
```


Ottiene se la forma è capovolta orizzontalmente .

**Example**

```
         if(shape.isFlippedHorizontally() == false)
             shape.setFlippedHorizontally(true);
```

**Returns:**
boolean
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


Ottiene se la forma è capovolta verticalmente .

**Example**

```
         if(shape.isFlippedVertically() == false)
             shape.setFlippedVertically(true);
```

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


Indica se questa forma è una forma di gruppo.

**Example**

```
         if(shape.isGroup())
         {
             //This shape is a group.
         }
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indica se l'oggetto è visibile.

**Example**

```
         shape.setHidden(false);
```

**Returns:**
boolean
### isInGroup() {#isInGroup--}
```
public boolean isInGroup()
```


Indica se la forma è raggruppata.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True indica che il rapporto d'aspetto della forma è bloccato.

**Remarks**

Solo per immagini e oggetti Ole. NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.IsAspectRatioLocked. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Example**

```
         shape.setHidden(false);
```

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


True indica che l'oggetto non può essere modificato quando il foglio è protetto. Nota che questo valore ha senso solo se il foglio di lavoro o gli oggetti nel foglio di lavoro sono protetti.

**Example**

```
         //Sets the specified shape to unlocked state
         if (shape.getWorksheet().isProtected() &&shape.isLocked())
         {
             shape.setLocked(false);
         }
 
         //Sets the specified shape to a locked state
         if (shape.getWorksheet().isProtected() &&!shape.isLocked())
         {
             shape.setLocked(true);
         }
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


Indica se l'oggetto è stampabile. Se False, questa forma non verrà stampata durante la stampa.

**Example**

```
         if(shape.isPrintable())
             shape.setPrintable(false);
```

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


Se il testo è o meno testo formattato.

**Example**

```
         if(shape.isRichText())
             System.out.println("The text is rich text.");
```

**Returns:**
boolean
### isSameSetting(Object obj) {#isSameSetting-java.lang.Object-}
```
public boolean isSameSetting(Object obj)
```


Restituisce se la forma è identica.

**Example**

```
         if (shape.isSameSetting(shape))
             System.out.println("Two objects the same.");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### isSmartArt() {#isSmartArt--}
```
public boolean isSmartArt()
```


Indica se la forma è un smart art.

**Remarks**

Solo per file ooxml.

**Example**

```
         //if true,the shape is a smart art.
         if(shape.isSmartArt())
         {
             //The shape is SmartArt object.
         }
```

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Ottiene il tipo di avvolgimento del testo della forma che contiene testo.

**Example**

```
         if (shape.isTextWrapped())
             shape.setTextWrapped(!shape.isTextWrapped());
```

**Returns:**
boolean
### isWordArt() {#isWordArt--}
```
public boolean isWordArt()
```


Indica se questa forma è un word art.

**Remarks**

Solo per la forma Legacy dei file xls.

**Example**

```
         if(shape.isWordArt())
         {
             //This shape is a WordArt object.
         }
```

**Returns:**
boolean
### moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Sposta la forma in un intervallo specificato.

**Example**

```
         shape.moveToRange(12, 3, 13, 5);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| bottomRow | int | Indice della riga in basso a destra |
| rightColumn | int | Indice della colonna in basso a destra |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeActiveXControl() {#removeActiveXControl--}
```
public void removeActiveXControl()
```


Rimuove il controllo ActiveX.

**Example**

```
         if(shape.getActiveXControl() != null)
         {
             shape.removeActiveXControl();
         }
```

### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


Rimuove il collegamento ipertestuale della forma.

**Example**

```
         shape.removeHyperlink();
```

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto [Shape](../../com.aspose.cells/shape).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setAnchorType(int value) {#setAnchorType-int-}
```
public void setAnchorType(int value)
```


Imposta il tipo del segnaposto di ancoraggio della forma.

Vedi [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setAspectRatioLocked(boolean value) {#setAspectRatioLocked-boolean-}
```
public void setAspectRatioLocked(boolean value)
```


True indica che il rapporto d'aspetto della forma è bloccato.

**Remarks**

Solo per immagini e oggetti Ole.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoShapeType(int value) {#setAutoShapeType-int-}
```
public void setAutoShapeType(int value)
```


Imposta il tipo di forma automatica.

Vedi [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Rappresenta la larghezza dello spostamento verticale della forma dalla sua riga d'angolo inferiore, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCreateId(UUID value) {#setCreateId-java.util.UUID-}
```
public void setCreateId(UUID value)
```


Imposta l'ID di creazione per questa forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.UUID |  |

### setDecorative(boolean value) {#setDecorative-boolean-}
```
public void setDecorative(boolean value)
```


Indica se l'oggetto è decorativo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFilled(boolean value) {#setFilled-boolean-}
```
public void setFilled(boolean value)
```


Indica se il formato di riempimento è visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFlippedHorizontally(boolean value) {#setFlippedHorizontally-boolean-}
```
public void setFlippedHorizontally(boolean value)
```


Imposta se la forma è capovolta orizzontalmente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Imposta se la forma è capovolta verticalmente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFont(Font value) {#setFont-com.aspose.cells.Font-}
```
public void setFont(Font value)
```


Rappresenta il carattere della forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Font](../../com.aspose.cells/font) |  |

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


Rappresenta l'altezza della forma, in unità di centimetri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setHeightInShape(int value) {#setHeightInShape-int-}
```
public void setHeightInShape(int value)
```


Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore, in unità di 1/4000 dell'altezza della forma genitore.

**Remarks**

Si applica solo quando questa forma è nel gruppo o nel grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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


Imposta la stringa HTML che contiene dati e alcuni formati in questa casella di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setInputRange(String value) {#setInputRange-java.lang.String-}
```
public void setInputRange(String value)
```


Imposta l'intervallo del foglio di lavoro usato per riempire la casella combinata specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setInputRange(String formula, boolean isR1C1, boolean isLocal) {#setInputRange-java.lang.String-boolean-boolean-}
```
public void setInputRange(String formula, boolean isR1C1, boolean isLocal)
```


Imposta l'intervallo usato per riempire il controllo.

**Example**

```
         //After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.
 
         for (int i = 0; i? ++i)
         {
             Cell cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | L'intervallo utilizzato per riempire il controllo. |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |

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

### setLeftInShape(int value) {#setLeftInShape-int-}
```
public void setLeftInShape(int value)
```


Rappresenta lo spostamento orizzontale della forma dal bordo sinistro della forma padre, in unità di 1/4000 della larghezza della forma padre.

**Remarks**

Si applica solo quando questa forma è nel gruppo o nel grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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


Imposta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro.

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

### setLinkedCell(String formula, boolean isR1C1, boolean isLocal) {#setLinkedCell-java.lang.String-boolean-boolean-}
```
public void setLinkedCell(String formula, boolean isR1C1, boolean isLocal)
```


Imposta l'intervallo collegato al valore del controllo.

**Example**

```
         //After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape scrollBar = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ScrollBar,2, 0, 2, 0, 30, 130);
 
         //Form Controls
         Shape scrollBar = book.getWorksheets().get(0).getShapes().addScrollBar(2, 0, 2, 0, 130, 30);
 
         //Sets the range linked to the control's value.
         scrollBar.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | L'intervallo collegato al valore del controllo. |
| isR1C1 | boolean | Indica se la formula deve essere formattata come R1C1. |
| isLocal | boolean | Indica se la formula deve essere formattata in base alla lingua locale. |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


True indica che il rapporto d'aspetto della forma è bloccato.

**Remarks**

Solo per immagini e oggetti Ole. NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.IsAspectRatioLocked. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True indica che l'oggetto non può essere modificato quando il foglio è protetto. Nota che questo valore ha senso solo se il foglio di lavoro o gli oggetti nel foglio di lavoro sono protetti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLockedProperty(int type, boolean value) {#setLockedProperty-int-boolean-}
```
public void setLockedProperty(int type, boolean value)
```


Imposta la proprietà bloccata.

**Example**

```
         shape.setLockedProperty(ShapeLockType.ADJUST_HANDLES, true);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). Il tipo bloccato. |
| valore | boolean | Il valore della proprietà. |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Imposta lo spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro.

**Remarks**

L'intervallo di valore è da 0 a 1024.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Imposta lo spostamento verticale della forma dalla riga dell'angolo inferiore destro.

**Remarks**

L'intervallo di valore è da 0 a 256.

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

### setMacroName(String value) {#setMacroName-java.lang.String-}
```
public void setMacroName(String value)
```


Imposta il nome della macro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome della forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti. La proprietà controlla il posizionamento di un oggetto su un foglio di lavoro.

Vedi [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Indica se l'oggetto è stampabile. Se False, questa forma non verrà stampata durante la stampa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

### setSoftEdges(double value) {#setSoftEdges-double-}
```
public void setSoftEdges(double value)
```


Imposta il raggio della sfocatura da applicare ai bordi, in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Imposta il testo di questa forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Imposta la direzione del flusso di testo per questo oggetto.

Vedi [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Imposta il tipo di allineamento orizzontale del testo della forma.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Imposta il tipo di overflow orizzontale del testo della forma che contiene testo.

Vedi [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextOptions(TextOptions value) {#setTextOptions-com.aspose.cells.TextOptions-}
```
public void setTextOptions(TextOptions value)
```


Rappresenta le opzioni di testo della forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [TextOptions](../../com.aspose.cells/textoptions) |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Imposta il tipo di orientamento del testo della forma.

Vedi [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Imposta il tipo di forma di testo predefinito.

Vedi [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Imposta il tipo di allineamento verticale del testo della forma.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Imposta il tipo di overflow verticale del testo della forma che contiene testo.

Vedi [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

### setTopInShape(int value) {#setTopInShape-int-}
```
public void setTopInShape(int value)
```


Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore, in unità di 1/4000 dell'altezza della forma genitore.

**Remarks**

Si applica solo quando questa forma è nel gruppo o nel grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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


Imposta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Imposta lo spostamento orizzontale della forma dalla colonna dell'angolo in alto a sinistra.

**Remarks**

L'intervallo di valore è da 0 a 1024.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Imposta lo spostamento verticale della forma dalla riga dell'angolo in alto a sinistra.

**Remarks**

L'intervallo di valore è da 0 a 256.

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


Rappresenta l'indice della riga superiore.

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

### setWidthInShape(int value) {#setWidthInShape-int-}
```
public void setWidthInShape(int value)
```


Rappresenta la larghezza della forma, in unità di 1/4000 della forma padre.

**Remarks**

Si applica solo quando questa forma è nel gruppo o nel grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

### toFrontOrBack(int orders) {#toFrontOrBack-int-}
```
public void toFrontOrBack(int orders)
```


Porta la forma in primo piano o invia la forma sullo sfondo.

**Example**

```
         shape.toFrontOrBack(2);
         //or shape.ToFrontOrBack(-1);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| orders | int | Se è inferiore a zero, imposta la forma sullo sfondo. Se è superiore a zero, porta la forma in primo piano. |

### toImage(OutputStream stream, ImageFormat imageFormat) {#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-}
```
public void toImage(OutputStream stream, ImageFormat imageFormat)
```


Crea l'immagine della forma e la salva in un flusso nel formato specificato.

**Remarks**

I seguenti formati sono supportati: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso di output. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | Il formato in cui salvare l'immagine. |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Salva la forma in un flusso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Salva la forma in un file.

**Example**

```
         ImageOrPrintOptions op = new ImageOrPrintOptions();
         shape.toImage("exmaple.png", op);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| imageFile | java.lang.String |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


Aggiorna il valore selezionato con il valore della cella collegata.

**Example**

```
         Cell cell = null;
         for (int i = 0; i? ++i)
         {
             cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
 
         ListBox listbx = (ListBox)listBox;
 
         //Set the value of cell A12
         cell = book.getWorksheets().get(0).getCells().get(11, 0);
         cell.setValue(3);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
 
         //-1 default, no option selected
         if(listbx.isSelected(2))
         {
             //Option 3 of the ListBox is selected
         }
 
         //Change the value of a linked cell
         cell.setValue(4);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
         if(listbx.isSelected(3))
         {
             //Option 4 of the ListBox is selected
         }
```

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

