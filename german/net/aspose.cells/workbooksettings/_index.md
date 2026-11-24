---
title: "Klasse WorkbookSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.WorkbookSettings-Klasse. Stellt alle Einstellungen der Arbeitsmappe dar"
type: docs
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
| [Author](../../aspose.cells/workbooksettings/author/) { get; set; } | Liest und setzt den Autor der Datei. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures/) { get; set; } | Gibt einen booleschen Wert an, der angibt, dass die Anwendung Bilder in der Arbeitsmappe automatisch komprimiert. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover/) { get; set; } | Gibt an, ob die Datei für die automatische Wiederherstellung markiert ist. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion/) { get; set; } | Gibt die inkrementelle öffentliche Version der Anwendung an. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility/) { get; set; } | Gibt an, ob die Kompatibilität mit früheren Versionen beim Speichern der Arbeitsmappe geprüft wird. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat/) { get; set; } | Gibt an, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat geprüft wird. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction/) { get; set; } | Ob die Beschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht, einen Zeichenfolgenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K eingeben, etwa mit Cell.PutValue(string), erhalten Sie bei true dieser Eigenschaft eine Exception. Ist die Eigenschaft false, akzeptieren wir Ihren Eingabestring als Zellwert, sodass Sie später den vollständigen Zeichenfolgenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel-Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel-Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel-Datei kommen. |
| [Compliance](../../aspose.cells/workbooksettings/compliance/) { get; set; } | Gibt die OOXML-Version für das Ausgabedokument an. Der Standardwert ist Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave/) { get; set; } | Gibt an, ob die Anwendung die Arbeitsmappe nach einem Absturz zuletzt gespeichert hat. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo/) { get; set; } | Liest oder setzt die Systemkulturinformationen. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload/) { get; set; } | Gibt an, ob die Anwendung die Arbeitsmappe zuletzt zur Datenwiederherstellung geöffnet hat. |
| [Date1904](../../aspose.cells/workbooksettings/date1904/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob das Workbook das 1904-Datumsystem verwendet. |
| [DefaultImageResolution](../../aspose.cells/workbooksettings/defaultimageresolution/) { get; set; } | Liest und setzt die Standardauflösung des Bildes. |
| [DefaultStyleSettings](../../aspose.cells/workbooksettings/defaultstylesettings/) { get; } | Liest die Einstellungen für Standardwerte von stilbezogenen Eigenschaften für dieses Workbook. |
| [DiscardImageEditData](../../aspose.cells/workbooksettings/discardimageeditdata/) { get; set; } | Gibt an, ob das Verwerfen von bearbeiteten Bilddaten erfolgt. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects/) { get; set; } | Gibt an, ob und wie Objekte im Workbook angezeigt werden. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros/) { get; set; } | Makros aktivieren; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab/) { get; set; } | Liest oder setzt den ersten sichtbaren Arbeitsblatt-Tab. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings/) { get; } | Liest die Einstellungen für formelbezogene Funktionen. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings/) { get; set; } | Liest und setzt die Globalisierungseinstellungen. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist/) { get; set; } | Liest und setzt, ob die Feldliste für die PivotTable ausgeblendet wird. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted/) { get; set; } | Gibt an, ob das Workbook mit dem Standardpasswort verschlüsselt wird, wenn Struktur und Fenster des Workbooks gesperrt sind. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted/) { get; } | Liest einen Wert, der angibt, ob für das Öffnen dieses Workbooks ein Passwort erforderlich ist. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden/) { get; set; } | Gibt an, ob dieses Workbook ausgeblendet ist. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob das erzeugte Tabellenblatt eine horizontale Bildlaufleiste enthält. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized/) { get; set; } | Gibt an, ob das erzeugte Tabellenblatt minimiert geöffnet wird. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected/) { get; } | Liest einen Wert, der angibt, ob die Struktur oder das Fenster des Workbooks geschützt ist. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob das erzeugte Tabellenblatt eine vertikale Bildlaufleiste enthält. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode/) { get; set; } | Liest oder setzt die Benutzeroberflächensprache der Workbook-Version basierend auf dem CountryCode, das die Datei gespeichert hat. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn/) { get; } | Liest den maximalen Spaltenindex, nullbasiert. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow/) { get; } | Liest den maximalen Zeilenindex, nullbasiert. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula/) { get; set; } | Liest und setzt die maximale Zeilennummer der geteilten Formel. |
| [MaxUniqueItemsPerField](../../aspose.cells/workbooksettings/maxuniqueitemsperfield/) { get; set; } | Liest und setzt die Begrenzung eindeutiger Elemente pro Feld. |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting/) { get; set; } | Liest oder setzt die Speicherverbrauchsoptionen. Die neue Option wird als Standardoption für neu erstellte Arbeitsblätter übernommen, wirkt jedoch nicht für bestehende Arbeitsblätter. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator/) { get; set; } | Liest oder setzt das Dezimaltrennzeichen für die Formatierung/Analyse numerischer Werte. Standard ist das Dezimaltrennzeichen der aktuellen Region. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator/) { get; set; } | Liest oder setzt das Zeichen, das Gruppen von Ziffern links vom Dezimaltrennzeichen in numerischen Werten trennt. Standard ist das Gruppentrennzeichen der aktuellen Region. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize/) { get; set; } | Liest und setzt die Standard-Papiergröße für den Druck. |
| [Password](../../aspose.cells/workbooksettings/password/) { get; set; } | Stellt das Verschlüsselungspasswort der Arbeitsmappendatei dar. |
| [PropertiesFollowChartPoint](../../aspose.cells/workbooksettings/propertiesfollowchartpoint/) { get; set; } | Gibt an, ob Datenpunkt-Eigenschaften und Datenbeschriftungen in allen Diagrammen dieser Arbeitsmappe ihrer Referenz folgen. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype/) { get; } | Liest den Schutztyp der Arbeitsmappe. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle/) { get; set; } | Gibt an, ob das Festlegen der [`QuotePrefix`](../style/quoteprefix/)-Eigenschaft beim Eingeben des Zeichenfolgenwerts (der mit einem einfachen Anführungszeichen beginnt) in die Zelle |
| [Region](../../aspose.cells/workbooksettings/region/) { get; set; } | Liest oder setzt die regionalen Einstellungen für die Arbeitsmappe. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation/) { get; set; } | Wahr, wenn persönliche Informationen aus der angegebenen Arbeitsmappe entfernt werden können. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload/) { get; set; } | Gibt an, ob die Anwendung die Arbeitsmappe zuletzt im sicheren oder Reparaturmodus geöffnet hat. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider/) { get; set; } | Liest und setzt den Stream‑Provider für externe Ressourcen, z. B. das Laden von Bilddaten für ein Bild vom Typ "LinkToFile". |
| [ShapeDisplayType](../../aspose.cells/workbooksettings/shapedisplaytype/) { get; set; } | Liest und setzt, wie die Anwendung Formen in dieser Arbeitsmappe anzeigt. |
| [Shared](../../aspose.cells/workbooksettings/shared/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Arbeitsmappe freigegeben ist. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth/) { get; set; } | Breite der Arbeitsblatt‑Registerkartenleiste (in 1/1000 der Fensterbreite). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs/) { get; set; } | Liest oder setzt einen Wert, ob die Arbeitsmappen‑Registerkarten angezeigt werden. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits/) { get; set; } | (**Obsolete.**) Liest und setzt die Anzahl signifikanter Stellen. Der Standardwert ist [`SignificantDigits`](../cellshelper/significantdigits/). |
| [SignificantDigitsType](../../aspose.cells/workbooksettings/significantdigitstype/) { get; set; } | Liest und setzt den Typ signifikanter Stellen für die Ausgabe numerischer Werte in dieser Arbeitsmappe. Der Standardwert ist [`SignificantDigitsType`](../cellshelper/significantdigitstype/). |
| [SmartTagOptions](../../aspose.cells/workbooksettings/smarttagoptions/) { get; } | Liest die Optionen des Smart‑Tags. |
| [StreamProvider](../../aspose.cells/workbooksettings/streamprovider/) { get; set; } | (**Obsolete.**) Liest und setzt den Stream‑Provider für externe Ressourcen. |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder/) { get; set; } | Gibt an, ob die Ränder angrenzender Zellen aktualisiert werden. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype/) { get; set; } | Liest und setzt, wie externe Links beim Öffnen der Arbeitsmappe aktualisiert werden. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback/) { get; set; } | Liest oder setzt den Warnungs-Callback. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight/) { get; set; } | Die Höhe des Fensters, gemessen in Punkten. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm/) { get; set; } | Die Höhe des Fensters, gemessen in Zentimetern. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch/) { get; set; } | Die Höhe des Fensters, gemessen in Zoll. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft/) { get; set; } | Der Abstand von der linken Kante des Client‑Bereichs zur linken Kante des Fensters, gemessen in Punkten. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm/) { get; set; } | Der Abstand von der linken Kante des Client‑Bereichs zur linken Kante des Fensters, gemessen in Zentimetern. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch/) { get; set; } | Der Abstand von der linken Kante des Client‑Bereichs zur linken Kante des Fensters, gemessen in Zoll. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop/) { get; set; } | Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters, in der Einheit Punkt. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm/) { get; set; } | Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters, in der Einheit Zentimeter. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch/) { get; set; } | Der Abstand von der oberen Kante des Clientbereichs bis zur oberen Kante des Fensters, in der Einheit Zoll. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth/) { get; set; } | Die Breite des Fensters, in der Einheit Punkt. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm/) { get; set; } | Die Breite des Fensters, in der Einheit Zentimeter. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch/) { get; set; } | Die Breite des Fensters, in der Einheit Zoll. |
| [WpsCompatibility](../../aspose.cells/workbooksettings/wpscompatibility/) { get; set; } | Gibt an, ob Kompatibilität mit WPS besteht. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection/) { get; } | Stellt Zugriff auf die Schreibschutzoptionen der Arbeitsmappe bereit. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose/)() | Gibt Ressourcen frei. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont/)(FontSchemeType) | Ruft den Standard‑Themen‑Schriftartnamen ab. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype/)(PageOrientationType) | Legt den Typ der Druckausrichtung für die gesamte Arbeitsmappe fest. |

### Beispiele

```csharp
using Aspose.Cells;
using System;
using System.Globalization;

public class WorkbookSettingsDemo
{
    public static void RunDemo()
    {
        // Erstelle ein neues Arbeitsbuch
        Workbook workbook = new Workbook();
        Worksheet sheet = workbook.Worksheets[0];

        // Fügen Sie einige Beispieldaten hinzu
        sheet.Cells["A1"].PutValue("Sample Data");
        sheet.Cells["A2"].PutValue(123);
        sheet.Cells["A3"].PutValue(DateTime.Now);

        // Greift auf die WorkbookSettings zu.
        WorkbookSettings settings = workbook.Settings;

        // Setzt verschiedene Einstellungen.
        settings.Author = "John Doe";
        settings.CheckCustomNumberFormat = true;
        settings.EnableMacros = false;
        settings.Date1904 = false;
        settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
        settings.SheetTabBarWidth = 1000;
        settings.ShowTabs = true;
        settings.FirstVisibleTab = 0;
        settings.IsHScrollBarVisible = true;
        settings.IsVScrollBarVisible = true;
        settings.Shared = false;
        settings.LanguageCode = CountryCode.USA;
        settings.Region = CountryCode.USA;
        settings.CultureInfo = new CultureInfo("en-US");
        settings.GlobalizationSettings = new GlobalizationSettings();
        settings.NumberDecimalSeparator = '.';
        settings.NumberGroupSeparator = ',';
        settings.Password = "password123";
        settings.IsDefaultEncrypted = false;
        settings.IsMinimized = false;
        settings.IsHidden = false;
        settings.AutoCompressPictures = true;
        settings.RemovePersonalInformation = false;
        settings.HidePivotFieldList = false;
        settings.UpdateLinksType = UpdateLinksType.UserSet;
        settings.WindowLeft = 0;
        settings.WindowLeftInch = 0;
        settings.WindowLeftCM = 0;
        settings.WindowTop = 0;
        settings.WindowTopInch = 0;
        settings.WindowTopCM = 0;
        settings.WindowWidth = 800;
        settings.WindowWidthInch = 8;
        settings.WindowWidthCM = 20.32;
        settings.WindowHeight = 600;
        settings.WindowHeightInch = 6;
        settings.WindowHeightCM = 15.24;
        settings.UpdateAdjacentCellsBorder = true;
        settings.SignificantDigits = 15;
        settings.CheckCompatibility = true;
        settings.CheckExcelRestriction = true;
        settings.AutoRecover = true;
        settings.CrashSave = false;
        settings.DataExtractLoad = false;
        settings.RepairLoad = false;
        settings.BuildVersion = "1.0.0";
        settings.MemorySetting = MemorySetting.Normal;
        settings.PaperSize = PaperSizeType.PaperA4;
        settings.WarningCallback = null;
        settings.MaxRowsOfSharedFormula = 1048576;
        settings.Compliance = OoxmlCompliance.Ecma376_2006;
        settings.QuotePrefixToStyle = false;

        // Speichere die Arbeitsmappe
        workbook.Save("WorkbookSettingsDemo.xlsx");
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


