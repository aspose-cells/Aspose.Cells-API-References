---
title: "PaginatedSaveOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Optionen für die Seitennummerierung dar."
type: docs
url: /de/java/com.aspose.cells/paginatedsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public abstract class PaginatedSaveOptions extends SaveOptions
```

Stellt die Optionen für die Seitennummerierung dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PaginatedSaveOptions()](#PaginatedSaveOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Gibt an, ob die Schriftkompatibilität für jedes Zeichen im Text überprüft werden soll. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie im pdf,image als Block erscheinen. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [getCreateDirectory()](#getCreateDirectory--) | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Liefert benutzerdefinierte Einstellungen während des Renderns. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Liefert die Standardsprache für die Bearbeitung. |
| [getDefaultFont()](#getDefaultFont--) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie im pdf,image als Block erscheinen. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Einstellung für das Rendern von Emf-Metadateien. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. |
| [getGridlineColor()](#getGridlineColor--) | Liefert die Farbe der Gitternetzlinien. |
| [getGridlineType()](#getGridlineType--) | Liefert den Typ der Gitternetzlinien. |
| [getIgnoreError()](#getIgnoreError--) | Gibt an, ob Sie den Fehler beim Rendern ausblenden müssen. |
| [getMergeAreas()](#getMergeAreas--) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist. |
| [getPageCount()](#getPageCount--) | Ermittelt die Anzahl der zu speichernden Seiten. |
| [getPageIndex()](#getPageIndex--) | Ermittelt den 0‑basierten Index der ersten zu speichernden Seite. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Steuert/Zeigt den Fortschritt des Seiten‑Speichervorgangs an. |
| [getPrintingPageType()](#getPrintingPageType--) | Gibt an, welche Seiten nicht gedruckt werden. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen. |
| [getRenderingBehavior()](#getRenderingBehavior--) | Ermittelt die Excel-spezifischen Rendering‑Verhalten, die angewendet werden sollen. |
| [getSaveFormat()](#getSaveFormat--) | Ermittelt das Speicherdateiformat. |
| [getSheetSet()](#getSheetSet--) | Ruft die zu rendernden Arbeitsblätter ab. |
| [getSortExternalNames()](#getSortExternalNames--) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden. |
| [getSortNames()](#getSortNames--) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [getTextCrossType()](#getTextCrossType--) | Ermittelt den Anzeigetexttyp, wenn die Textbreite größer als die Zellenbreite ist. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden. |
| [getWarningCallback()](#getWarningCallback--) | Liest den Warn‑Callback. |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Gibt an, ob nur die Schriftart des Zeichens ausgetauscht werden soll, wenn die Zellen‑Schriftart nicht kompatibel ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Gibt an, ob die Schriftkompatibilität für jedes Zeichen im Text überprüft werden soll. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie im pdf,image als Block erscheinen. |
| [setClearData(boolean value)](#setClearData-boolean-) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Legt benutzerdefinierte Einstellungen während des Renderns fest. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Legt die Standardsprache für die Bearbeitung fest. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie im pdf,image als Block erscheinen. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Einstellung für das Rendern von Emf-Metadateien. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Gibt an, ob nur die Schriftart des Zeichens ausgetauscht werden soll, wenn die Zellen‑Schriftart nicht kompatibel ist. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Legt die Farbe der Rasterlinien fest. |
| [setGridlineType(int value)](#setGridlineType-int-) | Legt den Typ der Rasterlinien fest. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Gibt an, ob Sie den Fehler beim Rendern ausblenden müssen. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist. |
| [setPageCount(int value)](#setPageCount-int-) | Legt die Anzahl der zu speichernden Seiten fest. |
| [setPageIndex(int value)](#setPageIndex-int-) | Legt den 0‑basierten Index der ersten zu speichernden Seite fest. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Steuert/Zeigt den Fortschritt des Seiten‑Speichervorgangs an. |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Gibt an, welche Seiten nicht gedruckt werden. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | Legt die Excel-spezifischen Rendering‑Verhalten fest, die angewendet werden sollen. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Legt die zu rendernden Arbeitsblätter fest. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Legt den Anzeigetexttyp fest, wenn die Textbreite größer als die Zellenbreite ist. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Legt die Warn‑Callback‑Funktion fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PaginatedSaveOptions() {#PaginatedSaveOptions--}
```
public PaginatedSaveOptions()
```


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


Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Breite der Papiergröße von pagesetup wird ignoriert, und die anderen Einstellungen von pagesetup bleiben wirksam.

**Returns:**
boolean
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können.

**Remarks**

Wenn der Ordner nicht angegeben wurde, ist der Standardwert dafür [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Wenn sein Standardwert null oder leer ist oder als null oder leer angegeben wurde, wird beim Speichern der Arbeitsmappe keine Cache‑Datei verwendet.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Ob die Beschränkungen einer Excel-Datei geprüft werden, wenn der Benutzer Zellen-bezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht das Eingeben eines Zeichenfolgenwerts, der länger als 32 K ist. Wenn Sie einen Wert eingeben, der länger als 32 K ist, wird er abgeschnitten.

**Returns:**
boolean
### getCheckFontCompatibility() {#getCheckFontCompatibility--}
```
public boolean getCheckFontCompatibility()
```


Gibt an, ob die Schriftkompatibilität für jedes Zeichen im Text überprüft werden soll.

**Remarks**

Der Standardwert ist true. Das Deaktivieren dieser Eigenschaft kann die Leistung verbessern. Wenn jedoch die Standard‑ oder angegebene Schriftart für Text/character nicht zum Rendern verwendet werden kann, können im erzeugten pdf unlesbare Zeichen (wie Block) auftreten. In einer solchen Situation sollte der Benutzer diese Eigenschaft auf true belassen, damit eine alternative Schriftart gesucht und zum Rendern des Textes verwendet wird;

**Returns:**
boolean
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
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Leert die Arbeitsmappe nach dem Speichern der Datei.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
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
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Einstellung für das Rendern von Emf-Metadateien.

Siehe [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

EMF‑Metadateien, die als \"EMF+ Dual\" identifiziert werden, können sowohl EMF+‑Datensätze als auch EMF‑Datensätze enthalten. Jeder dieser Datensatztypen kann zum Rendern des Bildes verwendet werden, nur EMF+‑Datensätze oder nur EMF‑Datensätze. Wenn [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) gesetzt ist, werden EMF+‑Datensätze beim Rendern der Seite geparst, andernfalls werden nur EMF‑Datensätze geparst. Der Standardwert ist [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).

**Returns:**
int
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.

**Remarks**

Nur für .xls, .xlsx, .xlsb und .xlsm-Dateien.

**Returns:**
boolean
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Liefert die Farbe der Gitternetzlinien.

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
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Gibt an, ob Sie den Fehler beim Rendern ausblenden müssen. Der Fehler kann ein Fehler in Form, Bild, Diagramm-Rendering usw. sein.

**Returns:**
boolean
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Papiergröße von pagesetup wird ungültig sein, und die anderen Einstellungen von pagesetup bleiben wirksam.

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist.

**Remarks**

Standard ist true.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Ermittelt die Anzahl der zu speichernden Seiten.

**Remarks**

Standard ist System.Int32.MaxValue, was bedeutet, dass alle Seiten gerendert werden.

**Example**

Das folgende Beispiel zeigt, wie man einen Seitenbereich (3 und 4) in einer Microsoft‑Excel‑Datei in PDF rendert.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Ermittelt den 0‑basierten Index der ersten zu speichernden Seite.

**Remarks**

Standard ist 0.

**Example**

Das folgende Beispiel zeigt, wie man einen Seitenbereich (3 und 4) in einer Microsoft‑Excel‑Datei in PDF rendert.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Steuert/Zeigt den Fortschritt des Seiten‑Speichervorgangs an.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintingPageType() {#getPrintingPageType--}
```
public int getPrintingPageType()
```


Gibt an, welche Seiten nicht gedruckt werden.

Siehe [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Wenn der Inhalt im Blatt spärlich ist, können einige Seiten in der ausgegebenen PDF-Datei völlig leer sein. Wenn Sie diese leeren Seiten nicht möchten, können Sie diese Option verwenden, um sie zu entfernen.

**Example**

Der folgende Code lässt leere Seiten oder Seiten weg, die nur Stil‑Inhalte wie Zellhintergrund, Rahmen usw. enthalten.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //ignore blank pages
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_BLANK);
 
         wb.save("output_ignore_blank_page.pdf", pdfSaveOptions);
 
 
         //ignore blank pages and pages which only contains some style content like cell background
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_STYLE);
 
         wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
```

**Returns:**
int
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen.

**Returns:**
boolean
### getRenderingBehavior() {#getRenderingBehavior--}
```
public int getRenderingBehavior()
```


Ermittelt die Excel-spezifischen Rendering‑Verhalten, die angewendet werden sollen.

Siehe [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

Der Standardwert ist [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\#ALL).

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ermittelt das Speicherdateiformat.

Siehe [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Ermittelt die zu rendernden Arbeitsblätter. Standard ist jedes sichtbare Arbeitsblatt im Arbeitsbuch: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Example**

Der folgende Code rendert nur das aktive Blatt zu PDF.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         int activeSheetIndex = workbook.getWorksheets().getActiveSheetIndex();
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
         //set active sheet index to sheet set.
         pdfSaveOptions.setSheetSet(new SheetSet(new int[] { activeSheetIndex }));
         workbook.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.

**Returns:**
boolean
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Ermittelt den Anzeigetexttyp, wenn die Textbreite größer als die Zellenbreite ist.

Siehe [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Gibt an, ob die Smart‑Art‑Einstellung aktualisiert wird. Der Standardwert ist false.

**Remarks**

Wirkt nur nach dem Aufruf der Methode Shape.GetResultOfSmartArt() und wenn die zwischengespeicherten Shapes in der Vorlagendatei vorhanden sind.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
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
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Gibt an, ob nur die Schriftart des Zeichens ausgetauscht werden soll, wenn die Zellen‑Schriftart nicht kompatibel ist.

**Remarks**

Standard ist false. Wir versuchen zuerst die Standardschriftart des Workbooks und PdfSaveOption/System für die Zellen­schrift.

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


Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Breite der Papiergröße von pagesetup wird ignoriert, und die anderen Einstellungen von pagesetup bleiben wirksam.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können.

**Remarks**

Wenn der Ordner nicht angegeben wurde, ist der Standardwert dafür [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Wenn sein Standardwert null oder leer ist oder als null oder leer angegeben wurde, wird beim Speichern der Arbeitsmappe keine Cache‑Datei verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Ob die Beschränkungen einer Excel-Datei geprüft werden, wenn der Benutzer Zellen-bezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht das Eingeben eines Zeichenfolgenwerts, der länger als 32 K ist. Wenn Sie einen Wert eingeben, der länger als 32 K ist, wird er abgeschnitten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCheckFontCompatibility(boolean value) {#setCheckFontCompatibility-boolean-}
```
public void setCheckFontCompatibility(boolean value)
```


Gibt an, ob die Schriftkompatibilität für jedes Zeichen im Text überprüft werden soll.

**Remarks**

Der Standardwert ist true. Das Deaktivieren dieser Eigenschaft kann die Leistung verbessern. Wenn jedoch die Standard‑ oder angegebene Schriftart für Text/character nicht zum Rendern verwendet werden kann, können im erzeugten pdf unlesbare Zeichen (wie Block) auftreten. In einer solchen Situation sollte der Benutzer diese Eigenschaft auf true belassen, damit eine alternative Schriftart gesucht und zum Rendern des Textes verwendet wird;

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Leert die Arbeitsmappe nach dem Speichern der Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Einstellung für das Rendern von Emf-Metadateien.

Siehe [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

EMF‑Metadateien, die als \"EMF+ Dual\" identifiziert werden, können sowohl EMF+‑Datensätze als auch EMF‑Datensätze enthalten. Jeder dieser Datensatztypen kann zum Rendern des Bildes verwendet werden, nur EMF+‑Datensätze oder nur EMF‑Datensätze. Wenn [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) gesetzt ist, werden EMF+‑Datensätze beim Rendern der Seite geparst, andernfalls werden nur EMF‑Datensätze geparst. Der Standardwert ist [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.

**Remarks**

Nur für .xls, .xlsx, .xlsb und .xlsm-Dateien.

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


Legt die Farbe der Rasterlinien fest.

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

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Gibt an, ob Sie den Fehler beim Rendern ausblenden müssen. Der Fehler kann ein Fehler in Form, Bild, Diagramm-Rendering usw. sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Papiergröße von pagesetup wird ungültig sein, und die anderen Einstellungen von pagesetup bleiben wirksam.

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

Standard ist true.

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

### setPrintingPageType(int value) {#setPrintingPageType-int-}
```
public void setPrintingPageType(int value)
```


Gibt an, welche Seiten nicht gedruckt werden.

Siehe [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Wenn der Inhalt im Blatt spärlich ist, können einige Seiten in der ausgegebenen PDF-Datei völlig leer sein. Wenn Sie diese leeren Seiten nicht möchten, können Sie diese Option verwenden, um sie zu entfernen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRenderingBehavior(int value) {#setRenderingBehavior-int-}
```
public void setRenderingBehavior(int value)
```


Legt die Excel-spezifischen Rendering‑Verhalten fest, die angewendet werden sollen.

Siehe [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

Der Standardwert ist [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\#ALL).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Legt die zu rendernden Arbeitsblätter fest. Standard ist, dass alle sichtbaren Arbeitsblätter in der Arbeitsmappe verwendet werden: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Gibt an, ob die Smart‑Art‑Einstellung aktualisiert wird. Der Standardwert ist false.

**Remarks**

Wirkt nur nach dem Aufruf der Methode Shape.GetResultOfSmartArt() und wenn die zwischengespeicherten Shapes in der Vorlagendatei vorhanden sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

