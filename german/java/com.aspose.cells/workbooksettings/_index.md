---
title: "WorkbookSettings"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt alle Einstellungen der Arbeitsmappe dar."
type: docs
url: /de/java/com.aspose.cells/workbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookSettings
```

Stellt alle Einstellungen der Arbeitsmappe dar.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorkbookSettings settings = workbook.getSettings();
 
         //do your business
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [dispose()](#dispose--) | Gibt Ressourcen frei. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Liefert den Autor der Datei. |
| [getAutoCompressPictures()](#getAutoCompressPictures--) | Gibt einen booleschen Wert an, der angibt, dass die Anwendung Bilder im Arbeitsbuch automatisch komprimiert. |
| [getAutoRecover()](#getAutoRecover--) | Gibt an, ob die Datei für die automatische Wiederherstellung markiert ist. |
| [getBuildVersion()](#getBuildVersion--) | Gibt die inkrementelle öffentliche Version der Anwendung an. |
| [getCheckCompatibility()](#getCheckCompatibility--) | Gibt an, ob die Kompatibilität mit früheren Versionen beim Speichern des Arbeitsbuchs geprüft wird. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Gibt an, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat geprüft wird. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [getClass()](#getClass--) |  |
| [getCompliance()](#getCompliance--) | Gibt die OOXML-Version für das Ausgabedokument an. |
| [getCrashSave()](#getCrashSave--) | Gibt an, ob die Anwendung die Arbeitsbuchdatei nach einem Absturz zuletzt gespeichert hat. |
| [getDataExtractLoad()](#getDataExtractLoad--) | Gibt an, ob die Anwendung das Arbeitsbuch zuletzt zur Datenwiederherstellung geöffnet hat. |
| [getDate1904()](#getDate1904--) | Liefert einen Wert, der angibt, ob das Arbeitsbuch das 1904-Datumsystem verwendet. |
| [getDefaultImageResolution()](#getDefaultImageResolution--) | Liefert die Standardauflösung des Bildes. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Liefert die Einstellungen für Standardwerte von stilbezogenen Eigenschaften dieses Arbeitsbuchs. |
| [getDiscardImageEditData()](#getDiscardImageEditData--) | Gibt an, ob Bilddaten beim Bearbeiten verworfen werden. |
| [getDisplayDrawingObjects()](#getDisplayDrawingObjects--) | Gibt an, ob und wie Objekte im Arbeitsbuch angezeigt werden. |
| [getEnableMacros()](#getEnableMacros--) | Makros aktivieren; |
| [getFirstVisibleTab()](#getFirstVisibleTab--) | Liefert die erste sichtbare Arbeitsblattregisterkarte. |
| [getFormulaSettings()](#getFormulaSettings--) | Liefert die Einstellungen für formelbezogene Funktionen. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Liefert die Globalisierungseinstellungen. |
| [getHidePivotFieldList()](#getHidePivotFieldList--) | Liefert, ob die Feldliste für die PivotTable ausgeblendet wird. |
| [getLanguageCode()](#getLanguageCode--) | Liest die Benutzerschnittstellensprache der Arbeitsmappen‑Version basierend auf dem Ländercode, unter dem die Datei gespeichert wurde. |
| [getLocale()](#getLocale--) | Liefert das von diesem Arbeitsbuch verwendete Gebietsschema. |
| [getMaxColumn()](#getMaxColumn--) | Liefert den maximalen Spaltenindex, nullbasiert. |
| [getMaxRow()](#getMaxRow--) | Liefert den maximalen Zeilenindex, nullbasiert. |
| [getMaxRowsOfSharedFormula()](#getMaxRowsOfSharedFormula--) | Liefert die maximale Zeilennummer der gemeinsam genutzten Formel. |
| [getMaxUniqueItemsPerField()](#getMaxUniqueItemsPerField--) | Ermittelt die Begrenzung eindeutiger Elemente pro Feld |
| [getMemorySetting()](#getMemorySetting--) | Ermittelt die Optionen zur Speichernutzung. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Ermittelt das Dezimaltrennzeichen für die Formatierung/Analyse numerischer Werte. |
| [getNumberGroupSeparator()](#getNumberGroupSeparator--) | Ermittelt das Zeichen, das Gruppen von Ziffern links vom Dezimalpunkt in numerischen Werten trennt. |
| [getPaperSize()](#getPaperSize--) | Ermittelt die Standard-Papiergröße für den Druck. |
| [getPassword()](#getPassword--) | Stellt das Verschlüsselungspasswort der Arbeitsmappendatei dar. |
| [getPropertiesFollowChartPoint()](#getPropertiesFollowChartPoint--) | Gibt an, ob Datenpunkt-Eigenschaften und Datenbeschriftungen in allen Diagrammen dieser Arbeitsmappe ihrer Referenz folgen. |
| [getProtectionType()](#getProtectionType--) | Ermittelt den Schutztyp der Arbeitsmappe. |
| [getQuotePrefixToStyle()](#getQuotePrefixToStyle--) | Gibt an, ob das Festlegen der Eigenschaft [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) beim Eingeben des Zeichenfolgenwerts (der mit einem einfachen Anführungszeichen beginnt) in die Zelle |
| [getRegion()](#getRegion--) | Ermittelt die regionalen Einstellungen für die Arbeitsmappe. |
| [getRemovePersonalInformation()](#getRemovePersonalInformation--) | True, wenn persönliche Informationen aus der angegebenen Arbeitsmappe entfernt werden können. |
| [getRepairLoad()](#getRepairLoad--) | Gibt an, ob die Anwendung die Arbeitsmappe zuletzt im sicheren oder Reparaturmodus geöffnet hat. |
| [getResourceProvider()](#getResourceProvider--) | Ermittelt den Stream-Anbieter für externe Ressourcen, z. B. das Laden von Bilddaten für ein Bild vom Typ "LinkToFile". |
| [getShapeDisplayType()](#getShapeDisplayType--) | Ermittelt, wie die Anwendung Formen in dieser Arbeitsmappe darstellt. |
| [getShared()](#getShared--) | Ermittelt einen Wert, der angibt, ob die Arbeitsmappe freigegeben ist. |
| [getSheetTabBarWidth()](#getSheetTabBarWidth--) | Breite der Arbeitsblatt-Registerkartenleiste (in 1/1000 der Fensterbreite). |
| [getShowTabs()](#getShowTabs--) | Ermittelt einen Wert, ob die Arbeitsmappe-Registerkarten angezeigt werden. |
| [getSignificantDigits()](#getSignificantDigits--) | Ermittelt die Anzahl signifikanter Stellen. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Ermittelt den Typ signifikanter Stellen für die Ausgabe numerischer Werte in dieser Arbeitsmappe. |
| [getSmartTagOptions()](#getSmartTagOptions--) | Ermittelt die Optionen des SmartTags. |
| [getStreamProvider()](#getStreamProvider--) | Ermittelt den Stream-Anbieter für externe Ressourcen. |
| [getThemeFont(int type)](#getThemeFont-int-) | Ermittelt den Standard-Schriftartnamen des Themas. |
| [getUpdateAdjacentCellsBorder()](#getUpdateAdjacentCellsBorder--) | Gibt an, ob die Rahmen angrenzender Zellen aktualisiert werden. |
| [getUpdateLinksType()](#getUpdateLinksType--) | Ermittelt, wie externe Links beim Öffnen der Arbeitsmappe aktualisiert werden. |
| [getWarningCallback()](#getWarningCallback--) | Liest den Warn‑Callback. |
| [getWindowHeight()](#getWindowHeight--) | Die Höhe des Fensters in Punkt. |
| [getWindowHeightCM()](#getWindowHeightCM--) | Die Höhe des Fensters in Zentimeter. |
| [getWindowHeightInch()](#getWindowHeightInch--) | Die Höhe des Fensters, in der Einheit Zoll. |
| [getWindowLeft()](#getWindowLeft--) | Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters, in der Einheit Punkt. |
| [getWindowLeftCM()](#getWindowLeftCM--) | Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters. |
| [getWindowLeftInch()](#getWindowLeftInch--) | Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters. |
| [getWindowTop()](#getWindowTop--) | Der Abstand von der oberen Kante des Clientbereichs zur oberen Kante des Fensters, in der Einheit Punkt. |
| [getWindowTopCM()](#getWindowTopCM--) | Der Abstand von der oberen Kante des Clientbereichs zur oberen Kante des Fensters, in der Einheit Zentimeter. |
| [getWindowTopInch()](#getWindowTopInch--) | Der Abstand von der oberen Kante des Clientbereichs zur oberen Kante des Fensters, in der Einheit Zoll. |
| [getWindowWidth()](#getWindowWidth--) | Die Breite des Fensters, in der Einheit Punkt. |
| [getWindowWidthCM()](#getWindowWidthCM--) | Die Breite des Fensters, in der Einheit Zentimeter. |
| [getWindowWidthInch()](#getWindowWidthInch--) | Die Breite des Fensters, in der Einheit Zoll. |
| [getWpsCompatibility()](#getWpsCompatibility--) | Gibt an, ob Kompatibilität mit WPS besteht. |
| [getWriteProtection()](#getWriteProtection--) | Stellt Zugriff auf die Schreibschutzoptionen der Arbeitsmappe bereit. |
| [hashCode()](#hashCode--) |  |
| [isDefaultEncrypted()](#isDefaultEncrypted--) | Gibt an, ob die Arbeitsmappe mit dem Standardkennwort verschlüsselt wird, wenn Struktur und Fenster der Arbeitsmappe gesperrt sind. |
| [isEncrypted()](#isEncrypted--) | Ermittelt einen Wert, der angibt, ob ein Kennwort zum Öffnen dieser Arbeitsmappe erforderlich ist. |
| [isHScrollBarVisible()](#isHScrollBarVisible--) | Ermittelt einen Wert, der angibt, ob das erzeugte Tabellenblatt eine horizontale Bildlaufleiste enthält. |
| [isHidden()](#isHidden--) | Gibt an, ob diese Arbeitsmappe ausgeblendet ist. |
| [isMinimized()](#isMinimized--) | Gibt an, ob das erzeugte Tabellenblatt minimiert geöffnet wird. |
| [isProtected()](#isProtected--) | Ermittelt einen Wert, der angibt, ob die Struktur oder das Fenster der Arbeitsmappe geschützt ist. |
| [isVScrollBarVisible()](#isVScrollBarVisible--) | Ermittelt einen Wert, der angibt, ob das erzeugte Tabellenblatt eine vertikale Bildlaufleiste enthält. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Legt den Autor der Datei fest. |
| [setAutoCompressPictures(boolean value)](#setAutoCompressPictures-boolean-) | Gibt einen booleschen Wert an, der angibt, dass die Anwendung Bilder im Arbeitsbuch automatisch komprimiert. |
| [setAutoRecover(boolean value)](#setAutoRecover-boolean-) | Gibt an, ob die Datei für die automatische Wiederherstellung markiert ist. |
| [setBuildVersion(String value)](#setBuildVersion-java.lang.String-) | Gibt die inkrementelle öffentliche Version der Anwendung an. |
| [setCheckCompatibility(boolean value)](#setCheckCompatibility-boolean-) | Gibt an, ob die Kompatibilität mit früheren Versionen beim Speichern des Arbeitsbuchs geprüft wird. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Gibt an, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat geprüft wird. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [setCompliance(int value)](#setCompliance-int-) | Gibt die OOXML-Version für das Ausgabedokument an. |
| [setCrashSave(boolean value)](#setCrashSave-boolean-) | Gibt an, ob die Anwendung die Arbeitsbuchdatei nach einem Absturz zuletzt gespeichert hat. |
| [setDataExtractLoad(boolean value)](#setDataExtractLoad-boolean-) | Gibt an, ob die Anwendung das Arbeitsbuch zuletzt zur Datenwiederherstellung geöffnet hat. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Legt einen Wert fest, der angibt, ob die Arbeitsmappe das 1904-Datumsystem verwendet. |
| [setDefaultEncrypted(boolean value)](#setDefaultEncrypted-boolean-) | Gibt an, ob die Arbeitsmappe mit dem Standardkennwort verschlüsselt wird, wenn Struktur und Fenster der Arbeitsmappe gesperrt sind. |
| [setDefaultImageResolution(int value)](#setDefaultImageResolution-int-) | Legt die Standardauflösung des Bildes fest. |
| [setDiscardImageEditData(boolean value)](#setDiscardImageEditData-boolean-) | Gibt an, ob Bilddaten beim Bearbeiten verworfen werden. |
| [setDisplayDrawingObjects(int value)](#setDisplayDrawingObjects-int-) | Gibt an, ob und wie Objekte im Arbeitsbuch angezeigt werden. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Makros aktivieren; |
| [setFirstVisibleTab(int value)](#setFirstVisibleTab-int-) | Legt die erste sichtbare Arbeitsblattregisterkarte fest. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-) | Legt die Globalisierungseinstellungen fest. |
| [setHScrollBarVisible(boolean value)](#setHScrollBarVisible-boolean-) | Legt einen Wert fest, der angibt, ob das erzeugte Tabellenblatt eine horizontale Bildlaufleiste enthält. |
| [setHidden(boolean value)](#setHidden-boolean-) | Gibt an, ob diese Arbeitsmappe ausgeblendet ist. |
| [setHidePivotFieldList(boolean value)](#setHidePivotFieldList-boolean-) | Legt fest, ob die Feldliste für die PivotTable ausgeblendet wird. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Legt die Sprache der Benutzeroberfläche der Arbeitsmappen‑Version basierend auf dem CountryCode fest, mit dem die Datei gespeichert wurde. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Legt das von dieser Arbeitsmappe verwendete Gebietsschema fest. |
| [setMaxRowsOfSharedFormula(int value)](#setMaxRowsOfSharedFormula-int-) | Legt die maximale Zeilenzahl für gemeinsam genutzte Formeln fest. |
| [setMaxUniqueItemsPerField(int value)](#setMaxUniqueItemsPerField-int-) | Legt die Begrenzung eindeutiger Elemente pro Feld fest |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Legt die Optionen zur Speicherverwendung fest. |
| [setMinimized(boolean value)](#setMinimized-boolean-) | Gibt an, ob das erzeugte Tabellenblatt minimiert geöffnet wird. |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Legt das Dezimaltrennzeichen für das Formatieren/Parsen numerischer Werte fest. |
| [setNumberGroupSeparator(char value)](#setNumberGroupSeparator-char-) | Legt das Zeichen fest, das Gruppen von Ziffern links vom Dezimalzeichen in numerischen Werten trennt. |
| [setPageOrientationType(int pageOrientationType)](#setPageOrientationType-int-) | Legt den Typ der Druckausrichtung für die gesamte Arbeitsmappe fest. |
| [setPaperSize(int value)](#setPaperSize-int-) | Legt die standardmäßige Druckpapiergröße fest. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Stellt das Verschlüsselungspasswort der Arbeitsmappendatei dar. |
| [setPropertiesFollowChartPoint(boolean value)](#setPropertiesFollowChartPoint-boolean-) | Gibt an, ob Datenpunkt-Eigenschaften und Datenbeschriftungen in allen Diagrammen dieser Arbeitsmappe ihrer Referenz folgen. |
| [setQuotePrefixToStyle(boolean value)](#setQuotePrefixToStyle-boolean-) | Gibt an, ob das Festlegen der Eigenschaft [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) beim Eingeben des Zeichenfolgenwerts (der mit einem einfachen Anführungszeichen beginnt) in die Zelle |
| [setRegion(int value)](#setRegion-int-) | Legt die regionalen Einstellungen für die Arbeitsmappe fest. |
| [setRemovePersonalInformation(boolean value)](#setRemovePersonalInformation-boolean-) | True, wenn persönliche Informationen aus der angegebenen Arbeitsmappe entfernt werden können. |
| [setRepairLoad(boolean value)](#setRepairLoad-boolean-) | Gibt an, ob die Anwendung die Arbeitsmappe zuletzt im sicheren oder Reparaturmodus geöffnet hat. |
| [setResourceProvider(IStreamProvider value)](#setResourceProvider-com.aspose.cells.IStreamProvider-) | Legt den Stream‑Provider für externe Ressourcen fest, z. B. das Laden von Bilddaten für ein Bild vom Typ "LinkToFile". |
| [setShapeDisplayType(int value)](#setShapeDisplayType-int-) | Legt fest, wie die Anwendung Formen in dieser Arbeitsmappe darstellt |
| [setShared(boolean value)](#setShared-boolean-) | Legt einen Wert fest, der angibt, ob die Arbeitsmappe freigegeben ist. |
| [setSheetTabBarWidth(int value)](#setSheetTabBarWidth-int-) | Breite der Arbeitsblatt-Registerkartenleiste (in 1/1000 der Fensterbreite). |
| [setShowTabs(boolean value)](#setShowTabs-boolean-) | Legt einen Wert fest, ob die Registerkarten der Arbeitsmappe angezeigt werden. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Legt die Anzahl signifikanter Stellen fest. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Legt den Typ der signifikanten Stellen für die Ausgabe numerischer Werte in dieser Arbeitsmappe fest. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Legt den Stream‑Provider für externe Ressourcen fest. |
| [setUpdateAdjacentCellsBorder(boolean value)](#setUpdateAdjacentCellsBorder-boolean-) | Gibt an, ob die Rahmen angrenzender Zellen aktualisiert werden. |
| [setUpdateLinksType(int value)](#setUpdateLinksType-int-) | Legt fest, wie externe Links beim Öffnen der Arbeitsmappe aktualisiert werden. |
| [setVScrollBarVisible(boolean value)](#setVScrollBarVisible-boolean-) | Legt einen Wert fest, der angibt, ob das erzeugte Tabellenblatt eine vertikale Bildlaufleiste enthält. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Legt die Warn‑Callback‑Funktion fest. |
| [setWindowHeight(double value)](#setWindowHeight-double-) | Die Höhe des Fensters in Punkt. |
| [setWindowHeightCM(double value)](#setWindowHeightCM-double-) | Die Höhe des Fensters in Zentimeter. |
| [setWindowHeightInch(double value)](#setWindowHeightInch-double-) | Die Höhe des Fensters, in der Einheit Zoll. |
| [setWindowLeft(double value)](#setWindowLeft-double-) | Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters, in der Einheit Punkt. |
| [setWindowLeftCM(double value)](#setWindowLeftCM-double-) | Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters. |
| [setWindowLeftInch(double value)](#setWindowLeftInch-double-) | Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters. |
| [setWindowTop(double value)](#setWindowTop-double-) | Der Abstand von der oberen Kante des Clientbereichs zur oberen Kante des Fensters, in der Einheit Punkt. |
| [setWindowTopCM(double value)](#setWindowTopCM-double-) | Der Abstand von der oberen Kante des Clientbereichs zur oberen Kante des Fensters, in der Einheit Zentimeter. |
| [setWindowTopInch(double value)](#setWindowTopInch-double-) | Der Abstand von der oberen Kante des Clientbereichs zur oberen Kante des Fensters, in der Einheit Zoll. |
| [setWindowWidth(double value)](#setWindowWidth-double-) | Die Breite des Fensters, in der Einheit Punkt. |
| [setWindowWidthCM(double value)](#setWindowWidthCM-double-) | Die Breite des Fensters, in der Einheit Zentimeter. |
| [setWindowWidthInch(double value)](#setWindowWidthInch-double-) | Die Breite des Fensters, in der Einheit Zoll. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | Gibt an, ob Kompatibilität mit WPS besteht. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### dispose() {#dispose--}
```
public void dispose()
```


Gibt Ressourcen frei.

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Liefert den Autor der Datei.

**Remarks**

Es ist nicht gesetzt, prüfen Sie zuerst [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\\#getAuthor--), dann prüfen Sie den Benutzer der Umgebung.

**Returns:**
java.lang.String
### getAutoCompressPictures() {#getAutoCompressPictures--}
```
public boolean getAutoCompressPictures()
```


Gibt einen booleschen Wert an, der angibt, dass die Anwendung Bilder im Arbeitsbuch automatisch komprimiert.

**Returns:**
boolean
### getAutoRecover() {#getAutoRecover--}
```
public boolean getAutoRecover()
```


Gibt an, ob die Datei für die automatische Wiederherstellung markiert ist.

**Returns:**
boolean
### getBuildVersion() {#getBuildVersion--}
```
public String getBuildVersion()
```


Gibt die inkrementelle öffentliche Version der Anwendung an.

**Returns:**
java.lang.String
### getCheckCompatibility() {#getCheckCompatibility--}
```
public boolean getCheckCompatibility()
```


Gibt an, ob die Kompatibilität mit früheren Versionen beim Speichern des Arbeitsbuchs geprüft wird.

**Remarks**

Der Standardwert ist true. Nur für Excel97-2003 xls- oder xlt-Dateien.

**Returns:**
boolean
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Gibt an, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat geprüft wird.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Ob die Beschränkungen der Excel‑Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht das Eingeben eines Zeichenkettenwertes, der länger als 32 KB ist. Wenn Sie einen Wert länger als 32 KB, etwa über Cell.PutValue(string), eingeben und diese Eigenschaft true ist, erhalten Sie eine Ausnahme. Ist die Eigenschaft false, akzeptieren wir den eingegebenen Zeichenkettenwert als Zellenwert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festgelegt haben, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Gibt die OOXML-Version für das Ausgabedokument an. Der Standardwert ist Ecma376\\_2006.

Siehe [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Nur für .xlsx-Dateien.

**Returns:**
int
### getCrashSave() {#getCrashSave--}
```
public boolean getCrashSave()
```


Gibt an, ob die Anwendung die Arbeitsbuchdatei nach einem Absturz zuletzt gespeichert hat.

**Returns:**
boolean
### getDataExtractLoad() {#getDataExtractLoad--}
```
public boolean getDataExtractLoad()
```


Gibt an, ob die Anwendung das Arbeitsbuch zuletzt zur Datenwiederherstellung geöffnet hat.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Liefert einen Wert, der angibt, ob das Arbeitsbuch das 1904-Datumsystem verwendet.

**Returns:**
boolean
### getDefaultImageResolution() {#getDefaultImageResolution--}
```
public int getDefaultImageResolution()
```


Liefert die Standardauflösung des Bildes.

**Returns:**
int
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Liefert die Einstellungen für Standardwerte von stilbezogenen Eigenschaften dieses Arbeitsbuchs.

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getDiscardImageEditData() {#getDiscardImageEditData--}
```
public boolean getDiscardImageEditData()
```


Gibt an, ob Bilddaten beim Bearbeiten verworfen werden.

**Returns:**
boolean
### getDisplayDrawingObjects() {#getDisplayDrawingObjects--}
```
public int getDisplayDrawingObjects()
```


Gibt an, ob und wie Objekte im Arbeitsbuch angezeigt werden.

Siehe [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Returns:**
int
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Makros aktivieren;

**Remarks**

Jetzt funktioniert es nur, wenn ein Arbeitsblatt in ein anderes Arbeitsblatt einer Arbeitsmappe kopiert wird.

**Returns:**
boolean
### getFirstVisibleTab() {#getFirstVisibleTab--}
```
public int getFirstVisibleTab()
```


Liefert die erste sichtbare Arbeitsblattregisterkarte.

**Returns:**
int
### getFormulaSettings() {#getFormulaSettings--}
```
public FormulaSettings getFormulaSettings()
```


Liefert die Einstellungen für formelbezogene Funktionen.

**Returns:**
[FormulaSettings](../../com.aspose.cells/formulasettings)
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public GlobalizationSettings getGlobalizationSettings()
```


Liefert die Globalisierungseinstellungen.

**Returns:**
[GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
### getHidePivotFieldList() {#getHidePivotFieldList--}
```
public boolean getHidePivotFieldList()
```


Liefert, ob die Feldliste für die PivotTable ausgeblendet wird.

**Returns:**
boolean
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Liest die Benutzerschnittstellensprache der Arbeitsmappen‑Version basierend auf dem Ländercode, unter dem die Datei gespeichert wurde.

Siehe [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Liefert das von diesem Arbeitsbuch verwendete Gebietsschema.

**Remarks**

Gibt null zurück, wenn weder Locale noch [getRegion()](../../com.aspose.cells/workbooksettings\\#getRegion--) gesetzt ist.

**Returns:**
java.util.Locale
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Liefert den maximalen Spaltenindex, nullbasiert.

**Remarks**

Gibt 255 zurück, wenn das Dateiformat Excel97-2003 ist;

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Liefert den maximalen Zeilenindex, nullbasiert.

**Remarks**

Gibt 65535 zurück, wenn das Dateiformat Excel97-2003 ist;

**Returns:**
int
### getMaxRowsOfSharedFormula() {#getMaxRowsOfSharedFormula--}
```
public int getMaxRowsOfSharedFormula()
```


Liefert die maximale Zeilennummer der gemeinsam genutzten Formel.

**Remarks**

Wenn die Zahl zu groß ist, arbeitet der Autofilter in MS Excel 2013 sehr langsam.

**Returns:**
int
### getMaxUniqueItemsPerField() {#getMaxUniqueItemsPerField--}
```
public int getMaxUniqueItemsPerField()
```


Ermittelt die Begrenzung eindeutiger Elemente pro Feld

**Remarks**

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Liest die Optionen zur Speicherverwendung. Die neue Option wird als Standardoption für neu erstellte Arbeitsblätter verwendet, wirkt sich jedoch nicht auf bereits vorhandene Arbeitsblätter aus.

Siehe [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Weitere Details zum Speichermodus finden Sie unter [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Liest das Dezimaltrennzeichen für die Formatierung/Analyse numerischer Werte. Standard ist das Dezimaltrennzeichen der aktuellen Region.

**Returns:**
char
### getNumberGroupSeparator() {#getNumberGroupSeparator--}
```
public char getNumberGroupSeparator()
```


Liest das Zeichen, das Gruppen von Ziffern links vom Dezimalpunkt in numerischen Werten trennt. Standard ist das Gruppentrennzeichen der aktuellen Region.

**Returns:**
char
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Ermittelt die Standard-Papiergröße für den Druck.

Siehe [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

Wenn keine Einstellung für die Papiergröße vorhanden ist, verwendet MS Excel die Standardeinstellung des Druckers.

**Returns:**
int
### getPassword() {#getPassword--}
```
public String getPassword()
```


Stellt das Verschlüsselungspasswort der Arbeitsmappendatei dar.

**Returns:**
java.lang.String
### getPropertiesFollowChartPoint() {#getPropertiesFollowChartPoint--}
```
public boolean getPropertiesFollowChartPoint()
```


Gibt an, ob Datenpunkt-Eigenschaften und Datenbeschriftungen in allen Diagrammen dieser Arbeitsmappe ihrer Referenz folgen.

**Returns:**
boolean
### getProtectionType() {#getProtectionType--}
```
public int getProtectionType()
```


Ermittelt den Schutztyp der Arbeitsmappe.

Siehe [ProtectionType](../../com.aspose.cells/protectiontype).

**Returns:**
int
### getQuotePrefixToStyle() {#getQuotePrefixToStyle--}
```
public boolean getQuotePrefixToStyle()
```


Gibt an, ob das Festlegen der Eigenschaft [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) beim Eingeben des Zeichenfolgenwerts (der mit einem einfachen Anführungszeichen beginnt) in die Zelle

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Ermittelt die regionalen Einstellungen für die Arbeitsmappe.

Siehe [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Regionaleinstellungen, die von der Aspose.Cells‑Komponente für eine Arbeitsmappe verwendet werden, die aus einer Vorlagendatei geladen wurde: i). Für eine XLS‑Datei gibt es Felder für regionale Einstellungen, und MS Excel speichert regionale Einstellungsdaten beim Speichern der XLS‑Datei. Daher verwenden wir die im Vorlagendatei gespeicherte Region für die Arbeitsmappe. Wenn Sie die in der XLS‑Datei gespeicherte Region nicht verwenden möchten, setzen Sie sie nach dem Laden der Vorlagendatei auf die gewünschte (z. B. CountryCode.Default) zurück. Und wir speichern den vom Benutzer angegebenen Wert (mit dieser Methode) ebenfalls beim Speichern einer XLS‑Datei in die Datei. ii). Für andere Dateiformate, wie XLSX, XLSB usw., ist im Dateiformatspezifikation kein Feld für regionale Einstellungen definiert. Daher verwenden wir die regionalen Einstellungen der Anwendungsumgebung für die Arbeitsmappe. Der vom Benutzer angegebene Wert (mit dieser Methode) kann für die erzeugten Dateien dieser Formate nicht beibehalten werden. 2. Für die Anzeige in MS Excel: Die hier angewendeten regionalen Einstellungen wirken nur zur Laufzeit mit der Aspose.Cells‑Komponente und nicht beim Betrachten der erzeugten Datei mit MS Excel. Selbst bei einer erzeugten XLS‑Datei, in der die angegebenen regionalen Einstellungsdaten gespeichert wurden, wird beim Betrachten/Bearbeiten mit MS Excel die von MS Excel zur Formatierung verwendete Region stets die Standard‑Regionseinstellungen der Umgebung sein, in der MS Excel läuft, und nicht die in der Datei gespeicherte. Das ist das Verhalten von MS Excel und kann nicht durch Code geändert werden.

**Returns:**
int
### getRemovePersonalInformation() {#getRemovePersonalInformation--}
```
public boolean getRemovePersonalInformation()
```


True, wenn persönliche Informationen aus der angegebenen Arbeitsmappe entfernt werden können.

**Remarks**

**Returns:**
boolean
### getRepairLoad() {#getRepairLoad--}
```
public boolean getRepairLoad()
```


Gibt an, ob die Anwendung die Arbeitsmappe zuletzt im sicheren oder Reparaturmodus geöffnet hat.

**Returns:**
boolean
### getResourceProvider() {#getResourceProvider--}
```
public IStreamProvider getResourceProvider()
```


Ermittelt den Stream-Anbieter für externe Ressourcen, z. B. das Laden von Bilddaten für ein Bild vom Typ "LinkToFile".

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getShapeDisplayType() {#getShapeDisplayType--}
```
public int getShapeDisplayType()
```


Ermittelt, wie die Anwendung Formen in dieser Arbeitsmappe darstellt.

Siehe [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Returns:**
int
### getShared() {#getShared--}
```
public boolean getShared()
```


Ermittelt einen Wert, der angibt, ob die Arbeitsmappe freigegeben ist.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
### getSheetTabBarWidth() {#getSheetTabBarWidth--}
```
public int getSheetTabBarWidth()
```


Breite der Arbeitsblatt-Registerkartenleiste (in 1/1000 der Fensterbreite).

**Returns:**
int
### getShowTabs() {#getShowTabs--}
```
public boolean getShowTabs()
```


Ermittelt einen Wert, ob die Arbeitsmappe-Registerkarten angezeigt werden.

**Remarks**

Der Standardwert ist true.

**Example**

Der folgende Code blendet die Blattregisterkarten und die Bildlauf‑Schaltflächen für das Tabellenblatt aus.

```
         // Hide the spreadsheet tabs.
         workbook.getSettings().setShowTabs(false);
```

**Returns:**
boolean
### getSignificantDigits() {#getSignificantDigits--}
```
public int getSignificantDigits()
```


Liest die Anzahl signifikanter Stellen. Der Standardwert ist [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Kann jetzt nur 15 oder 17 sein. HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). Diese Eigenschaft wird 12 Monate nach Juni 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public int getSignificantDigitsType()
```


Liest den Typ signifikanter Stellen für die Ausgabe numerischer Werte in dieser Arbeitsmappe. Der Standardwert ist [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

Siehe [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getSmartTagOptions() {#getSmartTagOptions--}
```
public SmartTagOptions getSmartTagOptions()
```


Ermittelt die Optionen des SmartTags.

**Returns:**
[SmartTagOptions](../../com.aspose.cells/smarttagoptions)
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Ermittelt den Stream-Anbieter für externe Ressourcen.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die ResourceProvider‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Juni 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getThemeFont(int type) {#getThemeFont-int-}
```
public String getThemeFont(int type)
```


Ermittelt den Standard-Schriftartnamen des Themas.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). Der Schematyp der Schriftart. |

**Returns:**
java.lang.String -
### getUpdateAdjacentCellsBorder() {#getUpdateAdjacentCellsBorder--}
```
public boolean getUpdateAdjacentCellsBorder()
```


Gibt an, ob die Rahmen angrenzender Zellen aktualisiert werden.

**Remarks**

Der Standardwert ist false. Zum Beispiel: Der untere Rand der Zelle A1 wird aktualisiert, der obere Rand der Zelle A2 sollte ebenfalls geändert werden.

**Returns:**
boolean
### getUpdateLinksType() {#getUpdateLinksType--}
```
public int getUpdateLinksType()
```


Ermittelt, wie externe Links beim Öffnen der Arbeitsmappe aktualisiert werden.

Siehe [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Liest den Warn‑Callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWindowHeight() {#getWindowHeight--}
```
public double getWindowHeight()
```


Die Höhe des Fensters in Punkt.

**Returns:**
double
### getWindowHeightCM() {#getWindowHeightCM--}
```
public double getWindowHeightCM()
```


Die Höhe des Fensters in Zentimeter.

**Returns:**
double
### getWindowHeightInch() {#getWindowHeightInch--}
```
public double getWindowHeightInch()
```


Die Höhe des Fensters, in der Einheit Zoll.

**Returns:**
double
### getWindowLeft() {#getWindowLeft--}
```
public double getWindowLeft()
```


Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters, in der Einheit Punkt.

**Returns:**
double
### getWindowLeftCM() {#getWindowLeftCM--}
```
public double getWindowLeftCM()
```


Der Abstand von der linken Kante des Client‑Bereichs zur linken Kante des Fensters. In Zentimetern.

**Returns:**
double
### getWindowLeftInch() {#getWindowLeftInch--}
```
public double getWindowLeftInch()
```


Der Abstand von der linken Kante des Client‑Bereichs zur linken Kante des Fensters. In Zoll.

**Returns:**
double
### getWindowTop() {#getWindowTop--}
```
public double getWindowTop()
```


Der Abstand von der oberen Kante des Clientbereichs zur oberen Kante des Fensters, in der Einheit Punkt.

**Returns:**
double
### getWindowTopCM() {#getWindowTopCM--}
```
public double getWindowTopCM()
```


Der Abstand von der oberen Kante des Clientbereichs zur oberen Kante des Fensters, in der Einheit Zentimeter.

**Returns:**
double
### getWindowTopInch() {#getWindowTopInch--}
```
public double getWindowTopInch()
```


Der Abstand von der oberen Kante des Clientbereichs zur oberen Kante des Fensters, in der Einheit Zoll.

**Returns:**
double
### getWindowWidth() {#getWindowWidth--}
```
public double getWindowWidth()
```


Die Breite des Fensters, in der Einheit Punkt.

**Returns:**
double
### getWindowWidthCM() {#getWindowWidthCM--}
```
public double getWindowWidthCM()
```


Die Breite des Fensters, in der Einheit Zentimeter.

**Returns:**
double
### getWindowWidthInch() {#getWindowWidthInch--}
```
public double getWindowWidthInch()
```


Die Breite des Fensters, in der Einheit Zoll.

**Returns:**
double
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


Gibt an, ob Kompatibilität mit WPS besteht.

**Returns:**
boolean
### getWriteProtection() {#getWriteProtection--}
```
public WriteProtection getWriteProtection()
```


Stellt Zugriff auf die Schreibschutzoptionen der Arbeitsmappe bereit.

**Returns:**
[WriteProtection](../../com.aspose.cells/writeprotection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDefaultEncrypted() {#isDefaultEncrypted--}
```
public boolean isDefaultEncrypted()
```


Gibt an, ob die Arbeitsmappe mit dem Standardkennwort verschlüsselt wird, wenn Struktur und Fenster der Arbeitsmappe gesperrt sind.

**Remarks**

Der Standardwert ist jetzt false. Er ist derselbe wie bei MS Excel 2013.

**Returns:**
boolean
### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Ermittelt einen Wert, der angibt, ob ein Kennwort zum Öffnen dieser Arbeitsmappe erforderlich ist.

**Returns:**
boolean
### isHScrollBarVisible() {#isHScrollBarVisible--}
```
public boolean isHScrollBarVisible()
```


Ermittelt einen Wert, der angibt, ob das erzeugte Tabellenblatt eine horizontale Bildlaufleiste enthält.

**Remarks**

Der Standardwert ist true.

**Example**

Der folgende Code macht die horizontale Bildlaufleiste für das Tabellenblatt unsichtbar.

```
         // Hide the horizontal scroll bar of the Excel file.
         settings.setHScrollBarVisible(false);
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Gibt an, ob diese Arbeitsmappe ausgeblendet ist.

**Returns:**
boolean
### isMinimized() {#isMinimized--}
```
public boolean isMinimized()
```


Gibt an, ob das erzeugte Tabellenblatt minimiert geöffnet wird.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Ermittelt einen Wert, der angibt, ob die Struktur oder das Fenster der Arbeitsmappe geschützt ist.

**Returns:**
boolean
### isVScrollBarVisible() {#isVScrollBarVisible--}
```
public boolean isVScrollBarVisible()
```


Ermittelt einen Wert, der angibt, ob das erzeugte Tabellenblatt eine vertikale Bildlaufleiste enthält.

**Remarks**

Der Standardwert ist true.

**Example**

Der folgende Code macht die vertikale Bildlaufleiste für das Tabellenblatt unsichtbar.

```
         	// Hide the vertical scroll bar of the Excel file.
         settings.setVScrollBarVisible(false);
```

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Legt den Autor der Datei fest.

**Remarks**

Es ist nicht gesetzt, prüfen Sie zuerst [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\\#getAuthor--), dann prüfen Sie den Benutzer der Umgebung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setAutoCompressPictures(boolean value) {#setAutoCompressPictures-boolean-}
```
public void setAutoCompressPictures(boolean value)
```


Gibt einen booleschen Wert an, der angibt, dass die Anwendung Bilder im Arbeitsbuch automatisch komprimiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAutoRecover(boolean value) {#setAutoRecover-boolean-}
```
public void setAutoRecover(boolean value)
```


Gibt an, ob die Datei für die automatische Wiederherstellung markiert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBuildVersion(String value) {#setBuildVersion-java.lang.String-}
```
public void setBuildVersion(String value)
```


Gibt die inkrementelle öffentliche Version der Anwendung an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCheckCompatibility(boolean value) {#setCheckCompatibility-boolean-}
```
public void setCheckCompatibility(boolean value)
```


Gibt an, ob die Kompatibilität mit früheren Versionen beim Speichern des Arbeitsbuchs geprüft wird.

**Remarks**

Der Standardwert ist true. Nur für Excel97-2003 xls- oder xlt-Dateien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Gibt an, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat geprüft wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Ob die Beschränkungen der Excel‑Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht das Eingeben eines Zeichenkettenwertes, der länger als 32 KB ist. Wenn Sie einen Wert länger als 32 KB, etwa über Cell.PutValue(string), eingeben und diese Eigenschaft true ist, erhalten Sie eine Ausnahme. Ist die Eigenschaft false, akzeptieren wir den eingegebenen Zeichenkettenwert als Zellenwert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festgelegt haben, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Gibt die OOXML-Version für das Ausgabedokument an. Der Standardwert ist Ecma376\\_2006.

Siehe [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Nur für .xlsx-Dateien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCrashSave(boolean value) {#setCrashSave-boolean-}
```
public void setCrashSave(boolean value)
```


Gibt an, ob die Anwendung die Arbeitsbuchdatei nach einem Absturz zuletzt gespeichert hat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDataExtractLoad(boolean value) {#setDataExtractLoad-boolean-}
```
public void setDataExtractLoad(boolean value)
```


Gibt an, ob die Anwendung das Arbeitsbuch zuletzt zur Datenwiederherstellung geöffnet hat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Legt einen Wert fest, der angibt, ob die Arbeitsmappe das 1904-Datumsystem verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDefaultEncrypted(boolean value) {#setDefaultEncrypted-boolean-}
```
public void setDefaultEncrypted(boolean value)
```


Gibt an, ob die Arbeitsmappe mit dem Standardkennwort verschlüsselt wird, wenn Struktur und Fenster der Arbeitsmappe gesperrt sind.

**Remarks**

Der Standardwert ist jetzt false. Er ist derselbe wie bei MS Excel 2013.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDefaultImageResolution(int value) {#setDefaultImageResolution-int-}
```
public void setDefaultImageResolution(int value)
```


Legt die Standardauflösung des Bildes fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDiscardImageEditData(boolean value) {#setDiscardImageEditData-boolean-}
```
public void setDiscardImageEditData(boolean value)
```


Gibt an, ob Bilddaten beim Bearbeiten verworfen werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDisplayDrawingObjects(int value) {#setDisplayDrawingObjects-int-}
```
public void setDisplayDrawingObjects(int value)
```


Gibt an, ob und wie Objekte im Arbeitsbuch angezeigt werden.

Siehe [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Makros aktivieren;

**Remarks**

Jetzt funktioniert es nur, wenn ein Arbeitsblatt in ein anderes Arbeitsblatt einer Arbeitsmappe kopiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFirstVisibleTab(int value) {#setFirstVisibleTab-int-}
```
public void setFirstVisibleTab(int value)
```


Legt die erste sichtbare Arbeitsblattregisterkarte fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-}
```
public void setGlobalizationSettings(GlobalizationSettings value)
```


Legt die Globalisierungseinstellungen fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.cells/globalizationsettings) |  |

### setHScrollBarVisible(boolean value) {#setHScrollBarVisible-boolean-}
```
public void setHScrollBarVisible(boolean value)
```


Legt einen Wert fest, der angibt, ob das erzeugte Tabellenblatt eine horizontale Bildlaufleiste enthält.

**Remarks**

Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Gibt an, ob diese Arbeitsmappe ausgeblendet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHidePivotFieldList(boolean value) {#setHidePivotFieldList-boolean-}
```
public void setHidePivotFieldList(boolean value)
```


Legt fest, ob die Feldliste für die PivotTable ausgeblendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Legt die Sprache der Benutzeroberfläche der Arbeitsmappen‑Version basierend auf dem CountryCode fest, mit dem die Datei gespeichert wurde.

Siehe [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Legt das von dieser Arbeitsmappe verwendete Gebietsschema fest.

**Remarks**

Gibt null zurück, wenn weder Locale noch [getRegion()](../../com.aspose.cells/workbooksettings\\#getRegion--) gesetzt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Locale |  |

### setMaxRowsOfSharedFormula(int value) {#setMaxRowsOfSharedFormula-int-}
```
public void setMaxRowsOfSharedFormula(int value)
```


Legt die maximale Zeilenzahl für gemeinsam genutzte Formeln fest.

**Remarks**

Wenn die Zahl zu groß ist, arbeitet der Autofilter in MS Excel 2013 sehr langsam.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMaxUniqueItemsPerField(int value) {#setMaxUniqueItemsPerField-int-}
```
public void setMaxUniqueItemsPerField(int value)
```


Legt die Begrenzung eindeutiger Elemente pro Feld fest

**Remarks**

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Legt die Optionen zur Speichernutzung fest. Die neue Option wird als Standardoption für neu erstellte Arbeitsblätter übernommen, wirkt jedoch nicht auf bereits vorhandene Arbeitsblätter.

Siehe [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Weitere Details zum Speichermodus finden Sie unter [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMinimized(boolean value) {#setMinimized-boolean-}
```
public void setMinimized(boolean value)
```


Gibt an, ob das erzeugte Tabellenblatt minimiert geöffnet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Legt das Dezimaltrennzeichen für die Formatierung/Analyse numerischer Werte fest. Standard ist das Dezimaltrennzeichen der aktuellen Region.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char |  |

### setNumberGroupSeparator(char value) {#setNumberGroupSeparator-char-}
```
public void setNumberGroupSeparator(char value)
```


Legt das Zeichen fest, das Gruppen von Ziffern links vom Dezimaltrennzeichen in numerischen Werten trennt. Standard ist das Gruppentrennzeichen der aktuellen Region.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char |  |

### setPageOrientationType(int pageOrientationType) {#setPageOrientationType-int-}
```
public void setPageOrientationType(int pageOrientationType)
```


Legt den Typ der Druckausrichtung für die gesamte Arbeitsmappe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageOrientationType | int | [PageOrientationType](../../com.aspose.cells/pageorientationtype). Der Seitenausrichtungstyp |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Legt die standardmäßige Druckpapiergröße fest.

Siehe [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

Wenn keine Einstellung für die Papiergröße vorhanden ist, verwendet MS Excel die Standardeinstellung des Druckers.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Stellt das Verschlüsselungspasswort der Arbeitsmappendatei dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPropertiesFollowChartPoint(boolean value) {#setPropertiesFollowChartPoint-boolean-}
```
public void setPropertiesFollowChartPoint(boolean value)
```


Gibt an, ob Datenpunkt-Eigenschaften und Datenbeschriftungen in allen Diagrammen dieser Arbeitsmappe ihrer Referenz folgen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setQuotePrefixToStyle(boolean value) {#setQuotePrefixToStyle-boolean-}
```
public void setQuotePrefixToStyle(boolean value)
```


Gibt an, ob das Festlegen der Eigenschaft [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) beim Eingeben des Zeichenfolgenwerts (der mit einem einfachen Anführungszeichen beginnt) in die Zelle

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Legt die regionalen Einstellungen für die Arbeitsmappe fest.

Siehe [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Regionaleinstellungen, die von der Aspose.Cells‑Komponente für eine Arbeitsmappe verwendet werden, die aus einer Vorlagendatei geladen wurde: i). Für eine XLS‑Datei gibt es Felder für regionale Einstellungen, und MS Excel speichert regionale Einstellungsdaten beim Speichern der XLS‑Datei. Daher verwenden wir die im Vorlagendatei gespeicherte Region für die Arbeitsmappe. Wenn Sie die in der XLS‑Datei gespeicherte Region nicht verwenden möchten, setzen Sie sie nach dem Laden der Vorlagendatei auf die gewünschte (z. B. CountryCode.Default) zurück. Und wir speichern den vom Benutzer angegebenen Wert (mit dieser Methode) ebenfalls beim Speichern einer XLS‑Datei in die Datei. ii). Für andere Dateiformate, wie XLSX, XLSB usw., ist im Dateiformatspezifikation kein Feld für regionale Einstellungen definiert. Daher verwenden wir die regionalen Einstellungen der Anwendungsumgebung für die Arbeitsmappe. Der vom Benutzer angegebene Wert (mit dieser Methode) kann für die erzeugten Dateien dieser Formate nicht beibehalten werden. 2. Für die Anzeige in MS Excel: Die hier angewendeten regionalen Einstellungen wirken nur zur Laufzeit mit der Aspose.Cells‑Komponente und nicht beim Betrachten der erzeugten Datei mit MS Excel. Selbst bei einer erzeugten XLS‑Datei, in der die angegebenen regionalen Einstellungsdaten gespeichert wurden, wird beim Betrachten/Bearbeiten mit MS Excel die von MS Excel zur Formatierung verwendete Region stets die Standard‑Regionseinstellungen der Umgebung sein, in der MS Excel läuft, und nicht die in der Datei gespeicherte. Das ist das Verhalten von MS Excel und kann nicht durch Code geändert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRemovePersonalInformation(boolean value) {#setRemovePersonalInformation-boolean-}
```
public void setRemovePersonalInformation(boolean value)
```


True, wenn persönliche Informationen aus der angegebenen Arbeitsmappe entfernt werden können.

**Remarks**

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRepairLoad(boolean value) {#setRepairLoad-boolean-}
```
public void setRepairLoad(boolean value)
```


Gibt an, ob die Anwendung die Arbeitsmappe zuletzt im sicheren oder Reparaturmodus geöffnet hat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setResourceProvider(IStreamProvider value) {#setResourceProvider-com.aspose.cells.IStreamProvider-}
```
public void setResourceProvider(IStreamProvider value)
```


Legt den Stream‑Provider für externe Ressourcen fest, z. B. das Laden von Bilddaten für ein Bild vom Typ "LinkToFile".

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setShapeDisplayType(int value) {#setShapeDisplayType-int-}
```
public void setShapeDisplayType(int value)
```


Legt fest, wie die Anwendung Formen in dieser Arbeitsmappe darstellt

Siehe [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setShared(boolean value) {#setShared-boolean-}
```
public void setShared(boolean value)
```


Legt einen Wert fest, der angibt, ob die Arbeitsmappe freigegeben ist.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSheetTabBarWidth(int value) {#setSheetTabBarWidth-int-}
```
public void setSheetTabBarWidth(int value)
```


Breite der Arbeitsblatt-Registerkartenleiste (in 1/1000 der Fensterbreite).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setShowTabs(boolean value) {#setShowTabs-boolean-}
```
public void setShowTabs(boolean value)
```


Legt einen Wert fest, ob die Registerkarten der Arbeitsmappe angezeigt werden.

**Remarks**

Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public void setSignificantDigits(int value)
```


Legt die Anzahl signifikanter Stellen fest. Der Standardwert ist [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Kann jetzt nur 15 oder 17 sein. HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). Diese Eigenschaft wird 12 Monate nach Juni 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public void setSignificantDigitsType(int value)
```


Legt den Typ signifikanter Stellen für die Ausgabe numerischer Werte in dieser Arbeitsmappe fest. Der Standardwert ist [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

Siehe [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Legt den Stream‑Provider für externe Ressourcen fest.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die ResourceProvider‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Juni 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setUpdateAdjacentCellsBorder(boolean value) {#setUpdateAdjacentCellsBorder-boolean-}
```
public void setUpdateAdjacentCellsBorder(boolean value)
```


Gibt an, ob die Rahmen angrenzender Zellen aktualisiert werden.

**Remarks**

Der Standardwert ist false. Zum Beispiel: Der untere Rand der Zelle A1 wird aktualisiert, der obere Rand der Zelle A2 sollte ebenfalls geändert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setUpdateLinksType(int value) {#setUpdateLinksType-int-}
```
public void setUpdateLinksType(int value)
```


Legt fest, wie externe Links beim Öffnen der Arbeitsmappe aktualisiert werden.

Siehe [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setVScrollBarVisible(boolean value) {#setVScrollBarVisible-boolean-}
```
public void setVScrollBarVisible(boolean value)
```


Legt einen Wert fest, der angibt, ob das erzeugte Tabellenblatt eine vertikale Bildlaufleiste enthält.

**Remarks**

Der Standardwert ist true.

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

### setWindowHeight(double value) {#setWindowHeight-double-}
```
public void setWindowHeight(double value)
```


Die Höhe des Fensters in Punkt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWindowHeightCM(double value) {#setWindowHeightCM-double-}
```
public void setWindowHeightCM(double value)
```


Die Höhe des Fensters in Zentimeter.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWindowHeightInch(double value) {#setWindowHeightInch-double-}
```
public void setWindowHeightInch(double value)
```


Die Höhe des Fensters, in der Einheit Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWindowLeft(double value) {#setWindowLeft-double-}
```
public void setWindowLeft(double value)
```


Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters, in der Einheit Punkt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWindowLeftCM(double value) {#setWindowLeftCM-double-}
```
public void setWindowLeftCM(double value)
```


Der Abstand von der linken Kante des Client‑Bereichs zur linken Kante des Fensters. In Zentimetern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWindowLeftInch(double value) {#setWindowLeftInch-double-}
```
public void setWindowLeftInch(double value)
```


Der Abstand von der linken Kante des Client‑Bereichs zur linken Kante des Fensters. In Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWindowTop(double value) {#setWindowTop-double-}
```
public void setWindowTop(double value)
```


Der Abstand von der oberen Kante des Clientbereichs zur oberen Kante des Fensters, in der Einheit Punkt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWindowTopCM(double value) {#setWindowTopCM-double-}
```
public void setWindowTopCM(double value)
```


Der Abstand von der oberen Kante des Clientbereichs zur oberen Kante des Fensters, in der Einheit Zentimeter.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWindowTopInch(double value) {#setWindowTopInch-double-}
```
public void setWindowTopInch(double value)
```


Der Abstand von der oberen Kante des Clientbereichs zur oberen Kante des Fensters, in der Einheit Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWindowWidth(double value) {#setWindowWidth-double-}
```
public void setWindowWidth(double value)
```


Die Breite des Fensters, in der Einheit Punkt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWindowWidthCM(double value) {#setWindowWidthCM-double-}
```
public void setWindowWidthCM(double value)
```


Die Breite des Fensters, in der Einheit Zentimeter.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWindowWidthInch(double value) {#setWindowWidthInch-double-}
```
public void setWindowWidthInch(double value)
```


Die Breite des Fensters, in der Einheit Zoll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


Gibt an, ob Kompatibilität mit WPS besteht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

