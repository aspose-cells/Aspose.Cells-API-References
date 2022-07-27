---
title: WorkbookSettings
second_title: Aspose.Cells für .NET-API-Referenz
description: Stellt alle Einstellungen der Arbeitsmappe dar.
type: docs
weight: 6500
url: /de/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

Stellt alle Einstellungen der Arbeitsmappe dar.

```csharp
public class WorkbookSettings : IDisposable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author) { get; set; } | Ruft den Autor der Datei ab und legt ihn fest. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures) { get; set; } | Gibt einen booleschen Wert an, der angibt, dass die Anwendung Bilder in der Arbeitsmappe automatisch komprimiert. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover) { get; set; } | Gibt an, ob die Datei für die automatische Wiederherstellung markiert ist. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion) { get; set; } | Gibt die inkrementelle öffentliche Version der Anwendung an. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility) { get; set; } | Gibt an, ob beim Speichern der Arbeitsmappe die Kompatibilität mit früheren Versionen geprüft werden soll. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat) { get; set; } | Gibt an, ob das benutzerdefinierte Zahlenformat beim Festlegen von Style.Custom. überprüft wird. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction) { get; set; } | Ob die Einschränkung der Excel-Datei überprüft wird, wenn der Benutzer zellenbezogene Objekte ändert. Zum Beispiel erlaubt Excel keine Eingabe von Zeichenfolgenwerten, die länger als 32 KB sind. Wenn Sie einen Wert eingeben, der länger als 32 KB ist, wie z Eigenschaft wahr ist, erhalten Sie eine Ausnahme. Wenn diese Eigenschaft falsch ist, akzeptieren wir Ihren eingegebenen Zeichenfolgenwert als Wert der Zelle, sodass Sie später den vollständigen Zeichenfolgenwert für andere Dateiformate wie CSV ausgeben können. Wenn jedoch Sie haben einen Wert festgelegt, der für das Excel-Dateiformat ungültig ist. Sie sollten die Arbeitsmappe später nicht im Excel-Dateiformat speichern. Andernfalls kann es zu einem unerwarteten Fehler für die generierte Excel-Datei kommen. |
| [Compliance](../../aspose.cells/workbooksettings/compliance) { get; set; } | Gibt die OOXML-Version für das Ausgabedokument an. Der Standardwert ist Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave) { get; set; } | gibt an, ob die Anwendung die Arbeitsmappendatei zuletzt nach einem Absturz gespeichert hat. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo) { get; set; } | Ruft die Systemkulturinformationen ab oder legt sie fest. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload) { get; set; } | gibt an, ob die Anwendung die Arbeitsmappe zuletzt zur Datenwiederherstellung geöffnet hat. |
| [Date1904](../../aspose.cells/workbooksettings/date1904) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Arbeitsmappe das Datumssystem 1904 verwendet. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects) { get; set; } | Gibt an, ob und wie Objekte in der Arbeitsmappe angezeigt werden. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros) { get; set; } | Makros aktivieren; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab) { get; set; } | Ruft die erste sichtbare Arbeitsblattregisterkarte ab oder legt sie fest. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings) { get; } | Ruft die Einstellungen für formelbezogene Funktionen ab. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings) { get; set; } | Ruft die Globalisierungseinstellungen ab und legt sie fest. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist) { get; set; } | Ruft ab und legt fest, ob die Feldliste für die PivotTable ausgeblendet wird. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted) { get; set; } | Gibt an, ob die Arbeitsmappe mit dem Standardkennwort verschlüsselt wird, wenn Struktur und Fenster der Arbeitsmappe gesperrt sind. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted) { get; } | Ruft einen Wert ab, der angibt, ob zum Öffnen dieser Arbeitsmappe ein Kennwort erforderlich ist. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden) { get; set; } | Gibt an, ob diese Arbeitsmappe ausgeblendet ist. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die generierte Tabelle eine horizontale Bildlaufleiste enthalten wird. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized) { get; set; } | Gibt an, ob die generierte Tabelle minimiert geöffnet wird. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected) { get; } | Ruft einen Wert ab, der angibt, ob die Struktur oder das Fenster der Arbeitsmappe geschützt ist. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die generierte Tabelle eine vertikale Bildlaufleiste enthalten wird. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode) { get; set; } | Ruft die Sprache der Benutzeroberfläche der Workbook-Version ab oder legt sie fest, basierend auf dem CountryCode, der die Datei gespeichert hat. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn) { get; } | Ruft den maximalen Spaltenindex ab, nullbasiert. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow) { get; } | Ruft den maximalen Zeilenindex ab, nullbasiert. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula) { get; set; } | Ruft die maximale Zeilenanzahl der freigegebenen Formel ab und legt sie fest. |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting) { get; set; } | Ruft die Speichernutzungsoptionen ab oder legt sie fest. Die neue Option wird als Standardoption für neu erstellte Arbeitsblätter verwendet, wird jedoch nicht für vorhandene Arbeitsblätter wirksam. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator) { get; set; } | Ruft das Dezimaltrennzeichen zum Formatieren/Parsen numerischer Werte ab oder legt es fest. Standard ist das Dezimaltrennzeichen der aktuellen Region. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator) { get; set; } | Ruft das Zeichen ab oder legt es fest, das Zifferngruppen links vom Dezimaltrennzeichen in numerischen Werten trennt. Standard ist das Gruppentrennzeichen der aktuellen Region. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize) { get; set; } | Ruft die Standarddruckpapiergröße ab und legt sie fest. |
| [Password](../../aspose.cells/workbooksettings/password) { get; set; } | Stellt das Kennwort für die Verschlüsselung der Arbeitsmappendatei dar. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype) { get; } | Ruft den Schutztyp der Arbeitsmappe ab. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle) { get; set; } | Zeigt an, ob Einstellung[`QuotePrefix`](../style/quoteprefix) -Eigenschaft bei der Eingabe des Zeichenfolgenwerts (der mit einem einfachen Anführungszeichen beginnt) in die Zelle |
| [Region](../../aspose.cells/workbooksettings/region) { get; set; } | Ruft die regionalen Einstellungen für die Arbeitsmappe ab oder legt sie fest. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation) { get; set; } | True, wenn persönliche Informationen aus der angegebenen Arbeitsmappe entfernt werden können. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload) { get; set; } | Gibt an, ob die Anwendung die Arbeitsmappe zuletzt im abgesicherten oder im Reparaturmodus geöffnet hat. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider) { get; set; } | Ruft den Stream-Provider für externe Ressourcen ab und legt ihn fest, z. B. das Laden von Bilddaten für ein Bild vom Typ „LinkToFile“. |
| [Shared](../../aspose.cells/workbooksettings/shared) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Arbeitsmappe freigegeben ist. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth) { get; set; } | Breite der Registerkartenleiste des Arbeitsblatts (in 1/1000 der Fensterbreite). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs) { get; set; } | Abrufen oder Festlegen eines Werts, ob die Registerkarten der Arbeitsmappe angezeigt werden. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits) { get; set; } | Ruft die Anzahl signifikanter Stellen ab und legt sie fest. Der Standardwert ist[`SignificantDigits`](../cellshelper/significantdigits) . |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder) { get; set; } | Gibt an, ob der Rand benachbarter Zellen aktualisiert wird. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype) { get; set; } | Ruft ab und legt fest, wie externe Links aktualisiert werden, wenn die Arbeitsmappe geöffnet wird. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback) { get; set; } | Ruft Warnrückruf ab oder legt ihn fest. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight) { get; set; } | Die Höhe des Fensters in Punkteinheiten. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm) { get; set; } | Die Höhe des Fensters in Zentimetern. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch) { get; set; } | Die Höhe des Fensters in Zoll. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft) { get; set; } | Der Abstand vom linken Rand des Clientbereichs zum linken Rand des Fensters, in Punkteinheiten. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm) { get; set; } | Der Abstand vom linken Rand des Clientbereichs zum linken Rand des Fensters. In Zentimetern. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch) { get; set; } | Der Abstand vom linken Rand des Clientbereichs zum linken Rand des Fensters. In der Einheit Zoll. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop) { get; set; } | Der Abstand vom oberen Rand des Clientbereichs zum oberen Rand des Fensters in Punkteinheiten. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm) { get; set; } | Der Abstand vom oberen Rand des Clientbereichs zum oberen Rand des Fensters in Zentimetern. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch) { get; set; } | Der Abstand vom oberen Rand des Clientbereichs zum oberen Rand des Fensters, in Zolleinheit. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth) { get; set; } | Die Breite des Fensters in Punkteinheiten. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm) { get; set; } | Die Breite des Fensters in Zentimetern. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch) { get; set; } | Die Breite des Fensters in Zoll. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection) { get; } | Bietet Zugriff auf die Schreibschutzoptionen für Arbeitsmappen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose)() | Gibt Ressourcen frei. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont)(FontSchemeType) | Ruft den Standardschriftnamen des Designs ab. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype)(PageOrientationType) | Legen Sie die Art der Druckausrichtung für die gesamte Arbeitsmappe fest. |

### Beispiele

```csharp
[C#]

Workbook workbook = new Workbook();

WorkbookSettings settings = workbook.Settings;

// Mach dein Geschäft

[Visual Basic]
Dim workbook as Workbook = new Workbook()

Dim settings as WorkbookSettings = workbook.Settings

'mach dein Geschäft
```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
