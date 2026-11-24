---
title: "Klasse HtmlLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HtmlLoadOptions class. Stellt Optionen beim Import einer HTML‑Datei dar."
type: docs
url: /de/net/aspose.cells/htmlloadoptions/
---
## HtmlLoadOptions class

Stellt Optionen beim Importieren einer HTML-Datei dar.

```csharp
public class HtmlLoadOptions : AbstractTextLoadOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [HtmlLoadOptions](htmlloadoptions/#constructor)() | Erstellt eine Option zum Laden der Datei. |
| [HtmlLoadOptions](htmlloadoptions/#constructor_1)(LoadFormat) | Erstellt eine Option zum Laden der Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells/htmlloadoptions/attachedfilesdirectory/) { get; set; } | (**Obsolete.**) Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows/) { get; set; } | Gibt an, ob Spalten und Zeilen automatisch angepasst werden. Der Standardwert ist false. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Liest und setzt die Auto-Fitter-Optionen.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Prüft, ob die Daten in der Vorlagendatei gültig sind.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Ob die Beschränkungen der Excel-Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB über Cell.PutValue(string) eingeben und diese Eigenschaft true ist, erhalten Sie eine Ausnahme. Ist die Eigenschaft false, wird der eingegebene Zeichenkettenwert als Zellenwert akzeptiert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel-Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel-Format speichern. Andernfalls kann ein unerwarteter Fehler in der erzeugten Excel-Datei auftreten.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Zeichenkette in einer Textdatei in Datumsdaten konvertiert wird. Der Standardwert ist true. (Vererbt von [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata/) { get; set; } | (**Obsolete.**) wenn true, Zeichenkette in Formel konvertieren, wenn der Zeichenkettenwert mit dem Zeichen '=', der Standardwert ist false. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. Standardwert ist true.(Vererbt von [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Liest oder setzt die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Liest die Standard-Style-Einstellungen zum Initialisieren der Stile der Arbeitsmappe.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces/) { get; set; } | Gibt an, ob überflüssige Leerzeichen gelöscht werden, wenn der Text Zeilenumbrüche mit dem `<br>`‑Tag erzeugt. Der Standardwert ist false. |
| [DetectLaTeX](../../aspose.cells/htmlloadoptions/detectlatex/) { get; set; } | Gibt an, ob LaTeX‑Formeln in der HTML‑Datei erkannt werden sollen. Der Standardwert ist false. |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Liest und setzt die Standardkodierung. Gilt nur für CSV‑Dateien.(Vererbt von [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Liest und setzt einzelne Schriftkonfigurationen. Funktioniert nur für die [`Workbook`](../workbook/), die diese [`LoadOptions`](../loadoptions/) zum Laden verwendet.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/htmlloadoptions/hasformula/) { get; set; } | Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt. |
| [HyperlinkLoadMode](../../aspose.cells/htmlloadoptions/hyperlinkloadmode/) { get; set; } | Gibt an, wie Hyperlinks beim Laden von HTML verarbeitet werden. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignoriere die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Gibt an, ob nutzlose Formen ignoriert werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Liest und setzt den Unterbrechungsmonitor.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Gibt an, ob ein Zeichenkettenwert nicht geparst wird, wenn die Länge 15 beträgt.(Vererbt von [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Ob die nicht geparsten Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. Standard ist true.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Liest oder setzt die Sprache der Benutzeroberfläche der Arbeitsmappen-Version basierend auf dem CountryCode, mit dem die Datei gespeichert wurde.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Der Daten-Handler zur Verarbeitung von Zellen-Daten beim Lesen der Vorlagendatei.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Der Filter, der angibt, wie Daten geladen werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Liest das Ladeformat.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas/) { get; set; } | Gibt an, ob Formeln importiert werden, wenn die ursprüngliche HTML‑Datei Formeln enthält |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Gibt die Strategie an, die Formatierung für geparste Werte anzuwenden, wenn Zeichenkettenwerte in Zahlen oder Datums‑/Uhrzeitwerte konvertiert werden.(Vererbt von [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Liest oder setzt den Speichermodus für die geladene Arbeitsmappe.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [ParagrahLayoutMode](../../aspose.cells/htmlloadoptions/paragrahlayoutmode/) { get; set; } | (**Obsolete.**) Gibt an, wie HTML &lt;p&gt;-Elemente beim Laden von HTML gerendert werden. Der Standardwert ist Normal. |
| [ParagraphLayoutMode](../../aspose.cells/htmlloadoptions/paragraphlayoutmode/) { get; set; } | Gibt an, wie HTML &lt;p&gt;-Elemente beim Laden von HTML gerendert werden. Der Standardwert ist Normal. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Gibt an, ob die Formel beim Lesen der Datei geparst wird.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. Der Standardwert ist false.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Liest und setzt das Passwort der Arbeitsmappe.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Gibt an, ob die zwischen Formeltoken eingefügten Leerzeichen und Zeilenumbrüche beim Lesen und Schreiben von Formeln erhalten bleiben. Der Standardwert ist false.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [ProgId](../../aspose.cells/htmlloadoptions/progid/) { get; } | Liest die Programm‑ID, mit der die Datei erstellt wurde. Nur für MHT‑Dateien. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Liest oder setzt die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Legt den Standard‑Schriftartnamen fest(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Legt die Standard‑Schriftgröße fest.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider/) { get; set; } | Liest oder setzt den StreamProviderImportHtmlFile zum Importieren von Objekten. |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag/) { get; set; } | Gibt an, ob das Layout des `<div>`‑Tags unterstützt wird, wenn die HTML‑Datei es enthält. Der Standardwert ist false. |
| [TableLoadOptions](../../aspose.cells/htmlloadoptions/tableloadoptions/) { get; } | Holt die HtmlTableLoadOptionCollection‑Instanz |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Liest oder setzt den Warn‑Callback.(Vererbt von [`LoadOptions`](../loadoptions/).) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Legt die Standard‑Papiergröße des Druckers aus den Druckereinstellungen fest.(Vererbt von [`LoadOptions`](../loadoptions/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class HtmlLoadOptionsDemo
    {
        public static void HtmlLoadOptionsExample()
        {
            // Erstelle eine Instanz von HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            loadOptions.LoadFormulas = true;
            loadOptions.SupportDivTag = true;
            loadOptions.DeleteRedundantSpaces = true;
            loadOptions.AutoFitColsAndRows = true;
            loadOptions.HasFormula = true;
            loadOptions.Encoding = System.Text.Encoding.UTF8;
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            loadOptions.ConvertNumericData = true;
            loadOptions.ConvertDateTimeData = true;
            loadOptions.KeepPrecision = true;
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = true;
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = true;
            loadOptions.KeepUnparsedData = true;
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = true;

            // Lade eine HTML‑Datei in ein Workbook mithilfe der HtmlLoadOptions
            Workbook workbook = new Workbook("HtmlLoadOptionsExample_original.html", loadOptions);

            // Speichere die Arbeitsmappe in einer Excel‑Datei
            workbook.Save("HtmlLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


