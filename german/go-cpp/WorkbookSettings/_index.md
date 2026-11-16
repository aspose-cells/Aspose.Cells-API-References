---
title: "WorkbookSettings Klasse"
linktitle: "WorkbookSettings"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "WorkbookSettings Klasse. Kapselt das Objekt, das WorkbookSettings in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/workbooksettings/
---

## WorkbookSettings class

Stellt alle Einstellungen der Arbeitsmappe dar.

```go

type WorkbookSettings struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [Dispose](./dispose/) | Gibt Ressourcen frei. |
| [GetThemeFont](./getthemefont/) | Ermittelt den Namen der Standardschriftart des Themas. |
| [GetAuthor](./getauthor/) | Ermittelt und legt den Autor der Datei fest. |
| [SetAuthor](./setauthor/) | Ermittelt und legt den Autor der Datei fest. |
| [GetCheckCustomNumberFormat](./getcheckcustomnumberformat/) | Gibt an, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat überprüft wird. |
| [SetCheckCustomNumberFormat](./setcheckcustomnumberformat/) | Gibt an, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat überprüft wird. |
| [GetEnableMacros](./getenablemacros/) | Makros aktivieren; |
| [SetEnableMacros](./setenablemacros/) | Makros aktivieren; |
| [GetDate1904](./getdate1904/) | Ermittelt oder legt einen Wert fest, der angibt, ob die Arbeitsmappe das 1904-Datumsystem verwendet. |
| [SetDate1904](./setdate1904/) | Ermittelt oder legt einen Wert fest, der angibt, ob die Arbeitsmappe das 1904-Datumsystem verwendet. |
| [GetProtectionType](./getprotectiontype/) | Ermittelt den Schutztyp der Arbeitsmappe. |
| [GetDisplayDrawingObjects](./getdisplaydrawingobjects/) | Gibt an, ob und wie Objekte in der Arbeitsmappe angezeigt werden. |
| [SetDisplayDrawingObjects](./setdisplaydrawingobjects/) | Gibt an, ob und wie Objekte in der Arbeitsmappe angezeigt werden. |
| [GetSheetTabBarWidth](./getsheettabbarwidth/) | Breite der Arbeitsblatt-Registerkartenleiste (in 1/1000 der Fensterbreite). |
| [SetSheetTabBarWidth](./setsheettabbarwidth/) | Breite der Arbeitsblatt-Registerkartenleiste (in 1/1000 der Fensterbreite). |
| [GetShowTabs](./getshowtabs/) | Ermittelt oder legt einen Wert fest, ob die Arbeitsmappe-Registerkarten angezeigt werden. |
| [SetShowTabs](./setshowtabs/) | Ermittelt oder legt einen Wert fest, ob die Arbeitsmappe-Registerkarten angezeigt werden. |
| [GetFirstVisibleTab](./getfirstvisibletab/) | Ermittelt oder legt die erste sichtbare Arbeitsblatt-Registerkarte fest. |
| [SetFirstVisibleTab](./setfirstvisibletab/) | Ermittelt oder legt die erste sichtbare Arbeitsblatt-Registerkarte fest. |
| [IsHScrollBarVisible](./ishscrollbarvisible/) | Ermittelt oder legt einen Wert fest, der angibt, ob das erzeugte Tabellenblatt eine horizontale Bildlaufleiste enthält. |
| [SetIsHScrollBarVisible](./setishscrollbarvisible/) | Ermittelt oder legt einen Wert fest, der angibt, ob das erzeugte Tabellenblatt eine horizontale Bildlaufleiste enthält. |
| [IsVScrollBarVisible](./isvscrollbarvisible/) | Ermittelt oder legt einen Wert fest, der angibt, ob das erzeugte Tabellenblatt eine vertikale Bildlaufleiste enthält. |
| [SetIsVScrollBarVisible](./setisvscrollbarvisible/) | Ermittelt oder legt einen Wert fest, der angibt, ob das erzeugte Tabellenblatt eine vertikale Bildlaufleiste enthält. |
| [GetShared](./getshared/) | Ermittelt oder legt einen Wert fest, der angibt, ob die Arbeitsmappe freigegeben ist. |
| [SetShared](./setshared/) | Ermittelt oder legt einen Wert fest, der angibt, ob die Arbeitsmappe freigegeben ist. |
| [GetLanguageCode](./getlanguagecode/) | Liest oder setzt die Sprache der Benutzeroberfläche der Arbeitsmappen‑Version basierend auf dem Ländercode, in dem die Datei gespeichert wurde. |
| [SetLanguageCode](./setlanguagecode/) | Liest oder setzt die Sprache der Benutzeroberfläche der Arbeitsmappen‑Version basierend auf dem Ländercode, in dem die Datei gespeichert wurde. |
| [GetRegion](./getregion/) | Liest oder legt die regionalen Einstellungen für die Arbeitsmappe fest. |
| [SetRegion](./setregion/) | Liest oder legt die regionalen Einstellungen für die Arbeitsmappe fest. |
| [GetGlobalizationSettings](./getglobalizationsettings/) | Liest und legt die Globalisierungseinstellungen fest. |
| [SetGlobalizationSettings](./setglobalizationsettings/) | Liest und legt die Globalisierungseinstellungen fest. |
| [GetNumberDecimalSeparator](./getnumberdecimalseparator/) | Liest oder legt das Dezimaltrennzeichen für die Formatierung/Analyse numerischer Werte fest. Standard ist das Dezimaltrennzeichen der aktuellen Region. |
| [SetNumberDecimalSeparator](./setnumberdecimalseparator/) | Liest oder legt das Dezimaltrennzeichen für die Formatierung/Analyse numerischer Werte fest. Standard ist das Dezimaltrennzeichen der aktuellen Region. |
| [GetNumberGroupSeparator](./getnumbergroupseparator/) | Liest oder legt das Zeichen fest, das Gruppen von Ziffern links vom Dezimaltrennzeichen in numerischen Werten trennt. Standard ist das Gruppentrennzeichen der aktuellen Region. |
| [SetNumberGroupSeparator](./setnumbergroupseparator/) | Liest oder legt das Zeichen fest, das Gruppen von Ziffern links vom Dezimaltrennzeichen in numerischen Werten trennt. Standard ist das Gruppentrennzeichen der aktuellen Region. |
| [GetPassword](./getpassword/) | Stellt das Verschlüsselungspasswort der Arbeitsmappendatei dar. |
| [SetPassword](./setpassword/) | Stellt das Verschlüsselungspasswort der Arbeitsmappendatei dar. |
| [GetWriteProtection](./getwriteprotection/) | Bietet Zugriff auf die Schreibschutzoptionen der Arbeitsmappe. |
| [IsEncrypted](./isencrypted/) | Liest einen Wert, der angibt, ob ein Passwort zum Öffnen dieser Arbeitsmappe erforderlich ist. |
| [IsProtected](./isprotected/) | Liest einen Wert, der angibt, ob die Struktur oder das Fenster der Arbeitsmappe geschützt ist. |
| [IsDefaultEncrypted](./isdefaultencrypted/) | Gibt an, ob die Arbeitsmappe mit dem Standardpasswort verschlüsselt wird, wenn Struktur und Fenster der Arbeitsmappe gesperrt sind. |
| [SetIsDefaultEncrypted](./setisdefaultencrypted/) | Gibt an, ob die Arbeitsmappe mit dem Standardpasswort verschlüsselt wird, wenn Struktur und Fenster der Arbeitsmappe gesperrt sind. |
| [IsMinimized](./isminimized/) | Stellt dar, ob die erzeugte Tabelle minimiert geöffnet wird. |
| [SetIsMinimized](./setisminimized/) | Stellt dar, ob die erzeugte Tabelle minimiert geöffnet wird. |
| [IsHidden](./ishidden/) | Gibt an, ob diese Arbeitsmappe ausgeblendet ist. |
| [SetIsHidden](./setishidden/) | Gibt an, ob diese Arbeitsmappe ausgeblendet ist. |
| [GetAutoCompressPictures](./getautocompresspictures/) | Gibt einen booleschen Wert an, der angibt, dass die Anwendung Bilder in der Arbeitsmappe automatisch komprimiert. |
| [SetAutoCompressPictures](./setautocompresspictures/) | Gibt einen booleschen Wert an, der angibt, dass die Anwendung Bilder in der Arbeitsmappe automatisch komprimiert. |
| [GetRemovePersonalInformation](./getremovepersonalinformation/) | Wahr, wenn persönliche Informationen aus der angegebenen Arbeitsmappe entfernt werden können. |
| [SetRemovePersonalInformation](./setremovepersonalinformation/) | Wahr, wenn persönliche Informationen aus der angegebenen Arbeitsmappe entfernt werden können. |
| [GetShapeDisplayType](./getshapedisplaytype/) | Liest und legt fest, wie die Anwendung Formen in dieser Arbeitsmappe darstellt. |
| [SetShapeDisplayType](./setshapedisplaytype/) | Liest und legt fest, wie die Anwendung Formen in dieser Arbeitsmappe darstellt. |
| [GetHidePivotFieldList](./gethidepivotfieldlist/) | Liest und legt fest, ob die Feldliste für die PivotTable ausgeblendet wird. |
| [SetHidePivotFieldList](./sethidepivotfieldlist/) | Liest und legt fest, ob die Feldliste für die PivotTable ausgeblendet wird. |
| [GetMaxUniqueItemsPerField](./getmaxuniqueitemsperfield/) | Liest und legt die Begrenzung eindeutiger Elemente pro Feld fest. |
| [SetMaxUniqueItemsPerField](./setmaxuniqueitemsperfield/) | Liest und legt die Begrenzung eindeutiger Elemente pro Feld fest. |
| [GetUpdateLinksType](./getupdatelinkstype/) | Liest und legt fest, wie externe Links beim Öffnen der Arbeitsmappe aktualisiert werden. |
| [SetUpdateLinksType](./setupdatelinkstype/) | Liest und legt fest, wie externe Links beim Öffnen der Arbeitsmappe aktualisiert werden. |
| [SetPageOrientationType](./setpageorientationtype/) | Legt den Typ der Druckausrichtung für die gesamte Arbeitsmappe fest. |
| [GetMaxRow](./getmaxrow/) | Liest den maximalen Zeilenindex, nullbasiert. |
| [GetMaxColumn](./getmaxcolumn/) | Liest den maximalen Spaltenindex, nullbasiert. |
| [GetSmartTagOptions](./getsmarttagoptions/) | Liest die Optionen des SmartTags. |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | Liest die Einstellungen für Standardwerte von stilbezogenen Eigenschaften dieser Arbeitsmappe. |
| [GetWindowLeft](./getwindowleft/) | Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters, in Punkt. |
| [SetWindowLeft](./setwindowleft/) | Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters, in Punkt. |
| [GetWindowLeftInch](./getwindowleftinch/) | Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters, in Zoll. |
| [SetWindowLeftInch](./setwindowleftinch/) | Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters, in Zoll. |
| [GetWindowLeftCM](./getwindowleftcm/) | Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters, in Zentimetern. |
| [SetWindowLeftCM](./setwindowleftcm/) | Der Abstand von der linken Kante des Clientbereichs zur linken Kante des Fensters, in Zentimetern. |
| [GetWindowTop](./getwindowtop/) | Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters, in der Einheit Punkt. |
| [SetWindowTop](./setwindowtop/) | Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters, in der Einheit Punkt. |
| [GetWindowTopInch](./getwindowtopinch/) | Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters, in der Einheit Zoll. |
| [SetWindowTopInch](./setwindowtopinch/) | Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters, in der Einheit Zoll. |
| [GetWindowTopCM](./getwindowtopcm/) | Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters, in der Einheit Zentimeter. |
| [SetWindowTopCM](./setwindowtopcm/) | Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters, in der Einheit Zentimeter. |
| [GetWindowWidth](./getwindowwidth/) | Die Breite des Fensters, in der Einheit Punkt. |
| [SetWindowWidth](./setwindowwidth/) | Die Breite des Fensters, in der Einheit Punkt. |
| [GetWindowWidthInch](./getwindowwidthinch/) | Die Breite des Fensters, in der Einheit Zoll. |
| [SetWindowWidthInch](./setwindowwidthinch/) | Die Breite des Fensters, in der Einheit Zoll. |
| [GetWindowWidthCM](./getwindowwidthcm/) | Die Breite des Fensters, in der Einheit Zentimeter. |
| [SetWindowWidthCM](./setwindowwidthcm/) | Die Breite des Fensters, in der Einheit Zentimeter. |
| [GetWindowHeight](./getwindowheight/) | Die Höhe des Fensters, in der Einheit Punkt. |
| [SetWindowHeight](./setwindowheight/) | Die Höhe des Fensters, in der Einheit Punkt. |
| [GetWindowHeightInch](./getwindowheightinch/) | Die Höhe des Fensters, in der Einheit Zoll. |
| [SetWindowHeightInch](./setwindowheightinch/) | Die Höhe des Fensters, in der Einheit Zoll. |
| [GetWindowHeightCM](./getwindowheightcm/) | Die Höhe des Fensters, in der Einheit Zentimeter. |
| [SetWindowHeightCM](./setwindowheightcm/) | Die Höhe des Fensters, in der Einheit Zentimeter. |
| [GetUpdateAdjacentCellsBorder](./getupdateadjacentcellsborder/) | Gibt an, ob die Ränder benachbarter Zellen aktualisiert werden. |
| [SetUpdateAdjacentCellsBorder](./setupdateadjacentcellsborder/) | Gibt an, ob die Ränder benachbarter Zellen aktualisiert werden. |
| [GetSignificantDigitsType](./getsignificantdigitstype/) | Liest und setzt den Typ der signifikanten Stellen für die Ausgabe numerischer Werte in dieser Arbeitsmappe. Der Standardwert ist CellsHelper.SignificantDigitsType. |
| [SetSignificantDigitsType](./setsignificantdigitstype/) | Liest und setzt den Typ der signifikanten Stellen für die Ausgabe numerischer Werte in dieser Arbeitsmappe. Der Standardwert ist CellsHelper.SignificantDigitsType. |
| [GetCheckCompatibility](./getcheckcompatibility/) | Gibt an, ob bei der Speicherung der Arbeitsmappe die Kompatibilität mit früheren Versionen geprüft wird. |
| [SetCheckCompatibility](./setcheckcompatibility/) | Gibt an, ob bei der Speicherung der Arbeitsmappe die Kompatibilität mit früheren Versionen geprüft wird. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Ob die Beschränkungen einer Excel‑Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K, etwa mit Cell.PutValue(string), eingeben, erhalten Sie bei true‑Eigenschaft eine Ausnahme. Ist die Eigenschaft false, akzeptieren wir Ihren Eingabe‑Zeichenkettenwert als Zellwert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Ob die Beschränkungen einer Excel‑Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K, etwa mit Cell.PutValue(string), eingeben, erhalten Sie bei true‑Eigenschaft eine Ausnahme. Ist die Eigenschaft false, akzeptieren wir Ihren Eingabe‑Zeichenkettenwert als Zellwert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen. |
| [GetAutoRecover](./getautorecover/) | Gibt an, ob die Datei für die automatische Wiederherstellung markiert ist. |
| [SetAutoRecover](./setautorecover/) | Gibt an, ob die Datei für die automatische Wiederherstellung markiert ist. |
| [GetCrashSave](./getcrashsave/) | Gibt an, ob die Anwendung die Arbeitsmappe nach einem Absturz zuletzt gespeichert hat. |
| [SetCrashSave](./setcrashsave/) | Gibt an, ob die Anwendung die Arbeitsmappe nach einem Absturz zuletzt gespeichert hat. |
| [GetDataExtractLoad](./getdataextractload/) | Gibt an, ob die Anwendung die Arbeitsmappe zuletzt zur Datenwiederherstellung geöffnet hat. |
| [SetDataExtractLoad](./setdataextractload/) | Gibt an, ob die Anwendung die Arbeitsmappe zuletzt zur Datenwiederherstellung geöffnet hat. |
| [GetRepairLoad](./getrepairload/) | Gibt an, ob die Anwendung die Arbeitsmappe zuletzt im sicheren oder Reparaturmodus geöffnet hat. |
| [SetRepairLoad](./setrepairload/) | Gibt an, ob die Anwendung die Arbeitsmappe zuletzt im sicheren oder Reparaturmodus geöffnet hat. |
| [GetBuildVersion](./getbuildversion/) | Gibt die inkrementelle öffentliche Version der Anwendung an. |
| [SetBuildVersion](./setbuildversion/) | Gibt die inkrementelle öffentliche Version der Anwendung an. |
| [GetMemorySetting](./getmemorysetting/) | Liest oder setzt die Optionen zur Speicherverwendung. Die neue Option wird als Standardoption für neu erstellte Arbeitsblätter übernommen, wirkt jedoch nicht für bereits vorhandene Arbeitsblätter. |
| [SetMemorySetting](./setmemorysetting/) | Liest oder setzt die Optionen zur Speicherverwendung. Die neue Option wird als Standardoption für neu erstellte Arbeitsblätter übernommen, wirkt jedoch nicht für bereits vorhandene Arbeitsblätter. |
| [GetPaperSize](./getpapersize/) | Liest und setzt die Standard-Papiergröße für den Druck. |
| [SetPaperSize](./setpapersize/) | Liest und setzt die Standard-Papiergröße für den Druck. |
| [GetMaxRowsOfSharedFormula](./getmaxrowsofsharedformula/) | Liest und setzt die maximale Zeilennummer für geteilte Formeln. |
| [SetMaxRowsOfSharedFormula](./setmaxrowsofsharedformula/) | Liest und setzt die maximale Zeilennummer für geteilte Formeln. |
| [GetCompliance](./getcompliance/) | Gibt die OOXML-Version für das Ausgabedokument an. Der Standardwert ist Ecma376_2006. |
| [SetCompliance](./setcompliance/) | Gibt die OOXML-Version für das Ausgabedokument an. Der Standardwert ist Ecma376_2006. |
| [GetQuotePrefixToStyle](./getquoteprefixtostyle/) | Gibt an, ob beim Eingeben des Zeichenfolgenwerts (der mit einem einfachen Anführungszeichen beginnt) in die Zelle die Eigenschaft Style.QuotePrefix gesetzt wird. |
| [SetQuotePrefixToStyle](./setquoteprefixtostyle/) | Gibt an, ob beim Eingeben des Zeichenfolgenwerts (der mit einem einfachen Anführungszeichen beginnt) in die Zelle die Eigenschaft Style.QuotePrefix gesetzt wird. |
| [GetFormulaSettings](./getformulasettings/) | Liest die Einstellungen für formelbezogene Funktionen. |
| [GetPropertiesFollowChartPoint](./getpropertiesfollowchartpoint/) | Gibt an, ob Datenpunkt-Eigenschaften und Datenbeschriftungen in allen Diagrammen dieser Arbeitsmappe ihrer Referenz folgen. |
| [SetPropertiesFollowChartPoint](./setpropertiesfollowchartpoint/) | Gibt an, ob Datenpunkt-Eigenschaften und Datenbeschriftungen in allen Diagrammen dieser Arbeitsmappe ihrer Referenz folgen. |
| [GetDiscardImageEditData](./getdiscardimageeditdata/) | Gibt an, ob das Verwerfen bearbeiteter Bilddaten erfolgt. |
| [SetDiscardImageEditData](./setdiscardimageeditdata/) | Gibt an, ob das Verwerfen bearbeiteter Bilddaten erfolgt. |
| [GetDefaultImageResolution](./getdefaultimageresolution/) | Liest und setzt die Standardauflösung des Bildes. |
| [SetDefaultImageResolution](./setdefaultimageresolution/) | Liest und setzt die Standardauflösung des Bildes. |
| [GetWpsCompatibility](./getwpscompatibility/) | Gibt an, ob Kompatibilität mit WPS besteht. |
| [SetWpsCompatibility](./setwpscompatibility/) | Gibt an, ob Kompatibilität mit WPS besteht. |
