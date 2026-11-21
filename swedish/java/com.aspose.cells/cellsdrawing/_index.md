---
title: "CellsDrawing"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar autoformen och ritningsobjektet."
type: docs
url: /sv/java/com.aspose.cells/cellsdrawing/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Shape](../../com.aspose.cells/shape)
```
public class CellsDrawing extends Shape
```

Representerar autoformen och ritningsobjektet.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Lägger till en hyperlänk till formen. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Flyttar bilden till det övre högra hörnet. |
| [calculateTextSize()](#calculateTextSize--) | Beräkna om textområdet |
| [characters(int startIndex, int length)](#characters-int-int-) | Returnerar ett Characters-objekt som representerar ett intervall av tecken inom texten. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fitToTextSize()](#fitToTextSize--) | Beräkna om ett textområde som är lämpligt för att visa allt textinnehåll. |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Formaterar vissa tecken med teckensnittsinställningen. |
| [getActiveXControl()](#getActiveXControl--) | Hämtar ActiveX-kontrollen. |
| [getActualBox()](#getActualBox--) | Hämta den faktiska positionen och storleken på formen (efter att rotation, vändning osv. har tillämpats). |
| [getActualLowerRightRow()](#getActualLowerRightRow--) | Hämta den faktiska nedersta raden. |
| [getAlternativeText()](#getAlternativeText--) | Returnerar eller anger den beskrivande (alternativa) textsträngen för [Shape](../../com.aspose.cells/shape)-objektet. |
| [getAnchorType()](#getAnchorType--) | Hämtar typen av platshållaren för formens ankare. |
| [getAutoShapeType()](#getAutoShapeType--) | Hämtar den automatiska formtypen. |
| [getBottom()](#getBottom--) | Representerar bredden på formens vertikala förskjutning från dess nedre hörnrad, i enhet pixlar. |
| [getCharacters()](#getCharacters--) | Returnerar alla Characters-objekt som representerar ett teckenintervall inom texten. |
| [getClass()](#getClass--) |  |
| [getConnectionPoints()](#getConnectionPoints--) | Hämta anslutningspunkterna |
| [getControlData()](#getControlData--) | Hämtar kontrollens data. |
| [getCreateId()](#getCreateId--) | Hämtar skapande-ID för denna form. |
| [getFill()](#getFill--) | Returnerar ett [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--)‑objekt som innehåller fyllningsformateringsegenskaper för den angivna formen. |
| [getFillFormat()](#getFillFormat--) | Returnerar ett MsoFillFormat‑objekt som innehåller fyllningsformateringsegenskaper för den angivna formen. |
| [getFont()](#getFont--) | Representerar formens teckensnitt. |
| [getFormatPicture()](#getFormatPicture--) | Hämtar alternativen för bildformatet. |
| [getGeometry()](#getGeometry--) | Hämtar geometrin |
| [getGlow()](#getGlow--) | Representerar ett [GlowEffect](../../com.aspose.cells/gloweffect)‑objekt som specificerar glödeffekt för diagramelementet eller formen. |
| [getGroup()](#getGroup--) | Hämtar gruppformen som innehåller denna form. |
| [getHeight()](#getHeight--) | Representerar höjden på formen, i enhet pixlar. |
| [getHeightCM()](#getHeightCM--) | Representerar höjden på formen, i enhet centimeter. |
| [getHeightInShape()](#getHeightInShape--) | Representerar den vertikala förskjutningen av formen från den översta kanten av föräldraformen, i enhet 1/4000 av föräldraformens höjd. |
| [getHeightInch()](#getHeightInch--) | Representerar höjden på formen, i enhet tum. |
| [getHeightPt()](#getHeightPt--) | Representerar höjden på formen, i enhet punkter. |
| [getHeightScale()](#getHeightScale--) | Hämtar höjds‑skalan, i enhet procent av den ursprungliga bildens höjd. |
| [getHtmlText()](#getHtmlText--) | Hämtar HTML-strängen som innehåller data och vissa format i den här textrutan. |
| [getHyperlink()](#getHyperlink--) | Hämtar hyperlänken för formen. |
| [getId()](#getId--) | Hämtar identifieraren för denna form. |
| [getInputRange()](#getInputRange--) | Hämtar kalkylbladsintervallet som används för att fylla den angivna kombinationsrutan. |
| [getInputRange(boolean isR1C1, boolean isLocal)](#getInputRange-boolean-boolean-) | Hämtar intervallet som används för att fylla kontrollen. |
| [getLeft()](#getLeft--) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixlar. |
| [getLeftCM()](#getLeftCM--) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet centimeter. |
| [getLeftInShape()](#getLeftInShape--) | Representerar den horisontella förskjutningen av formen från den vänstra kanten av föräldraformen, i enhet 1/4000 av föräldraformens bredd. |
| [getLeftInch()](#getLeftInch--) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet tum. |
| [getLeftToCorner()](#getLeftToCorner--) | Hämtar den horisontella förskjutningen av formen från kalkylbladets vänstra kant. |
| [getLine()](#getLine--) | Hämtar linjestil |
| [getLineFormat()](#getLineFormat--) | Returnerar ett MsoLineFormat-objekt som innehåller linjeformateringsegenskaper för den angivna formen. |
| [getLinkedCell()](#getLinkedCell--) | Hämtar kalkylbladsintervallet som är länkat till kontrollens värde. |
| [getLinkedCell(boolean isR1C1, boolean isLocal)](#getLinkedCell-boolean-boolean-) | Hämtar intervallet som är länkat till kontrollens värde. |
| [getLockedProperty(int type)](#getLockedProperty-int-) | Hämtar värdet för egenskapen låst. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Hämtar formens horisontella förskjutning från dess nedre högra hörnkolumn. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Hämtar formens vertikala förskjutning från dess nedre högra hörnrad. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Representerar index för nedre högra hörnkolumn. |
| [getLowerRightRow()](#getLowerRightRow--) | Representerar index för nedre högra hörnrad. |
| [getMacroName()](#getMacroName--) | Hämtar namnet på makrot. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Hämtar ritningstyp. |
| [getName()](#getName--) | Hämtar namnet på formen. |
| [getPaths()](#getPaths--) | Hämtar sökvägarna för en anpassad geometrisk form. |
| [getPlacement()](#getPlacement--) | Representerar hur ritobjektet är fäst vid cellerna under det. |
| [getReflection()](#getReflection--) | Representerar ett [ReflectionEffect](../../com.aspose.cells/reflectioneffect) objekt som specificerar reflektionseffekt för diagramelementet eller formen. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Indikerar om formen är relativ till originalbildens storlek. |
| [getResultOfSmartArt()](#getResultOfSmartArt--) | Konverterar smart art till grupperade former. |
| [getRichFormattings()](#getRichFormattings--) | Returnerar alla Characters-objekt som representerar ett teckenintervall inom texten. |
| [getRight()](#getRight--) | Representerar bredden på formens horisontella förskjutning från dess nedre högra hörnkolumn, i enhet pixlar. |
| [getRotationAngle()](#getRotationAngle--) | Hämtar rotationen av formen. |
| [getShadowEffect()](#getShadowEffect--) | Representerar ett [ShadowEffect](../../com.aspose.cells/shadoweffect) objekt som specificerar skuggeffekt för diagramelementet eller formen. |
| [getSoftEdges()](#getSoftEdges--) | Hämtar suddradie radien som ska appliceras på kanterna, i enheten punkter. |
| [getSpid()](#getSpid--) | Anger en valfri strängidentifierare som ett program kan använda för att identifiera den specifika formen. |
| [getSpt()](#getSpt--) | Anger ett valfritt tal som ett program kan använda för att associera den specifika formen med en definierad formtyp. |
| [getText()](#getText--) | Hämtar texten för denna form. |
| [getTextBody()](#getTextBody--) | Hämtar inställningen för formens text. |
| [getTextBoxOptions()](#getTextBoxOptions--) | Hämtar textinformationen i formen |
| [getTextDirection()](#getTextDirection--) | Hämtar riktningen för textflödet för detta objekt. |
| [getTextEffect()](#getTextEffect--) | Returnerar ett TextEffectFormat-objekt som innehåller text-effektformateringsegenskaper för den angivna formen. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Hämtar den horisontella justeringstypen för formens text. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Hämtar den horisontella översvämningstypen för formen som innehåller text. |
| [getTextOptions()](#getTextOptions--) | Representerar textalternativen för formen. |
| [getTextOrientationType()](#getTextOrientationType--) | Hämtar textorienteringstypen för formen. |
| [getTextShapeType()](#getTextShapeType--) | Hämtar den förinställda textformstypen. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Hämtar den vertikala justeringstypen för formens text. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Hämtar den vertikala översvämningstypen för formen som innehåller text. |
| [getThreeDFormat()](#getThreeDFormat--) | Hämtar 3D-formatet för formen. |
| [getTitle()](#getTitle--) | Anger titeln (rubriken) för det aktuella formobjektet. |
| [getTop()](#getTop--) | Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten pixlar. |
| [getTopCM()](#getTopCM--) | Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten centimeter. |
| [getTopInShape()](#getTopInShape--) | Representerar den vertikala förskjutningen för formen från den översta kanten av föräldraformen, i enheten 1/4000 av föräldraformens höjd. |
| [getTopInch()](#getTopInch--) | Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten tum. |
| [getTopToCorner()](#getTopToCorner--) | Hämtar den vertikala förskjutningen för formen från kalkylbladets översta kant, i enheten pixlar. |
| [getType()](#getType--) | Hämtar den automatiska formtypen. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Hämtar formens horisontella förskjutning från dess övre vänstra kolumn. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Hämtar formens vertikala förskjutning från dess övre vänstra rad. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Representerar index för övre vänstra kolumnen. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Representerar det översta radindexet. |
| [getWidth()](#getWidth--) | Representerar bredden på shape, i enheten pixlar. |
| [getWidthCM()](#getWidthCM--) | Representerar bredden på shape, i enheten centimeter. |
| [getWidthInShape()](#getWidthInShape--) | Representerar bredden på shape, i enheten 1/4000 av den överordnade shape. |
| [getWidthInch()](#getWidthInch--) | Representerar bredden på shape, i enheten tum. |
| [getWidthPt()](#getWidthPt--) | Representerar bredden på shape, i enheten punkt. |
| [getWidthScale()](#getWidthScale--) | Hämtar breddskalan, i enheten procent av den ursprungliga bildens bredd. |
| [getWorksheet()](#getWorksheet--) | Hämtar [Worksheet](../../com.aspose.cells/worksheet)-objektet som innehåller denna shape. |
| [getX()](#getX--) | Hämtar den horisontella förskjutningen av shape från kalkylbladets vänstra kant, i enheten pixlar. |
| [getY()](#getY--) | Hämtar den vertikala förskjutningen av shape från kalkylbladets övre kant, i enheten pixlar. |
| [getZOrderPosition()](#getZOrderPosition--) | Returnerar positionen för en shape i z-ordningen. |
| [hasLine()](#hasLine--) | Hämtar om linjekanten på shape är synlig. |
| [hashCode()](#hashCode--) |  |
| [isAspectRatioLocked()](#isAspectRatioLocked--) | Sant betyder att bildförhållandet för shape är låst. |
| [isDecorative()](#isDecorative--) | Indikerar om objektet är dekorativt. |
| [isEquation()](#isEquation--) | Indikerar om shape endast innehåller en ekvation. |
| [isFilled()](#isFilled--) | Indikerar om fyllningsformatet är synligt. |
| [isFlippedHorizontally()](#isFlippedHorizontally--) | Hämtar om shape är horisontellt speglad. |
| [isFlippedVertically()](#isFlippedVertically--) | Hämtar om shape är vertikalt speglad. |
| [isGroup()](#isGroup--) | Indikerar om denna shape är en gruppshape. |
| [isHidden()](#isHidden--) | Indikerar om objektet är synligt. |
| [isInGroup()](#isInGroup--) | Indikerar om shape är grupperad. |
| [isLockAspectRatio()](#isLockAspectRatio--) | Sant betyder att bildförhållandet för shape är låst. |
| [isLocked()](#isLocked--) | Sant betyder att objektet inte kan ändras när bladet är skyddat. |
| [isPrintable()](#isPrintable--) | Indikerar om objektet kan skrivas ut. |
| [isRichText()](#isRichText--) | Om texten är rik text eller inte. |
| [isSameSetting(Object obj)](#isSameSetting-java.lang.Object-) | Returnerar om shape är densamma. |
| [isSmartArt()](#isSmartArt--) | Anger om formen är en smart art. |
| [isTextWrapped()](#isTextWrapped--) | Hämtar den typ av textomslag för formen som innehåller text. |
| [isWordArt()](#isWordArt--) | Anger om denna form är en word art. |
| [moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)](#moveToRange-int-int-int-int-) | Flyttar formen till ett angivet område. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeActiveXControl()](#removeActiveXControl--) | Ta bort ActiveX-kontrollen. |
| [removeHyperlink()](#removeHyperlink--) | Tar bort hyperlänken för formen. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Returnerar eller anger den beskrivande (alternativa) textsträngen för [Shape](../../com.aspose.cells/shape)-objektet. |
| [setAnchorType(int value)](#setAnchorType-int-) | Ställer in typen av formens ankareplatshållare. |
| [setAspectRatioLocked(boolean value)](#setAspectRatioLocked-boolean-) | Sant betyder att bildförhållandet för shape är låst. |
| [setAutoShapeType(int value)](#setAutoShapeType-int-) | Ställer in autoformstypen. |
| [setBottom(int value)](#setBottom-int-) | Representerar bredden på formens vertikala förskjutning från dess nedre hörnrad, i enhet pixlar. |
| [setCreateId(UUID value)](#setCreateId-java.util.UUID-) | Ställer in skapande-ID för denna form. |
| [setDecorative(boolean value)](#setDecorative-boolean-) | Indikerar om objektet är dekorativt. |
| [setFilled(boolean value)](#setFilled-boolean-) | Indikerar om fyllningsformatet är synligt. |
| [setFlippedHorizontally(boolean value)](#setFlippedHorizontally-boolean-) | Ställer in om formen är horisontellt speglad. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Ställer in om formen är vertikalt speglad. |
| [setFont(Font value)](#setFont-com.aspose.cells.Font-) | Representerar formens teckensnitt. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Ställer in att linjekanten på formen är synlig. |
| [setHeight(int value)](#setHeight-int-) | Representerar höjden på formen, i enhet pixlar. |
| [setHeightCM(double value)](#setHeightCM-double-) | Representerar höjden på formen, i enhet centimeter. |
| [setHeightInShape(int value)](#setHeightInShape-int-) | Representerar den vertikala förskjutningen av formen från den översta kanten av föräldraformen, i enhet 1/4000 av föräldraformens höjd. |
| [setHeightInch(double value)](#setHeightInch-double-) | Representerar höjden på formen, i enhet tum. |
| [setHeightPt(double value)](#setHeightPt-double-) | Representerar höjden på formen, i enhet punkter. |
| [setHeightScale(int value)](#setHeightScale-int-) | Ställer in höjds-skalan i procent av den ursprungliga bildens höjd. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indikerar om objektet är synligt. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Ställer in HTML-strängen som innehåller data och vissa format i den här textrutan. |
| [setInputRange(String value)](#setInputRange-java.lang.String-) | Ställer in kalkylbladsområdet som används för att fylla den angivna kombinationsrutan. |
| [setInputRange(String formula, boolean isR1C1, boolean isLocal)](#setInputRange-java.lang.String-boolean-boolean-) | Ställer in området som används för att fylla kontrollen. |
| [setLeft(int value)](#setLeft-int-) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixlar. |
| [setLeftCM(double value)](#setLeftCM-double-) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet centimeter. |
| [setLeftInShape(int value)](#setLeftInShape-int-) | Representerar den horisontella förskjutningen av formen från den vänstra kanten av föräldraformen, i enhet 1/4000 av föräldraformens bredd. |
| [setLeftInch(double value)](#setLeftInch-double-) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet tum. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Ställer in den horisontella förskjutningen av formen från kalkylbladets vänstra kant. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Ställer in kalkylbladsområdet som är länkat till kontrollens värde. |
| [setLinkedCell(String formula, boolean isR1C1, boolean isLocal)](#setLinkedCell-java.lang.String-boolean-boolean-) | Ställer in området som är länkat till kontrollens värde. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | Sant betyder att bildförhållandet för shape är låst. |
| [setLocked(boolean value)](#setLocked-boolean-) | Sant betyder att objektet inte kan ändras när bladet är skyddat. |
| [setLockedProperty(int type, boolean value)](#setLockedProperty-int-boolean-) | Ställ in den låsta egenskapen. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Ställer in formens horisontella förskjutning från dess nedre högra kolumn. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Ställer in formens vertikala förskjutning från dess nedre högra rad. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Representerar index för nedre högra hörnkolumn. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Representerar index för nedre högra hörnrad. |
| [setMacroName(String value)](#setMacroName-java.lang.String-) | Ställer in namnet på makrot. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på formen. |
| [setPlacement(int value)](#setPlacement-int-) | Representerar hur ritobjektet är fäst vid cellerna under det. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Indikerar om objektet kan skrivas ut. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Indikerar om formen är relativ till originalbildens storlek. |
| [setRight(int value)](#setRight-int-) | Representerar bredden på formens horisontella förskjutning från dess nedre högra hörnkolumn, i enhet pixlar. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Ställer in rotationen av formen. |
| [setSoftEdges(double value)](#setSoftEdges-double-) | Ställer in suddradien som ska tillämpas på kanterna, i enheten punkter. |
| [setText(String value)](#setText-java.lang.String-) | Ställer in texten för den här formen. |
| [setTextDirection(int value)](#setTextDirection-int-) | Ställer in riktningen för textflödet för detta objekt. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Ställer in den horisontella justeringstypen för texten i formen. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Ställer in den horisontella översvämningstypen för texten i formen som innehåller text. |
| [setTextOptions(TextOptions value)](#setTextOptions-com.aspose.cells.TextOptions-) | Representerar textalternativen för formen. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Ställer in orienteringstypen för texten i formen. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Ställer in den förinställda textformstypen. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Ställer in den vertikala justeringstypen för texten i formen. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Ställer in den vertikala översvämningstypen för texten i formen som innehåller text. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Ställer in typen av textbrytning för formen som innehåller text. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Anger titeln (rubriken) för det aktuella formobjektet. |
| [setTop(int value)](#setTop-int-) | Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten pixlar. |
| [setTopCM(double value)](#setTopCM-double-) | Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten centimeter. |
| [setTopInShape(int value)](#setTopInShape-int-) | Representerar den vertikala förskjutningen för formen från den översta kanten av föräldraformen, i enheten 1/4000 av föräldraformens höjd. |
| [setTopInch(double value)](#setTopInch-double-) | Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten tum. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Ställer in den vertikala förskjutningen för formen från kalkylbladets övre kant, i enheten pixlar. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Ställer in formens horisontella förskjutning från dess övre vänstra kolumn. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Ställer in formens vertikala förskjutning från dess övre vänstra rad. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Representerar index för övre vänstra kolumnen. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Representerar det översta radindexet. |
| [setWidth(int value)](#setWidth-int-) | Representerar bredden på shape, i enheten pixlar. |
| [setWidthCM(double value)](#setWidthCM-double-) | Representerar bredden på shape, i enheten centimeter. |
| [setWidthInShape(int value)](#setWidthInShape-int-) | Representerar bredden på shape, i enheten 1/4000 av den överordnade shape. |
| [setWidthInch(double value)](#setWidthInch-double-) | Representerar bredden på shape, i enheten tum. |
| [setWidthPt(double value)](#setWidthPt-double-) | Representerar bredden på shape, i enheten punkt. |
| [setWidthScale(int value)](#setWidthScale-int-) | Ställer in breddskalan, i enheten procent av den ursprungliga bildens bredd. |
| [setX(int value)](#setX-int-) | Ställer in den horisontella förskjutningen för formen från kalkylbladets vänstra kant, i enheten pixlar. |
| [setY(int value)](#setY-int-) | Ställer in den vertikala förskjutningen för formen från kalkylbladets övre kant, i enheten pixlar. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Returnerar positionen för en shape i z-ordningen. |
| [toFrontOrBack(int orders)](#toFrontOrBack-int-) | Flyttar formen till framkant eller skickar formen till bakgrunden. |
| [toImage(OutputStream stream, ImageFormat imageFormat)](#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-) | Skapar formens bild och sparar den till en ström i det angivna formatet. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Sparar formen till en ström. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Sparar formen till en fil. |
| [toString()](#toString--) |  |
| [updateSelectedValue()](#updateSelectedValue--) | Uppdatera det valda värdet med värdet från den länkade cellen. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public Hyperlink addHyperlink(String address)
```


Lägger till en hyperlänk till formen.

**Example**

```
         Hyperlink hyperlink = shape.addHyperlink("https://www.aspose.com/");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| adress | java.lang.String | Adress för hyperlänken. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - Returns the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Flyttar bilden till det övre högra hörnet.

**Example**

```
         shape.alignTopRightCorner(2, 5);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | radindexet. |
| rightColumn | int | kolumnens index. |

### calculateTextSize() {#calculateTextSize--}
```
public int[] calculateTextSize()
```


Beräkna om textområdet

**Example**

```
         //The size of the text area is:w=size[0],h=size[1]
         int[] size = shape.calculateTextSize();
```

**Returns:**
int[] - Textens storlek i en array (bredd och höjd).
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Returnerar ett Characters-objekt som representerar ett intervall av tecken inom texten.

**Remarks**

Denna metod fungerar endast på form med titel.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int | Indexet för tecknets början. |
| length | int | Antalet tecken. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### fitToTextSize() {#fitToTextSize--}
```
public void fitToTextSize()
```


Beräkna om ett textområde som är lämpligt för att visa allt textinnehåll.

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


Formaterar vissa tecken med teckensnittsinställningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | int | Startindexet. |
| length | int | Längden. |
| font | [Font](../../com.aspose.cells/font) | Typsnittsinställningen. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flaggan för typsnittsinställningen. |

### getActiveXControl() {#getActiveXControl--}
```
public ActiveXControl getActiveXControl()
```


Hämtar ActiveX-kontrollen.

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


Hämta den faktiska positionen och storleken på formen (efter att rotation, vändning osv. har tillämpats).

**Remarks**

Obs: Gränssnittet är inte fullt funktionellt, särskilt är platsinformationen felaktig. Det rekommenderas att inte använda detta gränssnitt förrän funktionen är komplett.

**Example**

```
         float[] box = shape.getActualBox();
         System.out.println("x = " + box[0]);
         System.out.println("y = " + box[1]);
         System.out.println("w = " + box[2]);
         System.out.println("h = " + box[3]);
```

**Returns:**
float[] - Returnerar positionen och storleken i ordning x, y, w, h
### getActualLowerRightRow() {#getActualLowerRightRow--}
```
public int getActualLowerRightRow()
```


Hämta den faktiska nedersta raden.

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


Returnerar eller anger den beskrivande (alternativa) textsträngen för [Shape](../../com.aspose.cells/shape)-objektet.

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


Hämtar typen av platshållaren för formens ankare.

Se [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

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


Hämtar den automatiska formtypen.

Se [AutoShapeType](../../com.aspose.cells/autoshapetype).

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


Representerar bredden på formens vertikala förskjutning från dess nedre hörnrad, i enhet pixlar.

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


Returnerar alla Characters-objekt som representerar ett teckenintervall inom texten.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället Shape.GetRichFormattings()-metoden. Denna metod kommer att tas bort 12 månader senare, från och med november 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Returns:**
java.util.ArrayList - Alla teckenobjekt
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


Hämta anslutningspunkterna

**Example**

```
         float[][] points = shape.getConnectionPoints();
```

**Returns:**
float[][] - [X,Y]-par för anslutningspunkten. Varje element är en float[2]-array, [0] representerar x och [1] representerar y.
### getControlData() {#getControlData--}
```
public byte[] getControlData()
```


Hämtar kontrollens data.

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


Hämtar skapande-ID för denna form.

**Example**

```
         System.out.println(shape.getCreateId());
         java.util.UUID g = java.util.UUID.randomUUID();
         shape.setCreateId(g);
         System.out.println(shape.getCreateId());
```

**Returns:**
java.util.UUID
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Returnerar ett [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--)‑objekt som innehåller fyllningsformateringsegenskaper för den angivna formen.

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


Returnerar ett MsoFillFormat‑objekt som innehåller fyllningsformateringsegenskaper för den angivna formen.

**Remarks**

OBS: Detta medlemskap är nu föråldrat. Använd istället Shape.Fill-egenskapen. Denna egenskap kommer att tas bort 12 månader senare, från och med juli 2016. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[MsoFillFormat](../../com.aspose.cells/msofillformat)
### getFont() {#getFont--}
```
public Font getFont()
```


Representerar formens teckensnitt.

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


Hämtar alternativen för bildformatet.

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


Hämtar geometrin

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


Representerar ett [GlowEffect](../../com.aspose.cells/gloweffect)‑objekt som specificerar glödeffekt för diagramelementet eller formen.

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


Hämtar gruppformen som innehåller denna form.

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


Representerar höjden på formen, i enhet pixlar.

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


Representerar höjden på formen, i enhet centimeter.

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


Representerar den vertikala förskjutningen av formen från den översta kanten av föräldraformen, i enhet 1/4000 av föräldraformens höjd.

**Remarks**

Gäller endast när denna form är i en grupp eller ett diagram.

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


Representerar höjden på formen, i enhet tum.

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


Representerar höjden på formen, i enhet punkter.

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


Hämtar höjds-skalan, i enhet procent av den ursprungliga bildens höjd. Om formen inte är en bild, returnerar HeightScale‑egenskapen endast 100;

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


Hämtar HTML-strängen som innehåller data och vissa format i den här textrutan.

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


Hämtar hyperlänken för formen.

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


Hämtar identifieraren för denna form.

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


Hämtar kalkylbladsintervallet som används för att fylla den angivna kombinationsrutan.

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


Hämtar intervallet som används för att fylla kontrollen.

**Example**

```
         String range = shape.getInputRange(false, true);
         //If successful, a value like "$A$1:$A$3" will be returned
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |

**Returns:**
java.lang.String - Intervallet som används för att fylla kontrollen.
### getLeft() {#getLeft--}
```
public int getLeft()
```


Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixlar.

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


Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet centimeter.

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


Representerar den horisontella förskjutningen av formen från den vänstra kanten av föräldraformen, i enhet 1/4000 av föräldraformens bredd.

**Remarks**

Gäller endast när denna form är i en grupp eller ett diagram.

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


Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet tum.

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


Hämtar den horisontella förskjutningen av formen från kalkylbladets vänstra kant.

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


Hämtar linjestil

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


Returnerar ett MsoLineFormat-objekt som innehåller linjeformateringsegenskaper för den angivna formen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället Shape.Line‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare sedan juli 2016. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[MsoLineFormat](../../com.aspose.cells/msolineformat)
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Hämtar kalkylbladsintervallet som är länkat till kontrollens värde.

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


Hämtar intervallet som är länkat till kontrollens värde.

**Example**

```
         //You may get results like '$A$1'
         String link = shape.getLinkedCell(false, false);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |

**Returns:**
java.lang.String - Intervallet som är länkat till kontrollens värde.
### getLockedProperty(int type) {#getLockedProperty-int-}
```
public boolean getLockedProperty(int type)
```


Hämtar värdet för egenskapen låst.

**Example**

```
         int noAdjustHandles = 0;
         if (shape.getLockedProperty(ShapeLockType.ADJUST_HANDLES))
             noAdjustHandles = 1;
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). Typen av den låsta form‑egenskapen. |

**Returns:**
boolean - Returnerar värdet av den låsta egenskapen.
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Hämtar formens horisontella förskjutning från dess nedre högra hörnkolumn.

**Remarks**

Värdeintervallet är 0 till 1024.

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


Hämtar formens vertikala förskjutning från dess nedre högra hörnrad.

**Remarks**

Värdeintervallet är 0 till 256.

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


Representerar index för nedre högra hörnkolumn.

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


Representerar index för nedre högra hörnrad.

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


Hämtar namnet på makrot.

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


Hämtar ritningstyp.

Se [MsoDrawingType](../../com.aspose.cells/msodrawingtype).

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


Hämtar namnet på formen.

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


Hämtar sökvägarna för en anpassad geometrisk form.

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


Representerar hur ritobjektet är fäst vid cellerna under det. Egenskapen styr placeringen av ett objekt på ett kalkylblad.

Se [PlacementType](../../com.aspose.cells/placementtype).

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


Representerar ett [ReflectionEffect](../../com.aspose.cells/reflectioneffect) objekt som specificerar reflektionseffekt för diagramelementet eller formen.

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


Indikerar om formen är relativ till originalbildens storlek.

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


Konverterar smart art till grupperade former.

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


Returnerar alla Characters-objekt som representerar ett teckenintervall inom texten.

**Example**

```
         FontSetting[] list = shape.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Alla tecken‑objekt
### getRight() {#getRight--}
```
public int getRight()
```


Representerar bredden på formens horisontella förskjutning från dess nedre högra hörnkolumn, i enhet pixlar.

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


Hämtar rotationen av formen.

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


Representerar ett [ShadowEffect](../../com.aspose.cells/shadoweffect) objekt som specificerar skuggeffekt för diagramelementet eller formen.

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


Hämtar suddradie radien som ska appliceras på kanterna, i enheten punkter.

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


Anger en valfri strängidentifierare som ett program kan använda för att identifiera den specifika formen.

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


Anger ett valfritt tal som ett program kan använda för att associera den specifika formen med en definierad formtyp.

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


Hämtar texten för denna form.

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


Hämtar inställningen för formens text.

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


Hämtar textinformationen i formen

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


Hämtar riktningen för textflödet för detta objekt.

Se [TextDirectionType](../../com.aspose.cells/textdirectiontype).

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


Returnerar ett TextEffectFormat‑objekt som innehåller text‑effektformaterings‑egenskaper för den angivna formen. Gäller Shape‑objekt som representerar WordArt.

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


Hämtar den horisontella justeringstypen för formens text.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Hämtar den horisontella översvämningstypen för formen som innehåller text.

Se [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Representerar textalternativen för formen.

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


Hämtar textorienteringstypen för formen.

Se [TextOrientationType](../../com.aspose.cells/textorientationtype).

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


Hämtar den förinställda textformstypen.

Se [AutoShapeType](../../com.aspose.cells/autoshapetype).

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


Hämtar den vertikala justeringstypen för formens text.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Hämtar den vertikala översvämningstypen för formen som innehåller text.

Se [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Hämtar 3D-formatet för formen.

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


Anger titeln (rubriken) för det aktuella formobjektet.

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


Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten pixlar.

**Remarks**

Om formen är i diagrammet, representerar den vertikala förskjutningen av formen från dess övre kant.

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


Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten centimeter.

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


Representerar den vertikala förskjutningen för formen från den översta kanten av föräldraformen, i enheten 1/4000 av föräldraformens höjd.

**Remarks**

Gäller endast när denna form är i en grupp eller ett diagram.

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


Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten tum.

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


Hämtar den vertikala förskjutningen för formen från kalkylbladets översta kant, i enheten pixlar.

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


Hämtar den automatiska formtypen.

Se [AutoShapeType](../../com.aspose.cells/autoshapetype).

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


Hämtar formens horisontella förskjutning från dess övre vänstra kolumn.

**Remarks**

Värdeintervallet är 0 till 1024.

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


Hämtar formens vertikala förskjutning från dess övre vänstra rad.

**Remarks**

Värdeintervallet är 0 till 256.

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


Representerar index för övre vänstra kolumnen.

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


Representerar det översta radindexet.

**Remarks**

Om formen är i en form eller i en grupp, kommer UpperLeftRow att ignoreras.

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


Representerar bredden på shape, i enheten pixlar.

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


Representerar bredden på shape, i enheten centimeter.

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


Representerar bredden på shape, i enheten 1/4000 av den överordnade shape.

**Remarks**

Gäller endast när denna form är i en grupp eller ett diagram.

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


Representerar bredden på shape, i enheten tum.

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


Representerar bredden på shape, i enheten punkt.

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


Hämtar breddskalan, i enhet procent av den ursprungliga bildens bredd. Om formen inte är en bild, returnerar WidthScale‑egenskapen endast 100;

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


Hämtar [Worksheet](../../com.aspose.cells/worksheet)-objektet som innehåller denna shape.

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


Hämtar den horisontella förskjutningen av shape från kalkylbladets vänstra kant, i enheten pixlar.

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


Hämtar den vertikala förskjutningen av shape från kalkylbladets övre kant, i enheten pixlar.

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


Returnerar positionen för en shape i z-ordningen.

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


Hämtar om linjekanten på shape är synlig.

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


Sant betyder att bildförhållandet för shape är låst.

**Remarks**

Endast för bilder och Ole‑objekt.

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


Indikerar om objektet är dekorativt.

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


Indikerar om shape endast innehåller en ekvation.

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


Indikerar om fyllningsformatet är synligt.

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


Hämtar om shape är horisontellt speglad.

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


Hämtar om shape är vertikalt speglad.

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


Indikerar om denna shape är en gruppshape.

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


Indikerar om objektet är synligt.

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


Indikerar om shape är grupperad.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


Sant betyder att bildförhållandet för shape är låst.

**Remarks**

Endast för bilder och Ole-objekt. OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Shape.IsAspectRatioLocked. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


True betyder att objektet inte kan ändras när bladet är skyddat. Observera att detta värde endast är meningsfullt om kalkylbladet eller objekten i kalkylbladet är skyddade.

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


Anger om objektet är utskrivbart. Om False kommer denna form inte att skrivas ut vid utskrift.

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


Om texten är rik text eller inte.

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


Returnerar om shape är densamma.

**Example**

```
         if (shape.isSameSetting(shape))
             System.out.println("Two objects the same.");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### isSmartArt() {#isSmartArt--}
```
public boolean isSmartArt()
```


Anger om formen är en smart art.

**Remarks**

Endast för ooxml-fil.

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


Hämtar den typ av textomslag för formen som innehåller text.

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


Anger om denna form är en word art.

**Remarks**

Endast för den äldre formen i xls-fil.

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


Flyttar formen till ett angivet område.

**Example**

```
         shape.moveToRange(12, 3, 13, 5);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| bottomRow | int | Nedre högra radindex |
| rightColumn | int | Nedre högra kolumnindex |

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


Ta bort ActiveX-kontrollen.

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


Tar bort hyperlänken för formen.

**Example**

```
         shape.removeHyperlink();
```

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Returnerar eller anger den beskrivande (alternativa) textsträngen för [Shape](../../com.aspose.cells/shape)-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setAnchorType(int value) {#setAnchorType-int-}
```
public void setAnchorType(int value)
```


Ställer in typen av formens ankareplatshållare.

Se [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setAspectRatioLocked(boolean value) {#setAspectRatioLocked-boolean-}
```
public void setAspectRatioLocked(boolean value)
```


Sant betyder att bildförhållandet för shape är låst.

**Remarks**

Endast för bilder och Ole‑objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoShapeType(int value) {#setAutoShapeType-int-}
```
public void setAutoShapeType(int value)
```


Ställer in autoformstypen.

Se [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Representerar bredden på formens vertikala förskjutning från dess nedre hörnrad, i enhet pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCreateId(UUID value) {#setCreateId-java.util.UUID-}
```
public void setCreateId(UUID value)
```


Ställer in skapande-ID för denna form.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.UUID |  |

### setDecorative(boolean value) {#setDecorative-boolean-}
```
public void setDecorative(boolean value)
```


Indikerar om objektet är dekorativt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFilled(boolean value) {#setFilled-boolean-}
```
public void setFilled(boolean value)
```


Indikerar om fyllningsformatet är synligt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFlippedHorizontally(boolean value) {#setFlippedHorizontally-boolean-}
```
public void setFlippedHorizontally(boolean value)
```


Ställer in om formen är horisontellt speglad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Ställer in om formen är vertikalt speglad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFont(Font value) {#setFont-com.aspose.cells.Font-}
```
public void setFont(Font value)
```


Representerar formens teckensnitt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Font](../../com.aspose.cells/font) |  |

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


Representerar höjden på formen, i enhet centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setHeightInShape(int value) {#setHeightInShape-int-}
```
public void setHeightInShape(int value)
```


Representerar den vertikala förskjutningen av formen från den översta kanten av föräldraformen, i enhet 1/4000 av föräldraformens höjd.

**Remarks**

Gäller endast när denna form är i en grupp eller ett diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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


Ställer in HTML-strängen som innehåller data och vissa format i den här textrutan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setInputRange(String value) {#setInputRange-java.lang.String-}
```
public void setInputRange(String value)
```


Ställer in kalkylbladsområdet som används för att fylla den angivna kombinationsrutan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setInputRange(String formula, boolean isR1C1, boolean isLocal) {#setInputRange-java.lang.String-boolean-boolean-}
```
public void setInputRange(String formula, boolean isR1C1, boolean isLocal)
```


Ställer in området som används för att fylla kontrollen.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Intervallet som används för att fylla kontrollen. |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |

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

### setLeftInShape(int value) {#setLeftInShape-int-}
```
public void setLeftInShape(int value)
```


Representerar den horisontella förskjutningen av formen från den vänstra kanten av föräldraformen, i enhet 1/4000 av föräldraformens bredd.

**Remarks**

Gäller endast när denna form är i en grupp eller ett diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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


Ställer in den horisontella förskjutningen av formen från kalkylbladets vänstra kant.

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

### setLinkedCell(String formula, boolean isR1C1, boolean isLocal) {#setLinkedCell-java.lang.String-boolean-boolean-}
```
public void setLinkedCell(String formula, boolean isR1C1, boolean isLocal)
```


Ställer in området som är länkat till kontrollens värde.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Intervallet som är länkat till kontrollens värde. |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


Sant betyder att bildförhållandet för shape är låst.

**Remarks**

Endast för bilder och Ole-objekt. OBS: Denna medlem är nu föråldrad. Använd istället egenskapen Shape.IsAspectRatioLocked. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True betyder att objektet inte kan ändras när bladet är skyddat. Observera att detta värde endast är meningsfullt om kalkylbladet eller objekten i kalkylbladet är skyddade.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLockedProperty(int type, boolean value) {#setLockedProperty-int-boolean-}
```
public void setLockedProperty(int type, boolean value)
```


Ställ in den låsta egenskapen.

**Example**

```
         shape.setLockedProperty(ShapeLockType.ADJUST_HANDLES, true);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). Den låsta typen. |
| värde | boolean | Värdet på egenskapen. |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Ställer in formens horisontella förskjutning från dess nedre högra kolumn.

**Remarks**

Värdeintervallet är 0 till 1024.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Ställer in formens vertikala förskjutning från dess nedre högra rad.

**Remarks**

Värdeintervallet är 0 till 256.

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

### setMacroName(String value) {#setMacroName-java.lang.String-}
```
public void setMacroName(String value)
```


Ställer in namnet på makrot.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in namnet på formen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Representerar hur ritobjektet är fäst vid cellerna under det. Egenskapen styr placeringen av ett objekt på ett kalkylblad.

Se [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Anger om objektet är utskrivbart. Om False kommer denna form inte att skrivas ut vid utskrift.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

### setSoftEdges(double value) {#setSoftEdges-double-}
```
public void setSoftEdges(double value)
```


Ställer in suddradien som ska tillämpas på kanterna, i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Ställer in texten för den här formen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Ställer in riktningen för textflödet för detta objekt.

Se [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Ställer in den horisontella justeringstypen för texten i formen.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Ställer in den horisontella översvämningstypen för texten i formen som innehåller text.

Se [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextOptions(TextOptions value) {#setTextOptions-com.aspose.cells.TextOptions-}
```
public void setTextOptions(TextOptions value)
```


Representerar textalternativen för formen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TextOptions](../../com.aspose.cells/textoptions) |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Ställer in orienteringstypen för texten i formen.

Se [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Ställer in den förinställda textformstypen.

Se [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Ställer in den vertikala justeringstypen för texten i formen.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Ställer in den vertikala översvämningstypen för texten i formen som innehåller text.

Se [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

### setTopInShape(int value) {#setTopInShape-int-}
```
public void setTopInShape(int value)
```


Representerar den vertikala förskjutningen för formen från den översta kanten av föräldraformen, i enheten 1/4000 av föräldraformens höjd.

**Remarks**

Gäller endast när denna form är i en grupp eller ett diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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


Ställer in den vertikala förskjutningen för formen från kalkylbladets övre kant, i enheten pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Ställer in formens horisontella förskjutning från dess övre vänstra kolumn.

**Remarks**

Värdeintervallet är 0 till 1024.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Ställer in formens vertikala förskjutning från dess övre vänstra rad.

**Remarks**

Värdeintervallet är 0 till 256.

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


Representerar det översta radindexet.

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

### setWidthInShape(int value) {#setWidthInShape-int-}
```
public void setWidthInShape(int value)
```


Representerar bredden på shape, i enheten 1/4000 av den överordnade shape.

**Remarks**

Gäller endast när denna form är i en grupp eller ett diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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


Ställer in den horisontella förskjutningen för formen från kalkylbladets vänstra kant, i enheten pixlar.

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

### toFrontOrBack(int orders) {#toFrontOrBack-int-}
```
public void toFrontOrBack(int orders)
```


Flyttar formen till framkant eller skickar formen till bakgrunden.

**Example**

```
         shape.toFrontOrBack(2);
         //or shape.ToFrontOrBack(-1);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| orders | int | Om den är mindre än noll placeras formen i bakgrunden. Om den är större än noll flyttas formen framåt. |

### toImage(OutputStream stream, ImageFormat imageFormat) {#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-}
```
public void toImage(OutputStream stream, ImageFormat imageFormat)
```


Skapar formens bild och sparar den till en ström i det angivna formatet.

**Remarks**

Följande format stöds: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Utdatastreamen. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | Formatet som bilden ska sparas i. |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Sparar formen till en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Sparar formen till en fil.

**Example**

```
         ImageOrPrintOptions op = new ImageOrPrintOptions();
         shape.toImage("exmaple.png", op);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
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


Uppdatera det valda värdet med värdet från den länkade cellen.

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

