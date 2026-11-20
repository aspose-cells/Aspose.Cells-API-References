---
title: "SvgImageOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Optionen zur Erzeugung einer SVG‑Abbildung."
type: docs
url: /de/java/com.aspose.cells/svgimageoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
```
public class SvgImageOptions extends ImageOrPrintOptions
```

Optionen zur Erzeugung einer SVG‑Abbildung.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SvgImageOptions()](#SvgImageOptions--) | Konstruktor. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. |
| [getChartImageType()](#getChartImageType--) | Gibt den Bildtyp des Diagramms beim Konvertieren an. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie im pdf,image als Block erscheinen. |
| [getClass()](#getClass--) |  |
| [getCssPrefix()](#getCssPrefix--) | Ermittelt das Präfix des CSS‑Namens in SVG, der Standardwert ist eine leere Zeichenkette. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Liefert benutzerdefinierte Einstellungen während des Renderns. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Liefert die Standardsprache für die Bearbeitung. |
| [getDefaultFont()](#getDefaultFont--) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie im pdf,image als Block erscheinen. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | Ermittelt den Typ der Schriftart, die in SVG eingebettet ist. |
| [getEmbededImageNameInSvg()](#getEmbededImageNameInSvg--) | Gibt den Dateinamen des eingebetteten Bildes in SVG an. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Einstellung zum Rendern von EMF-Metadateien in der Quelldatei. |
| [getFitToViewPort()](#getFitToViewPort--) | Wenn diese Eigenschaft wahr ist, passt das erzeugte SVG zur Ansichtsebene. |
| [getGridlineColor()](#getGridlineColor--) | Ermittelt die Gitterlinienfarbe. |
| [getGridlineType()](#getGridlineType--) | Liefert den Typ der Gitternetzlinien. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Ermittelt die horizontale Auflösung für erzeugte Bilder, in Punkten pro Zoll. |
| [getImageType()](#getImageType--) | Ermittelt das Format der erzeugten Bilder. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. |
| [getOnlyArea()](#getOnlyArea--) | Wenn diese Eigenschaft wahr ist, wird ein Bereich ausgegeben und es wird keine Skalierung angewendet. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist. |
| [getPageCount()](#getPageCount--) | Ermittelt die Anzahl der zu speichernden Seiten. |
| [getPageIndex()](#getPageIndex--) | Ermittelt den 0‑basierten Index der ersten zu speichernden Seite. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Steuert/Zeigt den Fortschritt des Seiten‑Speichervorgangs an. |
| [getPrintWithStatusDialog()](#getPrintWithStatusDialog--) | Wenn PrintWithStatusDialog = true ist, wird ein Dialog angezeigt, der den aktuellen Druckstatus zeigt. |
| [getPrintingPage()](#getPrintingPage--) | Gibt an, welche Seiten nicht gedruckt werden. |
| [getQuality()](#getQuality--) | Ermittelt einen Wert, der die Qualität der erzeugten Bilder bestimmt und nur beim Speichern von Seiten im `Jpeg`‑Format angewendet wird. |
| [getSVGFitToViewPort()](#getSVGFitToViewPort--) | Wenn diese Eigenschaft wahr ist, passt das erzeugte SVG zur Ansichtsebene. |
| [getSaveFormat()](#getSaveFormat--) | Ermittelt den Ausgabedateiformattyp. Unterstützt Tiff/XPS |
| [getSheetSet()](#getSheetSet--) | Ruft die zu rendernden Arbeitsblätter ab. |
| [getSvgCssPrefix()](#getSvgCssPrefix--) | Ermittelt das Präfix des CSS‑Namens in SVG, der Standardwert ist eine leere Zeichenkette. |
| [getTextCrossType()](#getTextCrossType--) | Ermittelt den Anzeigetexttyp, wenn die Textbreite größer als die Zellenbreite ist. |
| [getTiffColorDepth()](#getTiffColorDepth--) | Ermittelt die Bittiefe, die nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird. |
| [getTiffCompression()](#getTiffCompression--) | Ermittelt den Kompressionstyp, der nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird. |
| [getTiffPhotometricInterpretation()](#getTiffPhotometricInterpretation--) | Ermittelt den Typ der PhotometricInterpretation, der nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird. |
| [getTransparent()](#getTransparent--) | Gibt an, ob der Hintergrund des erzeugten Bildes transparent sein soll. |
| [getVerticalResolution()](#getVerticalResolution--) | Ermittelt die vertikale Auflösung für erzeugte Bilder in Punkten pro Zoll. |
| [getWarningCallback()](#getWarningCallback--) | Liest den Warn‑Callback. |
| [hashCode()](#hashCode--) |  |
| [isCellAutoFit()](#isCellAutoFit--) | Gibt an, ob Breite und Höhe der Zellen automatisch an den Zellenwert angepasst werden. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Gibt an, ob nur die Schriftart des Zeichens ausgetauscht werden soll, wenn die Zellen‑Schriftart nicht kompatibel ist. |
| [isOptimized()](#isOptimized--) | Gibt an, ob die Ausgabeelemente optimiert werden sollen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. |
| [setCellAutoFit(boolean value)](#setCellAutoFit-boolean-) | Gibt an, ob Breite und Höhe der Zellen automatisch an den Zellenwert angepasst werden. |
| [setChartImageType(ImageFormat value)](#setChartImageType-com.aspose.cells.ImageFormat-) | Gibt den Bildtyp des Diagramms beim Konvertieren an. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie im pdf,image als Block erscheinen. |
| [setCssPrefix(String value)](#setCssPrefix-java.lang.String-) | Legt das Präfix des CSS-Namens in SVG fest, der Standardwert ist eine leere Zeichenkette. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Legt benutzerdefinierte Einstellungen während des Renderns fest. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Legt die Standardsprache für die Bearbeitung fest. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie im pdf,image als Block erscheinen. |
| [setDesiredSize(int desiredWidth, int desiredHeight)](#setDesiredSize-int-int-) | Legt die gewünschte Breite und Höhe des Bildes fest. |
| [setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)](#setDesiredSize-int-int-boolean-) | Legt die gewünschte Breite und Höhe des Bildes fest. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | Legt den Typ der Schriftart fest, die in SVG eingebettet wird. |
| [setEmbededImageNameInSvg(String value)](#setEmbededImageNameInSvg-java.lang.String-) | Gibt den Dateinamen des eingebetteten Bildes in SVG an. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Einstellung zum Rendern von EMF-Metadateien in der Quelldatei. |
| [setFitToViewPort(boolean value)](#setFitToViewPort-boolean-) | Wenn diese Eigenschaft wahr ist, passt das erzeugte SVG zur Ansichtsebene. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Gibt an, ob nur die Schriftart des Zeichens ausgetauscht werden soll, wenn die Zellen‑Schriftart nicht kompatibel ist. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Legt die Farbe der Gitternetzlinien fest. |
| [setGridlineType(int value)](#setGridlineType-int-) | Legt den Typ der Rasterlinien fest. |
| [setHorizontalResolution(int value)](#setHorizontalResolution-int-) | Legt die horizontale Auflösung für erzeugte Bilder in Punkten pro Zoll fest. |
| [setImageType(int value)](#setImageType-int-) | Legt das Format der erzeugten Bilder fest. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. |
| [setOnlyArea(boolean value)](#setOnlyArea-boolean-) | Wenn diese Eigenschaft wahr ist, wird ein Bereich ausgegeben und es wird keine Skalierung angewendet. |
| [setOptimized(boolean value)](#setOptimized-boolean-) | Gibt an, ob die Ausgabeelemente optimiert werden sollen. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist. |
| [setPageCount(int value)](#setPageCount-int-) | Legt die Anzahl der zu speichernden Seiten fest. |
| [setPageIndex(int value)](#setPageIndex-int-) | Legt den 0‑basierten Index der ersten zu speichernden Seite fest. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Steuert/Zeigt den Fortschritt des Seiten‑Speichervorgangs an. |
| [setPrintWithStatusDialog(boolean value)](#setPrintWithStatusDialog-boolean-) | Wenn PrintWithStatusDialog = true ist, wird ein Dialog angezeigt, der den aktuellen Druckstatus zeigt. |
| [setPrintingPage(int value)](#setPrintingPage-int-) | Gibt an, welche Seiten nicht gedruckt werden. |
| [setQuality(int value)](#setQuality-int-) | Legt einen Wert fest, der die Qualität der erzeugten Bilder bestimmt und nur beim Speichern von Seiten im `Jpeg`‑Format angewendet wird. |
| [setRenderingHint(RenderingHints.Key key, Object value)](#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-) | Legt den Wert einer einzelnen Einstellung für die Rendering‑Algorithmen fest. |
| [setSVGFitToViewPort(boolean value)](#setSVGFitToViewPort-boolean-) | Wenn diese Eigenschaft wahr ist, passt das erzeugte SVG zur Ansichtsebene. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Legt den Ausgabedateiformattyp fest, unterstützt Tiff/XPS |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Legt die zu rendernden Arbeitsblätter fest. |
| [setSvgCssPrefix(String value)](#setSvgCssPrefix-java.lang.String-) | Legt das Präfix des CSS-Namens in SVG fest, der Standardwert ist eine leere Zeichenkette. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Legt den Anzeigetexttyp fest, wenn die Textbreite größer als die Zellenbreite ist. |
| [setTiffColorDepth(int value)](#setTiffColorDepth-int-) | Legt die Bittiefe fest, die nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Legt den Kompressionstyp fest, der nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird. |
| [setTiffPhotometricInterpretation(int value)](#setTiffPhotometricInterpretation-int-) | Legt den Typ der PhotometricInterpretation fest, der nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Gibt an, ob der Hintergrund des erzeugten Bildes transparent sein soll. |
| [setVerticalResolution(int value)](#setVerticalResolution-int-) | Legt die vertikale Auflösung für erzeugte Bilder in Punkten pro Zoll fest. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Legt die Warn‑Callback‑Funktion fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SvgImageOptions() {#SvgImageOptions--}
```
public SvgImageOptions()
```


Konstruktor.

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
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Breite der Papiergröße der Seiten­einrichtung wird ungültig, während die anderen Einstellungen der Seiten­einrichtung weiterhin wirksam bleiben.

**Returns:**
boolean
### getChartImageType() {#getChartImageType--}
```
public ImageFormat getChartImageType()
```


Gibt den Bildtyp des Diagramms beim Konvertieren an. Standardwert: PNG.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen werden Diagramm und Form immer als Vektorelemente (z. B. Punkt, Linie) für die Renderqualität dargestellt. Diese Eigenschaft wird 12 Monate später, seit Juni 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


Wenn Zeichen in Excel Unicode sind und nicht mit der korrekten Schriftart im Zellenstil festgelegt wurden, können sie im pdf,image als Blockzeichen erscheinen. Setzen Sie dies auf true, um zunächst die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen anzuzeigen.

**Remarks**

Standard ist true.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssPrefix() {#getCssPrefix--}
```
public String getCssPrefix()
```


Ermittelt das Präfix des CSS‑Namens in SVG, der Standardwert ist eine leere Zeichenkette.

**Returns:**
java.lang.String
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


Liefert benutzerdefinierte Einstellungen während des Renderns.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Liefert die Standardsprache für die Bearbeitung.

Siehe [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Es kann unterschiedliche Layouts für Textabsätze anzeigen/rendern, wenn verschiedene Bearbeitungssprachen festgelegt sind. Standard ist [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


Wenn Zeichen in Excel Unicode sind und nicht mit der korrekten Schriftart im Zellenstil festgelegt wurden, können sie im pdf,image als Blockzeichen erscheinen. Setzen Sie die DefaultFont auf z. B. MingLiu oder MS Gothic, um diese Zeichen anzuzeigen. Wenn diese Eigenschaft nicht gesetzt ist, verwendet Aspose.Cells die systemweite Standardschriftart, um diese Unicode‑Zeichen darzustellen.

**Returns:**
java.lang.String
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```


Ermittelt den Typ der Schriftart, die in SVG eingebettet ist.

Siehe [SvgEmbeddedFontType](../../com.aspose.cells/svgembeddedfonttype).

**Remarks**

Standardwert ist [SvgEmbeddedFontType.NONE](../../com.aspose.cells/svgembeddedfonttype\#NONE), was bedeutet, dass keine Schriftart in Svg eingebettet wird.

**Returns:**
int
### getEmbededImageNameInSvg() {#getEmbededImageNameInSvg--}
```
public String getEmbededImageNameInSvg()
```


Geben Sie den Dateinamen des eingebetteten Bildes in svg an. Dies sollte ein voller Pfad mit Verzeichnis sein, z. B. "c:\\\\xpsEmbedded".

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen entfernen Sie bitte diese Eigenschaft, da Bilder jetzt immer im Svg im Base64-Format eingebettet werden. Diese Eigenschaft wird 12 Monate später, seit April 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
java.lang.String
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Einstellung zum Rendern von EMF-Metadateien in der Quelldatei.

Siehe [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

EMF-Metadateien, die als "EMF+ Dual" identifiziert werden, können sowohl EMF+-Datensätze als auch EMF-Datensätze enthalten. Jeder Datensatztyp kann zum Rendern des Bildes verwendet werden, nur EMF+-Datensätze oder nur EMF-Datensätze. Wenn [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) gesetzt ist, werden EMF+-Datensätze beim Rendern des Bildes geparst, andernfalls werden nur EMF-Datensätze geparst. Der Standardwert ist [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). Für Frameworks, die von .NET System.Drawing.Common abhängen, wird diese Einstellung ignoriert.

**Returns:**
int
### getFitToViewPort() {#getFitToViewPort--}
```
public boolean getFitToViewPort()
```


Wenn diese Eigenschaft wahr ist, passt das erzeugte SVG zur Ansichtsebene.

**Returns:**
boolean
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Ermittelt die Gitterlinienfarbe.

**Remarks**

Es wird die Rasterlinienfarbeneinstellungen in der Quelldatei ignorieren.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


Liefert den Typ der Gitternetzlinien.

Siehe [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Standard ist der Typ Dotted.

**Returns:**
int
### getHorizontalResolution() {#getHorizontalResolution--}
```
public int getHorizontalResolution()
```


Ermittelt die horizontale Auflösung für erzeugte Bilder, in Punkten pro Zoll.

**Remarks**

Der Standardwert ist 96. Das Festlegen von  und  wirkt sich auf die Breite und Höhe des Ausgabebildes in Pixeln aus.

**Example**

Der folgende Code setzt die Auflösung auf 192, die Breite und Höhe des erzeugten Bildes ist doppelt so groß wie bei einer Auflösung, die beim Standardwert 96 belassen wird.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render worksheet page to image.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), opts);
         sr.toImage(0, "Sheet_Page1.png");
```

**Returns:**
int
### getImageType() {#getImageType--}
```
public int getImageType()
```


Ermittelt das Format der erzeugten Bilder. Standardwert: PNG.

Siehe [ImageType](../../com.aspose.cells/imagetype).

**Returns:**
int
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Papiergröße von pagesetup wird ungültig sein, und die anderen Einstellungen von pagesetup bleiben wirksam.

**Returns:**
boolean
### getOnlyArea() {#getOnlyArea--}
```
public boolean getOnlyArea()
```


Wenn diese Eigenschaft wahr ist, wird ein Bereich ausgegeben und es wird keine Skalierung angewendet.

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist.

**Remarks**

Standard ist false.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Ermittelt die Anzahl der zu speichernden Seiten.

**Remarks**

Standard ist System.Int32.MaxValue, was bedeutet, dass alle Seiten gerendert werden.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Ermittelt den 0‑basierten Index der ersten zu speichernden Seite.

**Remarks**

Standard ist 0.

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Steuert/Zeigt den Fortschritt des Seiten‑Speichervorgangs an.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintWithStatusDialog() {#getPrintWithStatusDialog--}
```
public boolean getPrintWithStatusDialog()
```


Wenn PrintWithStatusDialog = true, wird ein Dialog angezeigt, der den aktuellen Druckstatus zeigt. Andernfalls wird kein solcher Dialog angezeigt.

**Returns:**
boolean
### getPrintingPage() {#getPrintingPage--}
```
public int getPrintingPage()
```


Gibt an, welche Seiten nicht gedruckt werden.

Siehe [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Returns:**
int
### getQuality() {#getQuality--}
```
public int getQuality()
```


Ermittelt einen Wert, der die Qualität der erzeugten Bilder bestimmt und nur beim Speichern von Seiten im `Jpeg`-Format angewendet wird. Der Standardwert ist 100

**Remarks**

Wirkt nur beim Speichern als JPEG. Der Wert muss zwischen 0 und 100 liegen. Der Standardwert ist 100.

**Returns:**
int
### getSVGFitToViewPort() {#getSVGFitToViewPort--}
```
public boolean getSVGFitToViewPort()
```


Wenn diese Eigenschaft wahr ist, passt das erzeugte SVG zur Ansichtsebene.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). Diese Eigenschaft wird 12 Monate später, seit April 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ermittelt den Ausgabedateiformattyp. Unterstützt Tiff/XPS

Siehe [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie für Tiff/Svg [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); für Xps [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) mit [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). Diese Eigenschaft wird 12 Monate später, seit August 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Ermittelt die zu rendernden Arbeitsblätter. Standard ist jedes sichtbare Arbeitsblatt im Arbeitsbuch: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

Das Set wird ignoriert, wenn es in [SheetRender](../../com.aspose.cells/sheetrender) verwendet wird

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSvgCssPrefix() {#getSvgCssPrefix--}
```
public String getSvgCssPrefix()
```


Ermittelt das Präfix des CSS‑Namens in SVG, der Standardwert ist eine leere Zeichenkette.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen bitte [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). Diese Eigenschaft wird 12 Monate später, seit April 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
java.lang.String
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Ermittelt den Anzeigetexttyp, wenn die Textbreite größer als die Zellenbreite ist.

Siehe [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
### getTiffColorDepth() {#getTiffColorDepth--}
```
public int getTiffColorDepth()
```


Ermittelt die Bittiefe, die nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird.

Siehe [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

Wirkt nur beim Speichern als TIFF. Wenn TiffCompression auf CCITT3, CCITT4 gesetzt ist, hat dies keine Wirkung, die Bit-Tiefe des erzeugten TIFF-Bildes ist immer 1.

**Returns:**
int
### getTiffCompression() {#getTiffCompression--}
```
public int getTiffCompression()
```


Ermittelt den Kompressionstyp, der nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird.

Siehe [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

Wirkt nur beim Speichern als TIFF. Der Standardwert ist Lzw.

**Returns:**
int
### getTiffPhotometricInterpretation() {#getTiffPhotometricInterpretation--}
```
public int getTiffPhotometricInterpretation()
```


Ermittelt den Typ der PhotometricInterpretation, der nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird.

**Remarks**

Wirkt nur beim Speichern als TIFF. Der Standardwert ist -1, was bedeutet, dass keine PhotometricInterpretation angewendet wird.

**Returns:**
int
### getTransparent() {#getTransparent--}
```
public boolean getTransparent()
```


Gibt an, ob der Hintergrund des erzeugten Bildes transparent sein soll.

**Remarks**

Der Standardwert ist false. Das bedeutet, dass der Hintergrund der erzeugten Bilder weiß ist.

**Returns:**
boolean
### getVerticalResolution() {#getVerticalResolution--}
```
public int getVerticalResolution()
```


Ermittelt die vertikale Auflösung für erzeugte Bilder in Punkten pro Zoll.

**Remarks**

Der Standardwert ist 96. Das Festlegen von  und  wirkt sich auf die Breite und Höhe des Ausgabebildes in Pixeln aus.

**Example**

Der folgende Code setzt die Auflösung auf 192, die Breite und Höhe des erzeugten Bildes ist doppelt so groß wie bei einer Auflösung, die beim Standardwert 96 belassen wird.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render Chart to image.
         wb.getWorksheets().get(0).getCharts().get(0).toImage("Chart.png", opts);
```

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Liest den Warn‑Callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellAutoFit() {#isCellAutoFit--}
```
public boolean isCellAutoFit()
```


Gibt an, ob Breite und Höhe der Zellen automatisch an den Zellenwert angepasst werden. Der Standardwert ist false.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen wird diese Eigenschaft nicht verwendet, bitte entfernen Sie diese Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit August 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Returns:**
boolean
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Gibt an, ob nur die Schriftart des Zeichens ausgetauscht werden soll, wenn die Zellen‑Schriftart nicht kompatibel ist.

**Remarks**

Standard ist false. Wir versuchen zuerst die Standardschriftart des Workbooks und PdfSaveOption/System für die Zellen­schrift.

**Returns:**
boolean
### isOptimized() {#isOptimized--}
```
public boolean isOptimized()
```


Gibt an, ob die Ausgabeelemente optimiert werden sollen.

**Remarks**

Der Standardwert ist false. Derzeit, wenn diese Eigenschaft auf true gesetzt wird, werden folgende Optimierungen durchgeführt: 1. Optimierung der Randlinien. 2. Optimierung der Dateigröße beim Rendern zu einem Svg-Bild.

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




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Breite der Papiergröße der Seiten­einrichtung wird ungültig, während die anderen Einstellungen der Seiten­einrichtung weiterhin wirksam bleiben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCellAutoFit(boolean value) {#setCellAutoFit-boolean-}
```
public void setCellAutoFit(boolean value)
```


Gibt an, ob Breite und Höhe der Zellen automatisch an den Zellenwert angepasst werden. Der Standardwert ist false.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen wird diese Eigenschaft nicht verwendet, bitte entfernen Sie diese Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit August 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setChartImageType(ImageFormat value) {#setChartImageType-com.aspose.cells.ImageFormat-}
```
public void setChartImageType(ImageFormat value)
```


Gibt den Bildtyp des Diagramms beim Konvertieren an. Standardwert: PNG.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen werden Diagramm und Form immer als Vektorelemente (z. B. Punkt, Linie) für die Renderqualität dargestellt. Diese Eigenschaft wird 12 Monate später, seit Juni 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


Wenn Zeichen in Excel Unicode sind und nicht mit der korrekten Schriftart im Zellenstil festgelegt wurden, können sie im pdf,image als Blockzeichen erscheinen. Setzen Sie dies auf true, um zunächst die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen anzuzeigen.

**Remarks**

Standard ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCssPrefix(String value) {#setCssPrefix-java.lang.String-}
```
public void setCssPrefix(String value)
```


Legt das Präfix des CSS-Namens in SVG fest, der Standardwert ist eine leere Zeichenkette.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


Legt benutzerdefinierte Einstellungen während des Renderns fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Legt die Standardsprache für die Bearbeitung fest.

Siehe [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Es kann unterschiedliche Layouts für Textabsätze anzeigen/rendern, wenn verschiedene Bearbeitungssprachen festgelegt sind. Standard ist [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


Wenn Zeichen in Excel Unicode sind und nicht mit der korrekten Schriftart im Zellenstil festgelegt wurden, können sie im pdf,image als Blockzeichen erscheinen. Setzen Sie die DefaultFont auf z. B. MingLiu oder MS Gothic, um diese Zeichen anzuzeigen. Wenn diese Eigenschaft nicht gesetzt ist, verwendet Aspose.Cells die systemweite Standardschriftart, um diese Unicode‑Zeichen darzustellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDesiredSize(int desiredWidth, int desiredHeight) {#setDesiredSize-int-int-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight)
```


Legt die gewünschte Breite und Höhe des Bildes fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen bitte [setDesiredSize(int,int,boolean)](../../com.aspose.cells/imageorprintoptions\#setDesiredSize-int-int-boolean-) und setzen Sie den Parameter keepAspectRatio auf false. Diese Eigenschaft wird 12 Monate später, seit Mai 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| desiredWidth | int | gewünschte Breite in Pixeln |
| desiredHeight | int | gewünschte Höhe in Pixeln |

### setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio) {#setDesiredSize-int-int-boolean-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)
```


Legt die gewünschte Breite und Höhe des Bildes fest.

**Remarks**

Die Breite und Höhe des Ausgabebildes in Pixeln basieren ausschließlich auf der festgelegten gewünschten Breite und Höhe. Die  und  haben in diesem Fall keinen Einfluss auf die Breite und Höhe des Ausgabebildes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| desiredWidth | int | gewünschte Breite in Pixeln |
| desiredHeight | int | gewünschte Höhe in Pixeln |
| keepAspectRatio | boolean | ob das Seitenverhältnis des Originalbildes beibehalten werden soll |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```


Legt den Typ der Schriftart fest, die in SVG eingebettet wird.

Siehe [SvgEmbeddedFontType](../../com.aspose.cells/svgembeddedfonttype).

**Remarks**

Standardwert ist [SvgEmbeddedFontType.NONE](../../com.aspose.cells/svgembeddedfonttype\#NONE), was bedeutet, dass keine Schriftart in Svg eingebettet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEmbededImageNameInSvg(String value) {#setEmbededImageNameInSvg-java.lang.String-}
```
public void setEmbededImageNameInSvg(String value)
```


Geben Sie den Dateinamen des eingebetteten Bildes in svg an. Dies sollte ein voller Pfad mit Verzeichnis sein, z. B. "c:\\\\xpsEmbedded".

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen entfernen Sie bitte diese Eigenschaft, da Bilder jetzt immer im Svg im Base64-Format eingebettet werden. Diese Eigenschaft wird 12 Monate später, seit April 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Einstellung zum Rendern von EMF-Metadateien in der Quelldatei.

Siehe [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

EMF-Metadateien, die als "EMF+ Dual" identifiziert werden, können sowohl EMF+-Datensätze als auch EMF-Datensätze enthalten. Jeder Datensatztyp kann zum Rendern des Bildes verwendet werden, nur EMF+-Datensätze oder nur EMF-Datensätze. Wenn [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) gesetzt ist, werden EMF+-Datensätze beim Rendern des Bildes geparst, andernfalls werden nur EMF-Datensätze geparst. Der Standardwert ist [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). Für Frameworks, die von .NET System.Drawing.Common abhängen, wird diese Einstellung ignoriert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setFitToViewPort(boolean value) {#setFitToViewPort-boolean-}
```
public void setFitToViewPort(boolean value)
```


Wenn diese Eigenschaft wahr ist, passt das erzeugte SVG zur Ansichtsebene.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


Gibt an, ob nur die Schriftart des Zeichens ausgetauscht werden soll, wenn die Zellen‑Schriftart nicht kompatibel ist.

**Remarks**

Standard ist false. Wir versuchen zuerst die Standardschriftart des Workbooks und PdfSaveOption/System für die Zellen­schrift.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Legt die Farbe der Gitternetzlinien fest.

**Remarks**

Es wird die Rasterlinienfarbeneinstellungen in der Quelldatei ignorieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


Legt den Typ der Rasterlinien fest.

Siehe [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Standard ist der Typ Dotted.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHorizontalResolution(int value) {#setHorizontalResolution-int-}
```
public void setHorizontalResolution(int value)
```


Legt die horizontale Auflösung für erzeugte Bilder in Punkten pro Zoll fest.

**Remarks**

Der Standardwert ist 96. Das Festlegen von  und  wirkt sich auf die Breite und Höhe des Ausgabebildes in Pixeln aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setImageType(int value) {#setImageType-int-}
```
public void setImageType(int value)
```


Legt das Format der erzeugten Bilder fest. Standardwert: PNG.

Siehe [ImageType](../../com.aspose.cells/imagetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Papiergröße von pagesetup wird ungültig sein, und die anderen Einstellungen von pagesetup bleiben wirksam.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOnlyArea(boolean value) {#setOnlyArea-boolean-}
```
public void setOnlyArea(boolean value)
```


Wenn diese Eigenschaft wahr ist, wird ein Bereich ausgegeben und es wird keine Skalierung angewendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOptimized(boolean value) {#setOptimized-boolean-}
```
public void setOptimized(boolean value)
```


Gibt an, ob die Ausgabeelemente optimiert werden sollen.

**Remarks**

Der Standardwert ist false. Derzeit, wenn diese Eigenschaft auf true gesetzt wird, werden folgende Optimierungen durchgeführt: 1. Optimierung der Randlinien. 2. Optimierung der Dateigröße beim Rendern zu einem Svg-Bild.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist.

**Remarks**

Standard ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


Legt die Anzahl der zu speichernden Seiten fest.

**Remarks**

Standard ist System.Int32.MaxValue, was bedeutet, dass alle Seiten gerendert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


Legt den 0‑basierten Index der ersten zu speichernden Seite fest.

**Remarks**

Standard ist 0.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


Steuert/Zeigt den Fortschritt des Seiten‑Speichervorgangs an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPrintWithStatusDialog(boolean value) {#setPrintWithStatusDialog-boolean-}
```
public void setPrintWithStatusDialog(boolean value)
```


Wenn PrintWithStatusDialog = true, wird ein Dialog angezeigt, der den aktuellen Druckstatus zeigt. Andernfalls wird kein solcher Dialog angezeigt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPrintingPage(int value) {#setPrintingPage-int-}
```
public void setPrintingPage(int value)
```


Gibt an, welche Seiten nicht gedruckt werden.

Siehe [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setQuality(int value) {#setQuality-int-}
```
public void setQuality(int value)
```


Legt einen Wert fest, der die Qualität der erzeugten Bilder bestimmt und nur beim Speichern von Seiten im `Jpeg`-Format angewendet wird. Der Standardwert ist 100

**Remarks**

Wirkt nur beim Speichern als JPEG. Der Wert muss zwischen 0 und 100 liegen. Der Standardwert ist 100.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRenderingHint(RenderingHints.Key key, Object value) {#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-}
```
public void setRenderingHint(RenderingHints.Key key, Object value)
```


Setzt den Wert einer einzelnen Präferenz für die Rendering-Algorithmen. Hinweis-Kategorien umfassen Steuerungen für die Rendering-Qualität und den Gesamtabwägung von Zeit/Qualität im Rendering-Prozess. Weitere Informationen finden Sie in der Klasse RenderingHints zu Definitionen einiger gängiger Schlüssel und Werte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | java.awt.RenderingHints.Key | der Schlüssel des zu setzenden Hinweises. |
| Wert | java.lang.Object | der Wert, der Präferenzen für die angegebene Hinweis-Kategorie angibt. |

### setSVGFitToViewPort(boolean value) {#setSVGFitToViewPort-boolean-}
```
public void setSVGFitToViewPort(boolean value)
```


Wenn diese Eigenschaft wahr ist, passt das erzeugte SVG zur Ansichtsebene.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). Diese Eigenschaft wird 12 Monate später, seit April 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Legt den Ausgabedateiformattyp fest, unterstützt Tiff/XPS

Siehe [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie für Tiff/Svg [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); für Xps [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) mit [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). Diese Eigenschaft wird 12 Monate später, seit August 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Legt die zu rendernden Arbeitsblätter fest. Standard ist, dass alle sichtbaren Arbeitsblätter in der Arbeitsmappe verwendet werden: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

Das Set wird ignoriert, wenn es in [SheetRender](../../com.aspose.cells/sheetrender) verwendet wird

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSvgCssPrefix(String value) {#setSvgCssPrefix-java.lang.String-}
```
public void setSvgCssPrefix(String value)
```


Legt das Präfix des CSS-Namens in SVG fest, der Standardwert ist eine leere Zeichenkette.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen bitte [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). Diese Eigenschaft wird 12 Monate später, seit April 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


Legt den Anzeigetexttyp fest, wenn die Textbreite größer als die Zellenbreite ist.

Siehe [TextCrossType](../../com.aspose.cells/textcrosstype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTiffColorDepth(int value) {#setTiffColorDepth-int-}
```
public void setTiffColorDepth(int value)
```


Legt die Bittiefe fest, die nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird.

Siehe [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

Wirkt nur beim Speichern als TIFF. Wenn TiffCompression auf CCITT3, CCITT4 gesetzt ist, hat dies keine Wirkung, die Bit-Tiefe des erzeugten TIFF-Bildes ist immer 1.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public void setTiffCompression(int value)
```


Legt den Kompressionstyp fest, der nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird.

Siehe [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

Wirkt nur beim Speichern als TIFF. Der Standardwert ist Lzw.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTiffPhotometricInterpretation(int value) {#setTiffPhotometricInterpretation-int-}
```
public void setTiffPhotometricInterpretation(int value)
```


Legt den Typ der PhotometricInterpretation fest, der nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird.

**Remarks**

Wirkt nur beim Speichern als TIFF. Der Standardwert ist -1, was bedeutet, dass keine PhotometricInterpretation angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Gibt an, ob der Hintergrund des erzeugten Bildes transparent sein soll.

**Remarks**

Der Standardwert ist false. Das bedeutet, dass der Hintergrund der erzeugten Bilder weiß ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setVerticalResolution(int value) {#setVerticalResolution-int-}
```
public void setVerticalResolution(int value)
```


Legt die vertikale Auflösung für erzeugte Bilder in Punkten pro Zoll fest.

**Remarks**

Der Standardwert ist 96. Das Festlegen von  und  wirkt sich auf die Breite und Höhe des Ausgabebildes in Pixeln aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Legt die Warn‑Callback‑Funktion fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

