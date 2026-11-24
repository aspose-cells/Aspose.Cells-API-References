---
title: "Klasse Workbook"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Workbook-Klasse. Stellt ein Root-Objekt zum Erstellen einer Excel-Tabelle dar"
type: docs
url: /de/net/aspose.cells/workbook/
---
## Workbook class

Stellt ein Root‑Objekt zum Erstellen einer Excel‑Tabelle dar.

```csharp
public class Workbook : IDisposable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Workbook](workbook/#constructor)() | Initialisiert eine neue Instanz der `Workbook`-Klasse. |
| [Workbook](workbook/#constructor_1)(FileFormatType) | Initialisiert eine neue Instanz der `Workbook`-Klasse. |
| [Workbook](workbook/#constructor_2)(LoadOptions) | Initialisiert eine neue leere Instanz der `Workbook`-Klasse mit Optionen |
| [Workbook](workbook/#constructor_3)(Stream) | Initialisiert eine neue Instanz der `Workbook`-Klasse und öffnet einen Stream. |
| [Workbook](workbook/#constructor_5)(string) | Initialisiert eine neue Instanz der `Workbook`-Klasse und öffnet eine Datei. |
| [Workbook](workbook/#constructor_4)(Stream, LoadOptions) | Initialisiert eine neue Instanz der `Workbook`-Klasse und öffnet einen Stream. |
| [Workbook](workbook/#constructor_6)(string, LoadOptions) | Initialisiert eine neue Instanz der `Workbook`-Klasse und öffnet eine Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath/) { get; set; } | Liest und setzt den absoluten Pfad der Datei. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties/) { get; } | Gibt eine [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) Sammlung zurück, die alle integrierten Dokumenteigenschaften der Tabelle darstellt. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory/) { get; } | Gibt die Fabrik zum Erstellen von ICellsDataTable aus benutzerdefinierten Objekten zurück |
| [Colors](../../aspose.cells/workbook/colors/) { get; } | Gibt Farben in der Palette für die Tabelle zurück. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties/) { get; } | Liest die Liste der [`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty/) Objekte im Arbeitsbuch. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool/) { get; } | Liest die Anzahl der Stile im Stil-Pool. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties/) { get; } | Gibt eine [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Tabelle darstellt. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts/) { get; } | Stellt einen benutzerdefinierten XML‑Datenspeicherteil dar (benutzerdefinierte XML‑Daten innerhalb eines Pakets). |
| [DataConnections](../../aspose.cells/workbook/dataconnections/) { get; } | Liest die [`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection/) Sammlung. |
| [DataMashup](../../aspose.cells/workbook/datamashup/) { get; } | Liest Mashup-Daten. |
| [DataModel](../../aspose.cells/workbook/datamodel/) { get; } | Liest das Datenmodell im Arbeitsbuch. |
| [DataSorter](../../aspose.cells/workbook/datasorter/) { get; } | Erhält ein DataSorter-Objekt zum Sortieren von Daten. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle/) { get; set; } | Liest oder setzt das [`Style`](../style/)‑Objekt der Arbeitsmappe. |
| [FileFormat](../../aspose.cells/workbook/fileformat/) { get; set; } | Liest und setzt das Dateiformat. |
| [FileName](../../aspose.cells/workbook/filename/) { get; set; } | Liest und setzt den aktuellen Dateinamen. |
| [HasCustomFunction](../../aspose.cells/workbook/hascustomfunction/) { get; } | Ermittelt, ob in dieser Arbeitsmappe benutzerdefinierte Funktionen verwendet werden, z. B. in Zellformeln oder definierten Namen... |
| [HasMacro](../../aspose.cells/workbook/hasmacro/) { get; } | Gibt an, ob diese Tabelle Makros/VBA enthält. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions/) { get; } | Liest, ob die Arbeitsmappe nachverfolgte Änderungen enthält |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor/) { get; set; } | Liest und setzt den Interrupt‑Monitor. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned/) { get; } | Gibt an, ob diese Tabelle digital signiert ist. |
| [IsLicensed](../../aspose.cells/workbook/islicensed/) { get; } | Gibt an, ob eine Lizenz festgelegt ist. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword/) { get; } | Gibt an, ob Struktur oder Fenster mit einem Kennwort geschützt ist. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml/) { get; set; } | Liest und setzt die XML‑Datei, die die Ribbon‑UI definiert. |
| [Settings](../../aspose.cells/workbook/settings/) { get; } | Stellt die Einstellungen der Arbeitsmappe dar. |
| [Theme](../../aspose.cells/workbook/theme/) { get; } | Liest den Namen des Themas. |
| [VbaProject](../../aspose.cells/workbook/vbaproject/) { get; } | Liest das [`VbaProject`](./vbaproject/) in einer Tabelle. |
| [Worksheets](../../aspose.cells/workbook/worksheets/) { get; } | Liest die [`WorksheetCollection`](../worksheetcollection/)-Sammlung in der Tabelle. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions/)() | Akzeptiert alle nachverfolgten Änderungen in der Arbeitsmappe. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature/)(DigitalSignatureCollection) | Fügt einer OOXML‑Tabellendatei (Excel2007 und neuer) eine digitale Signatur hinzu. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula)() | Berechnet das Ergebnis von Formeln. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_2)(bool) | Berechnet das Ergebnis von Formeln. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_1)(CalculationOptions) | Formeln in dieser Arbeitsmappe werden berechnet. |
| [ChangePalette](../../aspose.cells/workbook/changepalette/)(Color, int) | Ändert die Palette der Tabelle am angegebenen Index. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache/)(AccessCacheOptions) | Schließt die Sitzung, die Zwischenspeicher zum Datenzugriff verwendet. |
| [Combine](../../aspose.cells/workbook/combine/)(Workbook) | Kombiniert ein weiteres Workbook‑Objekt. |
| [Copy](../../aspose.cells/workbook/copy/#copy)(Workbook) | Kopiert Daten aus einem Quell‑Workbook‑Objekt. |
| [Copy](../../aspose.cells/workbook/copy/#copy_1)(Workbook, CopyOptions) | Kopiert ein weiteres Workbook‑Objekt. |
| [CopyTheme](../../aspose.cells/workbook/copytheme/)(Workbook) | Kopiert das Design aus einer anderen Arbeitsmappe. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle/)(BuiltinStyleType) | Erstellt einen integrierten Stil anhand des angegebenen Typs. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor/)() | Erstellt ein [`CellsColor`](../cellscolor/) Objekt. |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle)() | Erstellt einen neuen Stil. |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle_1)(bool) | Erstellt einen neuen Stil. |
| [CustomTheme](../../aspose.cells/workbook/customtheme/)(string, Color[]) | Passt das Design an. |
| [Dispose](../../aspose.cells/workbook/dispose/)() | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml)(string, Stream) | Exportiert XML‑Daten. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml_1)(string, string) | Exportiert XML‑Daten, die durch die angegebene XML‑Zuordnung verknüpft sind. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature/)() | Liest die digitale Signatur aus einer Datei. |
| [GetFonts](../../aspose.cells/workbook/getfonts/)() | Ermittelt alle Schriftarten im Stil‑Pool. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor/)(Color) | Findet die am besten passende Farbe in der aktuellen Palette. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle/)(string) | Ermittelt den benannten Stil im Stil‑Pool. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool/)(int) | Ermittelt den Stil im Stil‑Pool. Alle Stile in der Arbeitsmappe werden in einen Pool gesammelt. In den Zellen gibt es nur einen einfachen Referenz‑Index. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor/)(ThemeColorType) | Ermittelt die Designfarbe. |
| [HasExernalLinks](../../aspose.cells/workbook/hasexernallinks/)() | (**Obsolete.**) Gibt an, ob diese Arbeitsmappe externe Verknüpfungen zu anderen Datenquellen enthält. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml)(Stream, string, int, int) | Importiert/aktualisiert eine XML‑Datendatei in die Arbeitsmappe. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml_1)(string, string, int, int) | Importiert/aktualisiert eine XML‑Datendatei in die Arbeitsmappe. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette/)(Color) | Prüft, ob eine Farbe in der Palette für das Tabellenblatt vorhanden ist. |
| [MergeNamedStyles](../../aspose.cells/workbook/mergenamedstyles/)(Workbook) | Führt benannte Stile aus der anderen Excel‑Datei zusammen. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas/)(bool) | Parst alle Formeln, die beim Laden aus einer Vorlagendatei oder beim Setzen in eine Zelle nicht geparst wurden. |
| [Protect](../../aspose.cells/workbook/protect/)(ProtectionType, string) | Schützt eine Arbeitsmappe. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook/)(string) | Schützt eine freigegebene Arbeitsmappe. |
| [RefreshAll](../../aspose.cells/workbook/refreshall/)() | Aktualisiert verknüpfte Formen, alle Pivot‑Tabellen und Diagramme mit der Pivot‑Quelle. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas)(bool) | Aktualisiert dynamische Array‑Formeln (erweitern sich in einen neuen Bereich benachbarter Zellen gemäß den aktuellen Daten). Andere Formeln in der Arbeitsmappe werden nicht rekursiv berechnet, selbst wenn sie von dynamischen Array‑Formeln verwendet werden. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas_1)(bool, CalculationOptions) | Aktualisiert dynamische Array‑Formeln (erweitern sich in einen neuen Bereich benachbarter Zellen gemäß den aktuellen Daten). |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature/)() | Entfernt die digitale Signatur aus diesem Tabellenblatt. |
| [RemoveExternalLinks](../../aspose.cells/workbook/removeexternallinks/)() | (**Obsolete.**) Entfernt alle externen Verknüpfungen in der Arbeitsmappe. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro/)() | Entfernt VBA/Makro aus diesem Tabellenblatt. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation/)() | Entfernt persönliche Informationen. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles/)() | Entfernt alle ungenutzten Stile. |
| [Replace](../../aspose.cells/workbook/replace/#replace)(bool, object) | Ersetzt die Werte der Zellen durch neue Daten. |
| [Replace](../../aspose.cells/workbook/replace/#replace_1)(int, object) | Ersetzt die Werte der Zellen durch neue Daten. |
| [Replace](../../aspose.cells/workbook/replace/#replace_6)(string, DataTable) | Ersetzt die Werte der Zellen durch Daten aus einer DataTable. |
| [Replace](../../aspose.cells/workbook/replace/#replace_2)(string, double) | Ersetzt den Wert einer Zelle durch einen neuen Double. |
| [Replace](../../aspose.cells/workbook/replace/#replace_4)(string, int) | Ersetzt den Wert einer Zelle durch einen neuen Integer. |
| [Replace](../../aspose.cells/workbook/replace/#replace_7)(string, string) | Ersetzt den Wert einer Zelle durch einen neuen String. |
| [Replace](../../aspose.cells/workbook/replace/#replace_3)(string, double[], bool) | Ersetzt die Werte der Zellen durch ein Double-Array. |
| [Replace](../../aspose.cells/workbook/replace/#replace_5)(string, int[], bool) | Ersetzt die Werte der Zellen durch ein Integer-Array. |
| [Replace](../../aspose.cells/workbook/replace/#replace_8)(string, string, ReplaceOptions) | Ersetzt den Wert einer Zelle durch einen neuen String. |
| [Replace](../../aspose.cells/workbook/replace/#replace_9)(string, string[], bool) | Ersetzt den Wert einer Zelle durch ein neues String-Array. |
| [Save](../../aspose.cells/workbook/save/#save_2)(string) | Speichert die Arbeitsmappe auf der Festplatte. |
| [Save](../../aspose.cells/workbook/save/#save)(Stream, SaveFormat) | Speichert die Arbeitsmappe in den Stream. |
| [Save](../../aspose.cells/workbook/save/#save_1)(Stream, SaveOptions) | Speichert die Arbeitsmappe in den Stream. |
| [Save](../../aspose.cells/workbook/save/#save_3)(string, SaveFormat) | Speichert die Arbeitsmappe auf der Festplatte. |
| [Save](../../aspose.cells/workbook/save/#save_4)(string, SaveOptions) | Speichert die Arbeitsmappe auf der Festplatte. |
| [Save](../../aspose.cells/workbook/save/#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Erstellt die Ergebnis-Tabelle und überträgt sie an den Client, dann öffnet sie im Browser oder in MS Workbook. |
| [Save](../../aspose.cells/workbook/save/#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Erstellt die Ergebnis-Tabelle und überträgt sie an den Client, dann öffnet sie im Browser oder in MS Workbook. |
| [SaveToStream](../../aspose.cells/workbook/savetostream/)() | Speichert die Excel-Datei in ein MemoryStream-Objekt als Excel97-2003 xls-Datei und gibt sie zurück. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature/)(DigitalSignatureCollection) | Setzt eine digitale Signatur für eine Tabellenkalkulationsdatei (Excel2007 und neuer). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions/)(EncryptionType, int) | Verschlüsselungsoptionen festlegen. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor/)(ThemeColorType, Color) | Setzt die Designfarbe |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache/)(AccessCacheOptions) | Startet die Sitzung, die Caches zum Zugriff auf Daten verwendet. |
| [Unprotect](../../aspose.cells/workbook/unprotect/)(string) | Entfernt den Schutz einer Arbeitsmappe. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook/)(string) | Entfernt den Schutz einer freigegebenen Arbeitsmappe. |
| [UpdateCustomFunctionDefinition](../../aspose.cells/workbook/updatecustomfunctiondefinition/)(CustomFunctionDefinition) | Aktualisiert die Definition benutzerdefinierter Funktionen. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource/)(Workbook[]) | Wenn diese Arbeitsmappe externe Links zu anderen Datenquellen enthält, versucht Aspose.Cells, die neuesten Daten aus den angegebenen Quellen abzurufen. |

### Hinweise

Die Workbook-Klasse bezeichnet eine Excel-Tabelle. Jede Tabelle kann mehrere Arbeitsblätter enthalten. Das Grundmerkmal der Klasse ist das Öffnen und Speichern nativer Excel-Dateien. Die Klasse verfügt über erweiterte Funktionen wie das Kopieren von Daten aus anderen Workbooks, das Kombinieren zweier Workbooks, das Konvertieren von Excel zu PDF, das Rendern von Excel zu Bild und das Schützen der Excel-Tabelle.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDemo
    {
        public static void WorkbookExample()
        {
            // Erstelle eine neue Workbook-Instanz
            Workbook workbook = new Workbook();

            // Zugriff auf das Standard-Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Eigenschaften der Arbeitsmappe festlegen
            workbook.FileName = "ExampleWorkbook.xlsx";
            workbook.DefaultStyle.Font.Name = "Tahoma";

            // Ein neues Arbeitsblatt hinzufügen
            int newSheetIndex = workbook.Worksheets.Add();
            Worksheet newWorksheet = workbook.Worksheets[newSheetIndex];
            newWorksheet.Name = "NewSheet";

            // Einige Daten zum neuen Arbeitsblatt hinzufügen
            newWorksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");

            // Einige Dokumenteigenschaften festlegen
            workbook.BuiltInDocumentProperties["Author"].Value = "John Smith";
            workbook.CustomDocumentProperties.Add("Checked by", "Jane");

            // Speichere die Arbeitsmappe in einer Datei
            workbook.Save("WorkbookExample.xlsx");

            // Einige Eigenschaften anzeigen
            Console.WriteLine("Workbook File Name: " + workbook.FileName);
            Console.WriteLine("Default Font: " + workbook.DefaultStyle.Font.Name);
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Custom Property 'Checked by': " + workbook.CustomDocumentProperties["Checked by"].Value);

            // Prüfen, ob die Arbeitsmappe lizenziert ist
            Console.WriteLine("Is Licensed: " + workbook.IsLicensed);

            // Prüfen, ob die Arbeitsmappe digital signiert ist
            Console.WriteLine("Is Digitally Signed: " + workbook.IsDigitallySigned);

            // Prüfen, ob die Arbeitsmappe Makros enthält
            Console.WriteLine("Has Macros: " + workbook.HasMacro);

            // Prüfen, ob die Arbeitsmappe nachverfolgte Änderungen hat
            Console.WriteLine("Has Revisions: " + workbook.HasRevisions);

            // Anzahl der Stile im Stil-Pool prüfen
            Console.WriteLine("Number of Styles in Pool: " + workbook.CountOfStylesInPool);

            // Themenname prüfen
            Console.WriteLine("Theme: " + workbook.Theme);

            // Prüfen, ob die Arbeitsmappe mit einem Passwort geschützt ist
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Prüfen, ob die Arbeitsmappe externe Links enthält
            Console.WriteLine("Has External Links: " + (workbook.Worksheets.ExternalLinks.Count > 0));

            // Arbeitsmappe freigeben
            workbook.Dispose();
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


