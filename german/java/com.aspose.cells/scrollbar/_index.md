---
title: "Scrollleiste"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt ein Bildlaufleisten-Objekt dar."
type: docs
url: /de/java/com.aspose.cells/scrollbar/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Shape](../../com.aspose.cells/shape)
```
public class ScrollBar extends Shape
```

Stellt ein Bildlaufleisten-Objekt dar.

**Remarks**

Der Bildlaufwert muss zwischen 0 und 30000 liegen.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Fügt dem Shape einen Hyperlink hinzu. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Verschiebt das Bild in die obere rechte Ecke. |
| [calculateTextSize()](#calculateTextSize--) | Berechnet den Textbereich neu. |
| [characters(int startIndex, int length)](#characters-int-int-) | Gibt ein Characters‑Objekt zurück, das einen Zeichenbereich im Text darstellt. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fitToTextSize()](#fitToTextSize--) | Berechnet einen Textbereich neu, der geeignet ist, den gesamten Textinhalt anzuzeigen. |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Formatiert einige Zeichen mit der Schriftarteinstellung. |
| [getActiveXControl()](#getActiveXControl--) | Liefert das ActiveX‑Steuerelement. |
| [getActualBox()](#getActualBox--) | Ermittelt die tatsächliche Position und Größe des Shapes (nach Anwendung von Drehung, Spiegelung usw.). |
| [getActualLowerRightRow()](#getActualLowerRightRow--) | Ermittelt die tatsächliche untere Zeile. |
| [getAlternativeText()](#getAlternativeText--) | Gibt den beschreibenden (alternativen) Textstring des [Shape](../../com.aspose.cells/shape)-Objekts zurück oder setzt ihn. |
| [getAnchorType()](#getAnchorType--) | Liefert den Typ des Shape‑Anker‑Platzhalters. |
| [getAutoShapeType()](#getAutoShapeType--) | Ruft den Autoformtyp ab. |
| [getBottom()](#getBottom--) | Stellt die Breite des vertikalen Versatzes der Form von ihrer unteren Ecke in Pixeln dar. |
| [getCharacters()](#getCharacters--) | Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Text darstellen. |
| [getClass()](#getClass--) |  |
| [getConnectionPoints()](#getConnectionPoints--) | Ruft die Verbindungspunkte ab. |
| [getControlData()](#getControlData--) | Ruft die Daten des Steuerelements ab. |
| [getCreateId()](#getCreateId--) | Ruft die Erstellungs-ID für diese Form ab. |
| [getCurrentValue()](#getCurrentValue--) | Ermittelt den aktuellen Wert. |
| [getFill()](#getFill--) | Gibt ein [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) Objekt zurück, das Füllformatierungseigenschaften für die angegebene Form enthält. |
| [getFillFormat()](#getFillFormat--) | Gibt ein MsoFillFormat-Objekt zurück, das Füllformatierungseigenschaften für die angegebene Form enthält. |
| [getFont()](#getFont--) | Stellt die Schriftart der Form dar. |
| [getFormatPicture()](#getFormatPicture--) | Ruft die Optionen des Bildformats ab. |
| [getGeometry()](#getGeometry--) | Ruft die Geometrie ab. |
| [getGlow()](#getGlow--) | Stellt ein [GlowEffect](../../com.aspose.cells/gloweffect)-Objekt dar, das den Leuchteffekt für das Diagrammelement oder die Form angibt. |
| [getGroup()](#getGroup--) | Ruft die Gruppierungsform ab, die diese Form enthält. |
| [getHeight()](#getHeight--) | Stellt die Höhe der Form in Pixeln dar. |
| [getHeightCM()](#getHeightCM--) | Stellt die Höhe der Form in Zentimetern dar. |
| [getHeightInShape()](#getHeightInShape--) | Stellt den vertikalen Versatz der Form vom oberen Rand der übergeordneten Form in Einheiten von 1/4000 der Höhe der übergeordneten Form dar. |
| [getHeightInch()](#getHeightInch--) | Stellt die Höhe der Form in Zoll dar. |
| [getHeightPt()](#getHeightPt--) | Stellt die Höhe der Form in Punkt dar. |
| [getHeightScale()](#getHeightScale--) | Ruft die Höhenskalierung in Prozent der ursprünglichen Bildhöhe ab. |
| [getHtmlText()](#getHtmlText--) | Ruft die HTML-Zeichenfolge ab, die Daten und einige Formate in diesem Textfeld enthält. |
| [getHyperlink()](#getHyperlink--) | Ruft den Hyperlink der Form ab. |
| [getId()](#getId--) | Ruft den Bezeichner dieser Form ab. |
| [getIncrementalChange()](#getIncrementalChange--) | Ermittelt den Betrag, um den die Bildlaufleiste oder der Spinner bei einem Zeilen‑Scroll erhöht wird. |
| [getInputRange()](#getInputRange--) | Ruft den Arbeitsblattbereich ab, der zum Befüllen der angegebenen Kombinationsbox verwendet wird. |
| [getInputRange(boolean isR1C1, boolean isLocal)](#getInputRange-boolean-boolean-) | Ermittelt den Bereich, der zum Ausfüllen des Steuerelements verwendet wird. |
| [getLeft()](#getLeft--) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Pixeln. |
| [getLeftCM()](#getLeftCM--) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zentimetern. |
| [getLeftInShape()](#getLeftInShape--) | Stellt den horizontalen Versatz der Form vom linken Rand der übergeordneten Form dar, in Einheiten von 1/4000 der Breite der übergeordneten Form. |
| [getLeftInch()](#getLeftInch--) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zoll. |
| [getLeftToCorner()](#getLeftToCorner--) | Ermittelt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts. |
| [getLine()](#getLine--) | Ermittelt den Linienstil |
| [getLineFormat()](#getLineFormat--) | Gibt ein MsoLineFormat-Objekt zurück, das Linienformatierungseigenschaften für die angegebene Form enthält. |
| [getLinkedCell()](#getLinkedCell--) | Ermittelt den Arbeitsblattbereich, der mit dem Wert des Steuerelements verknüpft ist. |
| [getLinkedCell(boolean isR1C1, boolean isLocal)](#getLinkedCell-boolean-boolean-) | Ermittelt den Bereich, der mit dem Wert des Steuerelements verknüpft ist. |
| [getLockedProperty(int type)](#getLockedProperty-int-) | Ermittelt den Wert der gesperrten Eigenschaft. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Ermittelt den horizontalen Versatz der Form von ihrer unteren rechten Eckspalte. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Ermittelt den vertikalen Versatz der Form von ihrer unteren rechten Eckzeile. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Stellt den Spaltenindex der unteren rechten Ecke dar. |
| [getLowerRightRow()](#getLowerRightRow--) | Stellt den Zeilenindex der unteren rechten Ecke dar. |
| [getMacroName()](#getMacroName--) | Ermittelt den Namen des Makros. |
| [getMax()](#getMax--) | Ermittelt den Maximalwert eines Bildlaufleisten- oder Spinnerbereichs. |
| [getMin()](#getMin--) | Ermittelt den Minimalwert eines Bildlaufleisten- oder Spinnerbereichs. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Ermittelt den Zeichnungstyp. |
| [getName()](#getName--) | Ermittelt den Namen der Form. |
| [getPageChange()](#getPageChange--) | Ermittelt die Seitenänderung. |
| [getPaths()](#getPaths--) | Ermittelt die Pfade einer benutzerdefinierten geometrischen Form. |
| [getPlacement()](#getPlacement--) | Stellt die Art dar, wie das Zeichenobjekt an den darunterliegenden Zellen befestigt ist. |
| [getReflection()](#getReflection--) | Stellt ein [ReflectionEffect](../../com.aspose.cells/reflectioneffect)-Objekt dar, das den Reflexionseffekt für das Diagrammelement oder die Form angibt. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Gibt an, ob die Form relativ zur Originalbildgröße ist. |
| [getResultOfSmartArt()](#getResultOfSmartArt--) | Konvertieren von SmartArt in gruppierte Formen. |
| [getRichFormattings()](#getRichFormattings--) | Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Text darstellen. |
| [getRight()](#getRight--) | Stellt die Breite des horizontalen Versatzes der Form von ihrer unteren rechten Eckspalte dar, in Einheiten von Pixeln. |
| [getRotationAngle()](#getRotationAngle--) | Ermittelt die Drehung der Form. |
| [getShadow()](#getShadow--) | Gibt an, ob die Form 3‑D‑Schattierung hat. |
| [getShadowEffect()](#getShadowEffect--) | Stellt ein [ShadowEffect](../../com.aspose.cells/shadoweffect)-Objekt dar, das den Schatteneffekt für das Diagrammelement oder die Form angibt. |
| [getSoftEdges()](#getSoftEdges--) | Ermittelt den Unschärferadius, der auf die Kanten angewendet wird, in Punkten. |
| [getSpid()](#getSpid--) | Gibt einen optionalen Zeichenkettenbezeichner an, den eine Anwendung zur Identifizierung der jeweiligen Form verwenden kann. |
| [getSpt()](#getSpt--) | Gibt eine optionale Zahl an, die eine Anwendung verwenden kann, um die jeweilige Form einem definierten Formtyp zuzuordnen. |
| [getText()](#getText--) | Ermittelt den Text dieser Form. |
| [getTextBody()](#getTextBody--) | Ermittelt die Einstellung des Textes der Form. |
| [getTextBoxOptions()](#getTextBoxOptions--) | Ermittelt die Textinformationen in der Form |
| [getTextDirection()](#getTextDirection--) | Ermittelt die Richtung des Textflusses für dieses Objekt. |
| [getTextEffect()](#getTextEffect--) | Gibt ein TextEffectFormat-Objekt zurück, das Text-Effekt-Formatierungseigenschaften für die angegebene Form enthält. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Ermittelt den horizontalen Ausrichtungstyp des Textes der Form. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Ermittelt den horizontalen Überlauftyp des Textes der Form, die Text enthält. |
| [getTextOptions()](#getTextOptions--) | Stellt die Textoptionen der Form dar. |
| [getTextOrientationType()](#getTextOrientationType--) | Ermittelt den Orientierungstyp des Textes der Form. |
| [getTextShapeType()](#getTextShapeType--) | Ermittelt den voreingestellten Textformtyp. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Ermittelt den vertikalen Ausrichtungstyp des Textes der Form. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Ermittelt den vertikalen Überlauftyp des Textes der Form, die Text enthält. |
| [getThreeDFormat()](#getThreeDFormat--) | Ermittelt das 3D-Format der Form. |
| [getTitle()](#getTitle--) | Gibt den Titel (Beschriftung) des aktuellen Formobjekts an. |
| [getTop()](#getTop--) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Pixeln dar. |
| [getTopCM()](#getTopCM--) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zentimetern dar. |
| [getTopInShape()](#getTopInShape--) | Stellt den vertikalen Versatz der Form vom oberen Rand der übergeordneten Form in Einheiten von 1/4000 der Höhe der übergeordneten Form dar. |
| [getTopInch()](#getTopInch--) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zoll dar. |
| [getTopToCorner()](#getTopToCorner--) | Ermittelt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts in Pixeln. |
| [getType()](#getType--) | Ruft den Autoformtyp ab. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Ermittelt den horizontalen Versatz der Form von ihrer oberen linken Eckspalte. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Ermittelt den vertikalen Versatz der Form von ihrer oberen linken Eckzeile. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Stellt den Spaltenindex der oberen linken Ecke dar. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Stellt den Index der obersten Zeile dar. |
| [getWidth()](#getWidth--) | Stellt die Breite der Form dar, in Einheit Pixel. |
| [getWidthCM()](#getWidthCM--) | Stellt die Breite der Form dar, in Einheit Zentimeter. |
| [getWidthInShape()](#getWidthInShape--) | Stellt die Breite der Form dar, in Einheit 1/4000 der übergeordneten Form. |
| [getWidthInch()](#getWidthInch--) | Stellt die Breite der Form dar, in Einheit Zoll. |
| [getWidthPt()](#getWidthPt--) | Stellt die Breite der Form dar, in Einheit Punkt. |
| [getWidthScale()](#getWidthScale--) | Ermittelt die Breiten­skalierung, in Prozent der ursprünglichen Bildbreite. |
| [getWorksheet()](#getWorksheet--) | Ermittelt das [Worksheet](../../com.aspose.cells/worksheet)-Objekt, das diese Form enthält. |
| [getX()](#getX--) | Ermittelt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts, in Einheit Pixel. |
| [getY()](#getY--) | Ermittelt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts, in Einheit Pixel. |
| [getZOrderPosition()](#getZOrderPosition--) | Gibt die Position einer Form in der Z-Reihenfolge zurück. |
| [hasLine()](#hasLine--) | Ermittelt, ob die Linienbegrenzung der Form sichtbar ist. |
| [hashCode()](#hashCode--) |  |
| [isAspectRatioLocked()](#isAspectRatioLocked--) | True bedeutet, dass das Seitenverhältnis der Form gesperrt ist. |
| [isDecorative()](#isDecorative--) | Gibt an, ob das Objekt dekorativ ist. |
| [isEquation()](#isEquation--) | Gibt an, ob die Form nur eine Gleichung enthält. |
| [isFilled()](#isFilled--) | Gibt an, ob das Füllformat sichtbar ist. |
| [isFlippedHorizontally()](#isFlippedHorizontally--) | Ermittelt, ob die Form horizontal gespiegelt ist . |
| [isFlippedVertically()](#isFlippedVertically--) | Ermittelt, ob die Form vertikal gespiegelt ist . |
| [isGroup()](#isGroup--) | Gibt an, ob diese Form eine Gruppierung ist. |
| [isHidden()](#isHidden--) | Gibt an, ob das Objekt sichtbar ist. |
| [isHorizontal()](#isHorizontal--) | Gibt an, ob es sich um eine horizontale Bildlaufleiste handelt. |
| [isInGroup()](#isInGroup--) | Gibt an, ob die Form gruppiert ist. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True bedeutet, dass das Seitenverhältnis der Form gesperrt ist. |
| [isLocked()](#isLocked--) | True bedeutet, dass das Objekt nicht geändert werden kann, wenn das Blatt geschützt ist. |
| [isPrintable()](#isPrintable--) | Gibt an, ob das Objekt druckbar ist. |
| [isRichText()](#isRichText--) | Ob der Text Rich Text ist oder nicht. |
| [isSameSetting(Object obj)](#isSameSetting-java.lang.Object-) | Gibt zurück, ob die Form identisch ist. |
| [isSmartArt()](#isSmartArt--) | Gibt an, ob die Form ein SmartArt ist. |
| [isTextWrapped()](#isTextWrapped--) | Ermittelt den Textumbruchtyp der Form, die Text enthält. |
| [isWordArt()](#isWordArt--) | Gibt an, ob diese Form ein WordArt ist. |
| [moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)](#moveToRange-int-int-int-int-) | Verschiebt die Form in einen angegebenen Bereich. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeActiveXControl()](#removeActiveXControl--) | Entfernt das ActiveX-Steuerelement. |
| [removeHyperlink()](#removeHyperlink--) | Entfernt den Hyperlink der Form. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Gibt den beschreibenden (alternativen) Textstring des [Shape](../../com.aspose.cells/shape)-Objekts zurück oder setzt ihn. |
| [setAnchorType(int value)](#setAnchorType-int-) | Legt den Typ des Ankerplatzhalters der Form fest. |
| [setAspectRatioLocked(boolean value)](#setAspectRatioLocked-boolean-) | True bedeutet, dass das Seitenverhältnis der Form gesperrt ist. |
| [setAutoShapeType(int value)](#setAutoShapeType-int-) | Legt den Typ der AutoForm fest. |
| [setBottom(int value)](#setBottom-int-) | Stellt die Breite des vertikalen Versatzes der Form von ihrer unteren Ecke in Pixeln dar. |
| [setCreateId(UUID value)](#setCreateId-java.util.UUID-) | Setzt die Erstellungs-ID für diese Form. |
| [setCurrentValue(int value)](#setCurrentValue-int-) | Legt den aktuellen Wert fest. |
| [setDecorative(boolean value)](#setDecorative-boolean-) | Gibt an, ob das Objekt dekorativ ist. |
| [setFilled(boolean value)](#setFilled-boolean-) | Gibt an, ob das Füllformat sichtbar ist. |
| [setFlippedHorizontally(boolean value)](#setFlippedHorizontally-boolean-) | Legt fest, ob die Form horizontal gespiegelt ist. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Legt fest, ob die Form vertikal gespiegelt ist. |
| [setFont(Font value)](#setFont-com.aspose.cells.Font-) | Stellt die Schriftart der Form dar. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Legt fest, ob die Linienbegrenzung der Form sichtbar ist. |
| [setHeight(int value)](#setHeight-int-) | Stellt die Höhe der Form in Pixeln dar. |
| [setHeightCM(double value)](#setHeightCM-double-) | Stellt die Höhe der Form in Zentimetern dar. |
| [setHeightInShape(int value)](#setHeightInShape-int-) | Stellt den vertikalen Versatz der Form vom oberen Rand der übergeordneten Form in Einheiten von 1/4000 der Höhe der übergeordneten Form dar. |
| [setHeightInch(double value)](#setHeightInch-double-) | Stellt die Höhe der Form in Zoll dar. |
| [setHeightPt(double value)](#setHeightPt-double-) | Stellt die Höhe der Form in Punkt dar. |
| [setHeightScale(int value)](#setHeightScale-int-) | Legt die Höhenskala fest, in Prozent der ursprünglichen Bildhöhe. |
| [setHidden(boolean value)](#setHidden-boolean-) | Gibt an, ob das Objekt sichtbar ist. |
| [setHorizontal(boolean value)](#setHorizontal-boolean-) | Gibt an, ob es sich um eine horizontale Bildlaufleiste handelt. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Legt die HTML-Zeichenfolge fest, die Daten und einige Formate in diesem Textfeld enthält. |
| [setIncrementalChange(int value)](#setIncrementalChange-int-) | Legt den Betrag fest, um den die Bildlaufleiste oder der Spinner bei einem Zeilen‑Scroll erhöht wird. |
| [setInputRange(String value)](#setInputRange-java.lang.String-) | Legt den Arbeitsblattbereich fest, der zum Befüllen der angegebenen Kombinationsbox verwendet wird. |
| [setInputRange(String formula, boolean isR1C1, boolean isLocal)](#setInputRange-java.lang.String-boolean-boolean-) | Legt den Bereich fest, der zum Befüllen des Steuerelements verwendet wird. |
| [setLeft(int value)](#setLeft-int-) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Pixeln. |
| [setLeftCM(double value)](#setLeftCM-double-) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zentimetern. |
| [setLeftInShape(int value)](#setLeftInShape-int-) | Stellt den horizontalen Versatz der Form vom linken Rand der übergeordneten Form dar, in Einheiten von 1/4000 der Breite der übergeordneten Form. |
| [setLeftInch(double value)](#setLeftInch-double-) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zoll. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Legt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts fest. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Legt den Arbeitsblattbereich fest, der mit dem Wert des Steuerelements verknüpft ist. |
| [setLinkedCell(String formula, boolean isR1C1, boolean isLocal)](#setLinkedCell-java.lang.String-boolean-boolean-) | Legt den Bereich fest, der mit dem Wert des Steuerelements verknüpft ist. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True bedeutet, dass das Seitenverhältnis der Form gesperrt ist. |
| [setLocked(boolean value)](#setLocked-boolean-) | True bedeutet, dass das Objekt nicht geändert werden kann, wenn das Blatt geschützt ist. |
| [setLockedProperty(int type, boolean value)](#setLockedProperty-int-boolean-) | Setzt die gesperrte Eigenschaft. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Legt den horizontalen Versatz der Form von ihrer unteren rechten Eckspalte fest. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Legt den vertikalen Versatz der Form von ihrer unteren rechten Eckzeile fest. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Stellt den Spaltenindex der unteren rechten Ecke dar. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Stellt den Zeilenindex der unteren rechten Ecke dar. |
| [setMacroName(String value)](#setMacroName-java.lang.String-) | Legt den Namen des Makros fest. |
| [setMax(int value)](#setMax-int-) | Legt den Maximalwert eines Bildlaufleisten- oder Spinnerbereichs fest. |
| [setMin(int value)](#setMin-int-) | Legt den Minimalwert eines Bildlaufleisten- oder Spinnerbereichs fest. |
| [setName(String value)](#setName-java.lang.String-) | Legt den Namen der Form fest. |
| [setPageChange(int value)](#setPageChange-int-) | Legt die Seitenänderung fest. |
| [setPlacement(int value)](#setPlacement-int-) | Stellt die Art dar, wie das Zeichenobjekt an den darunterliegenden Zellen befestigt ist. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Gibt an, ob das Objekt druckbar ist. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Gibt an, ob die Form relativ zur Originalbildgröße ist. |
| [setRight(int value)](#setRight-int-) | Stellt die Breite des horizontalen Versatzes der Form von ihrer unteren rechten Eckspalte dar, in Einheiten von Pixeln. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Legt die Drehung der Form fest. |
| [setShadow(boolean value)](#setShadow-boolean-) | Gibt an, ob die Form 3‑D‑Schattierung hat. |
| [setSoftEdges(double value)](#setSoftEdges-double-) | Legt den Radius der Unschärfe fest, der auf die Kanten angewendet wird, in Einheit von Punkten. |
| [setText(String value)](#setText-java.lang.String-) | Legt den Text dieser Form fest. |
| [setTextDirection(int value)](#setTextDirection-int-) | Legt die Richtung des Textflusses für dieses Objekt fest. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Legt den Typ der horizontalen Textausrichtung der Form fest. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Legt den Typ des horizontalen Textüberlaufs der Form fest, die Text enthält. |
| [setTextOptions(TextOptions value)](#setTextOptions-com.aspose.cells.TextOptions-) | Stellt die Textoptionen der Form dar. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Legt den Typ der Textorientierung der Form fest. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Legt den voreingestellten Textformtyp fest. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Legt den Typ der vertikalen Textausrichtung der Form fest. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Legt den Typ des vertikalen Textüberlaufs der Form fest, die Text enthält. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Legt den Typ des umgebrochenen Textes der Form fest, die Text enthält. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Gibt den Titel (Beschriftung) des aktuellen Formobjekts an. |
| [setTop(int value)](#setTop-int-) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Pixeln dar. |
| [setTopCM(double value)](#setTopCM-double-) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zentimetern dar. |
| [setTopInShape(int value)](#setTopInShape-int-) | Stellt den vertikalen Versatz der Form vom oberen Rand der übergeordneten Form in Einheiten von 1/4000 der Höhe der übergeordneten Form dar. |
| [setTopInch(double value)](#setTopInch-double-) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zoll dar. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Legt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts fest, in Einheit von Pixeln. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Legt den horizontalen Versatz der Form von ihrer oberen linken Spalte fest. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Legt den vertikalen Versatz der Form von ihrer oberen linken Zeile fest. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Stellt den Spaltenindex der oberen linken Ecke dar. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Stellt den Index der obersten Zeile dar. |
| [setWidth(int value)](#setWidth-int-) | Stellt die Breite der Form dar, in Einheit Pixel. |
| [setWidthCM(double value)](#setWidthCM-double-) | Stellt die Breite der Form dar, in Einheit Zentimeter. |
| [setWidthInShape(int value)](#setWidthInShape-int-) | Stellt die Breite der Form dar, in Einheit 1/4000 der übergeordneten Form. |
| [setWidthInch(double value)](#setWidthInch-double-) | Stellt die Breite der Form dar, in Einheit Zoll. |
| [setWidthPt(double value)](#setWidthPt-double-) | Stellt die Breite der Form dar, in Einheit Punkt. |
| [setWidthScale(int value)](#setWidthScale-int-) | Legt die Breiten-Skalierung fest, in Prozent der ursprünglichen Bildbreite. |
| [setX(int value)](#setX-int-) | Legt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts fest, in Einheit von Pixeln. |
| [setY(int value)](#setY-int-) | Legt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts fest, in Einheit von Pixeln. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Gibt die Position einer Form in der Z-Reihenfolge zurück. |
| [toFrontOrBack(int orders)](#toFrontOrBack-int-) | Bringt die Form nach vorne oder sendet die Form nach hinten. |
| [toImage(OutputStream stream, ImageFormat imageFormat)](#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-) | Erstellt das Formbild und speichert es in einen Stream im angegebenen Format. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Speichert die Form in einen Stream. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Speichert die Form in einer Datei. |
| [toString()](#toString--) |  |
| [updateSelectedValue()](#updateSelectedValue--) | Aktualisiert den ausgewählten Wert anhand des Werts der verknüpften Zelle. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public Hyperlink addHyperlink(String address)
```


Fügt dem Shape einen Hyperlink hinzu.

**Example**

```
         Hyperlink hyperlink = shape.addHyperlink("https://www.aspose.com/");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Adresse | java.lang.String | Adresse des Hyperlinks. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - Returns the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Verschiebt das Bild in die obere rechte Ecke.

**Example**

```
         shape.alignTopRightCorner(2, 5);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | der Zeilenindex. |
| rightColumn | int | der Spaltenindex. |

### calculateTextSize() {#calculateTextSize--}
```
public int[] calculateTextSize()
```


Berechnet den Textbereich neu.

**Example**

```
         //The size of the text area is:w=size[0],h=size[1]
         int[] size = shape.calculateTextSize();
```

**Returns:**
int[] - Größe des Textes in einem Array (Breite und Höhe).
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Gibt ein Characters‑Objekt zurück, das einen Zeichenbereich im Text darstellt.

**Remarks**

Diese Methode funktioniert nur bei Formen mit Titel.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Der Index des Beginns des Zeichens. |
| length | int | Die Anzahl der Zeichen. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### fitToTextSize() {#fitToTextSize--}
```
public void fitToTextSize()
```


Berechnet einen Textbereich neu, der geeignet ist, den gesamten Textinhalt anzuzeigen.

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


Formatiert einige Zeichen mit der Schriftarteinstellung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Der Startindex. |
| length | int | Die Länge. |
| font | [Font](../../com.aspose.cells/font) | Die Schriftarteinstellung. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Das Flag der Schriftarteinstellung. |

### getActiveXControl() {#getActiveXControl--}
```
public ActiveXControl getActiveXControl()
```


Liefert das ActiveX‑Steuerelement.

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


Ermittelt die tatsächliche Position und Größe des Shapes (nach Anwendung von Drehung, Spiegelung usw.).

**Remarks**

Hinweis: Die Schnittstelle ist nicht vollständig funktionsfähig, insbesondere die Positionsinformationen sind nicht korrekt. Es wird empfohlen, diese Schnittstelle nicht zu verwenden, bis die Funktion fertiggestellt ist.

**Example**

```
         float[] box = shape.getActualBox();
         System.out.println("x = " + box[0]);
         System.out.println("y = " + box[1]);
         System.out.println("w = " + box[2]);
         System.out.println("h = " + box[3]);
```

**Returns:**
float[] - Gibt die Position und Größe in der Reihenfolge x, y, w, h zurück.
### getActualLowerRightRow() {#getActualLowerRightRow--}
```
public int getActualLowerRightRow()
```


Ermittelt die tatsächliche untere Zeile.

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


Gibt den beschreibenden (alternativen) Textstring des [Shape](../../com.aspose.cells/shape)-Objekts zurück oder setzt ihn.

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


Liefert den Typ des Shape‑Anker‑Platzhalters.

Siehe [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

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


Ruft den Autoformtyp ab.

Siehe [AutoShapeType](../../com.aspose.cells/autoshapetype).

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


Stellt die Breite des vertikalen Versatzes der Form von ihrer unteren Ecke in Pixeln dar.

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


Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Text darstellen.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode Shape.GetRichFormattings(). Diese Methode wird 12 Monate später, seit November 2023, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sind.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Returns:**
java.util.ArrayList - Alle Zeichenobjekte
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


Ruft die Verbindungspunkte ab.

**Example**

```
         float[][] points = shape.getConnectionPoints();
```

**Returns:**
float[][] - [X,Y]-Paare des Verbindungspunkts. Jeder Eintrag ist ein float[2]-Array, wobei [0] x und [1] y darstellt.
### getControlData() {#getControlData--}
```
public byte[] getControlData()
```


Ruft die Daten des Steuerelements ab.

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


Ruft die Erstellungs-ID für diese Form ab.

**Example**

```
         System.out.println(shape.getCreateId());
         java.util.UUID g = java.util.UUID.randomUUID();
         shape.setCreateId(g);
         System.out.println(shape.getCreateId());
```

**Returns:**
java.util.UUID
### getCurrentValue() {#getCurrentValue--}
```
public int getCurrentValue()
```


Ermittelt den aktuellen Wert.

**Returns:**
int
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Gibt ein [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) Objekt zurück, das Füllformatierungseigenschaften für die angegebene Form enthält.

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


Gibt ein MsoFillFormat-Objekt zurück, das Füllformatierungseigenschaften für die angegebene Form enthält.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft Shape.Fill. Diese Eigenschaft wird 12 Monate später, seit Juli 2016, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sind.

**Returns:**
[MsoFillFormat](../../com.aspose.cells/msofillformat)
### getFont() {#getFont--}
```
public Font getFont()
```


Stellt die Schriftart der Form dar.

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


Ruft die Optionen des Bildformats ab.

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


Ruft die Geometrie ab.

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


Stellt ein [GlowEffect](../../com.aspose.cells/gloweffect)-Objekt dar, das den Leuchteffekt für das Diagrammelement oder die Form angibt.

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


Ruft die Gruppierungsform ab, die diese Form enthält.

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


Stellt die Höhe der Form in Pixeln dar.

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


Stellt die Höhe der Form in Zentimetern dar.

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


Stellt den vertikalen Versatz der Form vom oberen Rand der übergeordneten Form in Einheiten von 1/4000 der Höhe der übergeordneten Form dar.

**Remarks**

Gilt nur, wenn diese Form in einer Gruppe oder einem Diagramm ist.

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


Stellt die Höhe der Form in Zoll dar.

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


Stellt die Höhe der Form in Punkt dar.

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


Ermittelt die Höhenskala, in Prozent der ursprünglichen Bildhöhe. Wenn das Shape kein Bild ist, gibt die HeightScale property nur 100 zurück;

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


Ruft die HTML-Zeichenfolge ab, die Daten und einige Formate in diesem Textfeld enthält.

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


Ruft den Hyperlink der Form ab.

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


Ruft den Bezeichner dieser Form ab.

**Example**

```
         int id = shape.getId();
```

**Returns:**
int
### getIncrementalChange() {#getIncrementalChange--}
```
public int getIncrementalChange()
```


Ermittelt den Betrag, um den die Bildlaufleiste oder der Spinner bei einem Zeilen‑Scroll erhöht wird.

**Returns:**
int
### getInputRange() {#getInputRange--}
```
public String getInputRange()
```


Ruft den Arbeitsblattbereich ab, der zum Befüllen der angegebenen Kombinationsbox verwendet wird.

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


Ermittelt den Bereich, der zum Ausfüllen des Steuerelements verwendet wird.

**Example**

```
         String range = shape.getInputRange(false, true);
         //If successful, a value like "$A$1:$A$3" will be returned
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |

**Returns:**
java.lang.String - Der Bereich, der zum Befüllen des Steuerelements verwendet wird.
### getLeft() {#getLeft--}
```
public int getLeft()
```


Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Pixeln.

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


Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zentimetern.

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


Stellt den horizontalen Versatz der Form vom linken Rand der übergeordneten Form dar, in Einheiten von 1/4000 der Breite der übergeordneten Form.

**Remarks**

Gilt nur, wenn diese Form in einer Gruppe oder einem Diagramm ist.

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


Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Zoll.

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


Ermittelt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts.

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


Ermittelt den Linienstil

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


Gibt ein MsoLineFormat-Objekt zurück, das Linienformatierungseigenschaften für die angegebene Form enthält.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Shape.Line property. Diese Property wird 12 Monate später, seit Juli 2016, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
[MsoLineFormat](../../com.aspose.cells/msolineformat)
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Ermittelt den Arbeitsblattbereich, der mit dem Wert des Steuerelements verknüpft ist.

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


Ermittelt den Bereich, der mit dem Wert des Steuerelements verknüpft ist.

**Example**

```
         //You may get results like '$A$1'
         String link = shape.getLinkedCell(false, false);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |

**Returns:**
java.lang.String - Der Bereich, der mit dem Wert des Steuerelements verknüpft ist.
### getLockedProperty(int type) {#getLockedProperty-int-}
```
public boolean getLockedProperty(int type)
```


Ermittelt den Wert der gesperrten Eigenschaft.

**Example**

```
         int noAdjustHandles = 0;
         if (shape.getLockedProperty(ShapeLockType.ADJUST_HANDLES))
             noAdjustHandles = 1;
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). Der Typ der shape locked property. |

**Returns:**
boolean - Gibt den Wert der locked property zurück.
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Ermittelt den horizontalen Versatz der Form von ihrer unteren rechten Eckspalte.

**Remarks**

Der Wertebereich liegt zwischen 0 und 1024.

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


Ermittelt den vertikalen Versatz der Form von ihrer unteren rechten Eckzeile.

**Remarks**

Der Wertebereich liegt zwischen 0 und 256.

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


Stellt den Spaltenindex der unteren rechten Ecke dar.

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


Stellt den Zeilenindex der unteren rechten Ecke dar.

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


Ermittelt den Namen des Makros.

**Example**

```
         //Sets the name of macro.
         shape.setMacroName("DoWork()");
```

**Returns:**
java.lang.String
### getMax() {#getMax--}
```
public int getMax()
```


Ermittelt den Maximalwert eines Bildlaufleisten- oder Spinnerbereichs.

**Returns:**
int
### getMin() {#getMin--}
```
public int getMin()
```


Ermittelt den Minimalwert eines Bildlaufleisten- oder Spinnerbereichs.

**Returns:**
int
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


Ermittelt den Zeichnungstyp.

Siehe [MsoDrawingType](../../com.aspose.cells/msodrawingtype).

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


Ermittelt den Namen der Form.

**Example**

```
         shape.setName("shape1");
```

**Returns:**
java.lang.String
### getPageChange() {#getPageChange--}
```
public int getPageChange()
```


Ermittelt die Seitenänderung.

**Returns:**
int
### getPaths() {#getPaths--}
```
public ShapePathCollection getPaths()
```


Ermittelt die Pfade einer benutzerdefinierten geometrischen Form.

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


Stellt dar, wie das Zeichenobjekt an den darunter liegenden Zellen befestigt ist. Die property steuert die Platzierung eines Objekts auf einem Arbeitsblatt.

Siehe [PlacementType](../../com.aspose.cells/placementtype).

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


Stellt ein [ReflectionEffect](../../com.aspose.cells/reflectioneffect)-Objekt dar, das den Reflexionseffekt für das Diagrammelement oder die Form angibt.

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


Gibt an, ob die Form relativ zur Originalbildgröße ist.

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


Konvertieren von SmartArt in gruppierte Formen.

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


Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Text darstellen.

**Example**

```
         FontSetting[] list = shape.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Alle Characters objects
### getRight() {#getRight--}
```
public int getRight()
```


Stellt die Breite des horizontalen Versatzes der Form von ihrer unteren rechten Eckspalte dar, in Einheiten von Pixeln.

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


Ermittelt die Drehung der Form.

**Example**

```
         //Gets rotation angle of the shape.
         double angle = shape.getRotationAngle() ;
 
         //Gets rotation angle of the shape.
          shape.setRotationAngle(60);
```

**Returns:**
double
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Gibt an, ob die Form 3‑D‑Schattierung hat.

**Returns:**
boolean
### getShadowEffect() {#getShadowEffect--}
```
public ShadowEffect getShadowEffect()
```


Stellt ein [ShadowEffect](../../com.aspose.cells/shadoweffect)-Objekt dar, das den Schatteneffekt für das Diagrammelement oder die Form angibt.

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


Ermittelt den Unschärferadius, der auf die Kanten angewendet wird, in Punkten.

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


Gibt einen optionalen Zeichenkettenbezeichner an, den eine Anwendung zur Identifizierung der jeweiligen Form verwenden kann.

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


Gibt eine optionale Zahl an, die eine Anwendung verwenden kann, um die jeweilige Form einem definierten Formtyp zuzuordnen.

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


Ermittelt den Text dieser Form.

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


Ermittelt die Einstellung des Textes der Form.

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


Ermittelt die Textinformationen in der Form

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


Ermittelt die Richtung des Textflusses für dieses Objekt.

Siehe [TextDirectionType](../../com.aspose.cells/textdirectiontype).

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


Gibt ein TextEffectFormat-Objekt zurück, das Text-Effekt-Formatierungseigenschaften für das angegebene Shape enthält. Gilt für Shape-Objekte, die WordArt darstellen.

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


Ermittelt den horizontalen Ausrichtungstyp des Textes der Form.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Ermittelt den horizontalen Überlauftyp des Textes der Form, die Text enthält.

Siehe [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Stellt die Textoptionen der Form dar.

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


Ermittelt den Orientierungstyp des Textes der Form.

Siehe [TextOrientationType](../../com.aspose.cells/textorientationtype).

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


Ermittelt den voreingestellten Textformtyp.

Siehe [AutoShapeType](../../com.aspose.cells/autoshapetype).

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


Ermittelt den vertikalen Ausrichtungstyp des Textes der Form.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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


Ermittelt den vertikalen Überlauftyp des Textes der Form, die Text enthält.

Siehe [TextOverflowType](../../com.aspose.cells/textoverflowtype).

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


Ermittelt das 3D-Format der Form.

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


Gibt den Titel (Beschriftung) des aktuellen Formobjekts an.

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


Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Pixeln dar.

**Remarks**

Wenn das Shape im Diagramm ist, stellt es den vertikalen Versatz des Shapes von seiner oberen Kante dar.

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


Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zentimetern dar.

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


Stellt den vertikalen Versatz der Form vom oberen Rand der übergeordneten Form in Einheiten von 1/4000 der Höhe der übergeordneten Form dar.

**Remarks**

Gilt nur, wenn diese Form in einer Gruppe oder einem Diagramm ist.

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


Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Zoll dar.

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


Ermittelt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts in Pixeln.

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


Ruft den Autoformtyp ab.

Siehe [AutoShapeType](../../com.aspose.cells/autoshapetype).

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


Ermittelt den horizontalen Versatz der Form von ihrer oberen linken Eckspalte.

**Remarks**

Der Wertebereich liegt zwischen 0 und 1024.

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


Ermittelt den vertikalen Versatz der Form von ihrer oberen linken Eckzeile.

**Remarks**

Der Wertebereich liegt zwischen 0 und 256.

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


Stellt den Spaltenindex der oberen linken Ecke dar.

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


Stellt den Index der obersten Zeile dar.

**Remarks**

Wenn das Shape im Shape oder in der Gruppe ist, wird UpperLeftRow ignoriert.

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


Stellt die Breite der Form dar, in Einheit Pixel.

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


Stellt die Breite der Form dar, in Einheit Zentimeter.

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


Stellt die Breite der Form dar, in Einheit 1/4000 der übergeordneten Form.

**Remarks**

Gilt nur, wenn diese Form in einer Gruppe oder einem Diagramm ist.

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


Stellt die Breite der Form dar, in Einheit Zoll.

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


Stellt die Breite der Form dar, in Einheit Punkt.

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


Ermittelt die Breiten­skala, in Prozent der ursprünglichen Bildbreite. Wenn das Shape kein Bild ist, gibt die WidthScale property nur 100 zurück;

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


Ermittelt das [Worksheet](../../com.aspose.cells/worksheet)-Objekt, das diese Form enthält.

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


Ermittelt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts, in Einheit Pixel.

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


Ermittelt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts, in Einheit Pixel.

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


Gibt die Position einer Form in der Z-Reihenfolge zurück.

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


Ermittelt, ob die Linienbegrenzung der Form sichtbar ist.

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


True bedeutet, dass das Seitenverhältnis der Form gesperrt ist.

**Remarks**

Nur für Bilder und Ole-Objects.

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


Gibt an, ob das Objekt dekorativ ist.

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


Gibt an, ob die Form nur eine Gleichung enthält.

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


Gibt an, ob das Füllformat sichtbar ist.

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


Ermittelt, ob die Form horizontal gespiegelt ist .

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


Ermittelt, ob die Form vertikal gespiegelt ist .

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


Gibt an, ob diese Form eine Gruppierung ist.

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


Gibt an, ob das Objekt sichtbar ist.

**Example**

```
         shape.setHidden(false);
```

**Returns:**
boolean
### isHorizontal() {#isHorizontal--}
```
public boolean isHorizontal()
```


Gibt an, ob es sich um eine horizontale Bildlaufleiste handelt.

**Returns:**
boolean
### isInGroup() {#isInGroup--}
```
public boolean isInGroup()
```


Gibt an, ob die Form gruppiert ist.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True bedeutet, dass das Seitenverhältnis der Form gesperrt ist.

**Remarks**

Nur für Bilder und Ole Objects. HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft Shape.IsAspectRatioLocked. Diese Eigenschaft wird 12 Monate später ab Juli 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

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


True bedeutet, dass das Objekt nicht geändert werden kann, wenn das Blatt geschützt ist. Beachten Sie, dass dieser Wert nur sinnvoll ist, wenn das Arbeitsblatt oder die Objekte im Arbeitsblatt geschützt sind.

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


Gibt an, ob das Objekt druckbar ist. Wenn False, wird diese Form beim Drucken nicht ausgedruckt.

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


Ob der Text Rich Text ist oder nicht.

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


Gibt zurück, ob die Form identisch ist.

**Example**

```
         if (shape.isSameSetting(shape))
             System.out.println("Two objects the same.");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### isSmartArt() {#isSmartArt--}
```
public boolean isSmartArt()
```


Gibt an, ob die Form ein SmartArt ist.

**Remarks**

Nur für ooxml-Datei.

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


Ermittelt den Textumbruchtyp der Form, die Text enthält.

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


Gibt an, ob diese Form ein WordArt ist.

**Remarks**

Nur für die Legacy-Form der xls-Datei.

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


Verschiebt die Form in einen angegebenen Bereich.

**Example**

```
         shape.moveToRange(12, 3, 13, 5);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| leftColumn | int | Index der oberen linken Spalte. |
| bottomRow | int | Index der unteren rechten Zeile |
| rightColumn | int | Index der unteren rechten Spalte |

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


Entfernt das ActiveX-Steuerelement.

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


Entfernt den Hyperlink der Form.

**Example**

```
         shape.removeHyperlink();
```

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Gibt den beschreibenden (alternativen) Textstring des [Shape](../../com.aspose.cells/shape)-Objekts zurück oder setzt ihn.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setAnchorType(int value) {#setAnchorType-int-}
```
public void setAnchorType(int value)
```


Legt den Typ des Ankerplatzhalters der Form fest.

Siehe [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setAspectRatioLocked(boolean value) {#setAspectRatioLocked-boolean-}
```
public void setAspectRatioLocked(boolean value)
```


True bedeutet, dass das Seitenverhältnis der Form gesperrt ist.

**Remarks**

Nur für Bilder und Ole-Objects.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoShapeType(int value) {#setAutoShapeType-int-}
```
public void setAutoShapeType(int value)
```


Legt den Typ der AutoForm fest.

Siehe [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Stellt die Breite des vertikalen Versatzes der Form von ihrer unteren Ecke in Pixeln dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCreateId(UUID value) {#setCreateId-java.util.UUID-}
```
public void setCreateId(UUID value)
```


Setzt die Erstellungs-ID für diese Form.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.UUID |  |

### setCurrentValue(int value) {#setCurrentValue-int-}
```
public void setCurrentValue(int value)
```


Legt den aktuellen Wert fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDecorative(boolean value) {#setDecorative-boolean-}
```
public void setDecorative(boolean value)
```


Gibt an, ob das Objekt dekorativ ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFilled(boolean value) {#setFilled-boolean-}
```
public void setFilled(boolean value)
```


Gibt an, ob das Füllformat sichtbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFlippedHorizontally(boolean value) {#setFlippedHorizontally-boolean-}
```
public void setFlippedHorizontally(boolean value)
```


Legt fest, ob die Form horizontal gespiegelt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Legt fest, ob die Form vertikal gespiegelt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFont(Font value) {#setFont-com.aspose.cells.Font-}
```
public void setFont(Font value)
```


Stellt die Schriftart der Form dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Font](../../com.aspose.cells/font) |  |

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


Stellt die Höhe der Form in Zentimetern dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setHeightInShape(int value) {#setHeightInShape-int-}
```
public void setHeightInShape(int value)
```


Stellt den vertikalen Versatz der Form vom oberen Rand der übergeordneten Form in Einheiten von 1/4000 der Höhe der übergeordneten Form dar.

**Remarks**

Gilt nur, wenn diese Form in einer Gruppe oder einem Diagramm ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

### setHorizontal(boolean value) {#setHorizontal-boolean-}
```
public void setHorizontal(boolean value)
```


Gibt an, ob es sich um eine horizontale Bildlaufleiste handelt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


Legt die HTML-Zeichenfolge fest, die Daten und einige Formate in diesem Textfeld enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setIncrementalChange(int value) {#setIncrementalChange-int-}
```
public void setIncrementalChange(int value)
```


Legt den Betrag fest, um den die Bildlaufleiste oder der Spinner bei einem Zeilen‑Scroll erhöht wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setInputRange(String value) {#setInputRange-java.lang.String-}
```
public void setInputRange(String value)
```


Legt den Arbeitsblattbereich fest, der zum Befüllen der angegebenen Kombinationsbox verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setInputRange(String formula, boolean isR1C1, boolean isLocal) {#setInputRange-java.lang.String-boolean-boolean-}
```
public void setInputRange(String formula, boolean isR1C1, boolean isLocal)
```


Legt den Bereich fest, der zum Befüllen des Steuerelements verwendet wird.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Der Bereich, der zum Füllen des Steuerelements verwendet wird. |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |

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

### setLeftInShape(int value) {#setLeftInShape-int-}
```
public void setLeftInShape(int value)
```


Stellt den horizontalen Versatz der Form vom linken Rand der übergeordneten Form dar, in Einheiten von 1/4000 der Breite der übergeordneten Form.

**Remarks**

Gilt nur, wenn diese Form in einer Gruppe oder einem Diagramm ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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


Legt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts fest.

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

### setLinkedCell(String formula, boolean isR1C1, boolean isLocal) {#setLinkedCell-java.lang.String-boolean-boolean-}
```
public void setLinkedCell(String formula, boolean isR1C1, boolean isLocal)
```


Legt den Bereich fest, der mit dem Wert des Steuerelements verknüpft ist.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Der Bereich, der mit dem Wert des Steuerelements verknüpft ist. |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


True bedeutet, dass das Seitenverhältnis der Form gesperrt ist.

**Remarks**

Nur für Bilder und Ole Objects. HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft Shape.IsAspectRatioLocked. Diese Eigenschaft wird 12 Monate später ab Juli 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True bedeutet, dass das Objekt nicht geändert werden kann, wenn das Blatt geschützt ist. Beachten Sie, dass dieser Wert nur sinnvoll ist, wenn das Arbeitsblatt oder die Objekte im Arbeitsblatt geschützt sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLockedProperty(int type, boolean value) {#setLockedProperty-int-boolean-}
```
public void setLockedProperty(int type, boolean value)
```


Setzt die gesperrte Eigenschaft.

**Example**

```
         shape.setLockedProperty(ShapeLockType.ADJUST_HANDLES, true);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). Der gesperrte Typ. |
| Wert | boolean | Der Wert der Eigenschaft. |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Legt den horizontalen Versatz der Form von ihrer unteren rechten Eckspalte fest.

**Remarks**

Der Wertebereich liegt zwischen 0 und 1024.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Legt den vertikalen Versatz der Form von ihrer unteren rechten Eckzeile fest.

**Remarks**

Der Wertebereich liegt zwischen 0 und 256.

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

### setMacroName(String value) {#setMacroName-java.lang.String-}
```
public void setMacroName(String value)
```


Legt den Namen des Makros fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setMax(int value) {#setMax-int-}
```
public void setMax(int value)
```


Legt den Maximalwert eines Bildlaufleisten- oder Spinnerbereichs fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMin(int value) {#setMin-int-}
```
public void setMin(int value)
```


Legt den Minimalwert eines Bildlaufleisten- oder Spinnerbereichs fest.

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

### setPageChange(int value) {#setPageChange-int-}
```
public void setPageChange(int value)
```


Legt die Seitenänderung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Stellt dar, wie das Zeichenobjekt an den darunter liegenden Zellen befestigt ist. Die property steuert die Platzierung eines Objekts auf einem Arbeitsblatt.

Siehe [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Gibt an, ob das Objekt druckbar ist. Wenn False, wird diese Form beim Drucken nicht ausgedruckt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Gibt an, ob die Form 3‑D‑Schattierung hat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSoftEdges(double value) {#setSoftEdges-double-}
```
public void setSoftEdges(double value)
```


Legt den Radius der Unschärfe fest, der auf die Kanten angewendet wird, in Einheit von Punkten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Legt den Text dieser Form fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Legt die Richtung des Textflusses für dieses Objekt fest.

Siehe [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Legt den Typ der horizontalen Textausrichtung der Form fest.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Legt den Typ des horizontalen Textüberlaufs der Form fest, die Text enthält.

Siehe [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextOptions(TextOptions value) {#setTextOptions-com.aspose.cells.TextOptions-}
```
public void setTextOptions(TextOptions value)
```


Stellt die Textoptionen der Form dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [TextOptions](../../com.aspose.cells/textoptions) |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Legt den Typ der Textorientierung der Form fest.

Siehe [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Legt den voreingestellten Textformtyp fest.

Siehe [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Legt den Typ der vertikalen Textausrichtung der Form fest.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Legt den Typ des vertikalen Textüberlaufs der Form fest, die Text enthält.

Siehe [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

### setTopInShape(int value) {#setTopInShape-int-}
```
public void setTopInShape(int value)
```


Stellt den vertikalen Versatz der Form vom oberen Rand der übergeordneten Form in Einheiten von 1/4000 der Höhe der übergeordneten Form dar.

**Remarks**

Gilt nur, wenn diese Form in einer Gruppe oder einem Diagramm ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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


Legt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts fest, in Einheit von Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Legt den horizontalen Versatz der Form von ihrer oberen linken Spalte fest.

**Remarks**

Der Wertebereich liegt zwischen 0 und 1024.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Legt den vertikalen Versatz der Form von ihrer oberen linken Zeile fest.

**Remarks**

Der Wertebereich liegt zwischen 0 und 256.

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


Stellt den Index der obersten Zeile dar.

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

### setWidthInShape(int value) {#setWidthInShape-int-}
```
public void setWidthInShape(int value)
```


Stellt die Breite der Form dar, in Einheit 1/4000 der übergeordneten Form.

**Remarks**

Gilt nur, wenn diese Form in einer Gruppe oder einem Diagramm ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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


Legt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts fest, in Einheit von Pixeln.

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

### toFrontOrBack(int orders) {#toFrontOrBack-int-}
```
public void toFrontOrBack(int orders)
```


Bringt die Form nach vorne oder sendet die Form nach hinten.

**Example**

```
         shape.toFrontOrBack(2);
         //or shape.ToFrontOrBack(-1);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| orders | int | Wenn es kleiner als Null ist, wird die Form nach hinten gesetzt. Wenn es größer als Null ist, wird die Form nach vorne gebracht. |

### toImage(OutputStream stream, ImageFormat imageFormat) {#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-}
```
public void toImage(OutputStream stream, ImageFormat imageFormat)
```


Erstellt das Formbild und speichert es in einen Stream im angegebenen Format.

**Remarks**

Die folgenden Formate werden unterstützt: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Ausgabestream. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | Das Format, in dem das Bild gespeichert werden soll. |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Speichert die Form in einen Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Speichert die Form in einer Datei.

**Example**

```
         ImageOrPrintOptions op = new ImageOrPrintOptions();
         shape.toImage("exmaple.png", op);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
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


Aktualisiert den ausgewählten Wert anhand des Werts der verknüpften Zelle.

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

