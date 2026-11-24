---
title: "Klasse GridTxtLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.GridTxtLoadOptions Klasse. Stellt die Optionen zum Laden von Textdateien bereit."
type: docs
url: /de/net/aspose.cells.gridweb.data/gridtxtloadoptions/
---
## GridTxtLoadOptions class

Stellt die Optionen zum Laden einer Textdatei dar.

```csharp
[Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.TxtLoadOptions ")]
public class GridTxtLoadOptions : GridLoadOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GridTxtLoadOptions](gridtxtloadoptions/)() | Erstellt die Optionen zum Laden einer Textdatei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. (Vererbt von [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | Überprüft, ob die Daten in der Vorlagendatei gültig sind. (Vererbt von [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | Ob die Beschränkungen der Excel-Datei überprüft werden, wenn der Benutzer Zellen-bezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K eingeben, etwa durch Cell.PutValue(string), und diese Eigenschaft wahr ist, erhalten Sie eine Ausnahme. Wenn diese Eigenschaft falsch ist, akzeptieren wir Ihren Eingabe‑Stringwert als Zellenwert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festgelegt haben, der für das Excel-Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel-Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel-Datei kommen. (Vererbt von [`GridLoadOptions`](../gridloadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertdatetimedata/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Zeichenkette in der Textdatei in Datumsdaten konvertiert wird. |
| [ConvertNumericData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertnumericdata/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. |
| [Encoding](../../aspose.cells.gridweb.data/gridtxtloadoptions/encoding/) { get; set; } | Liest und setzt die Standardkodierung. Gilt nur für CSV-Dateien. |
| [ExtendToNextSheet](../../aspose.cells.gridweb.data/gridtxtloadoptions/extendtonextsheet/) { get; set; } | Ob Daten auf das nächste Blatt erweitert werden, wenn Zeilen oder Spalten das Limit überschreiten. Wenn diese Eigenschaft wahr ist, werden überschüssige Daten auf das nächste Blatt hinter dem aktuellen Blatt erweitert (wenn das aktuelle Blatt das letzte ist, wird ein neues Blatt zum aktuellen Arbeitsbuch hinzugefügt). Wenn diese Eigenschaft falsch ist, werden die Daten, die das Limit überschreiten, ignoriert. Standardwert ist false; |
| [HasFormula](../../aspose.cells.gridweb.data/gridtxtloadoptions/hasformula/) { get; set; } | Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt. |
| [HasTextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/hastextqualifier/) { get; set; } | Ob ein Textqualifizierer für den Zellenwert vorhanden ist. Standard ist true. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | Ignoriert die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird (Vererbt von [`GridLoadOptions`](../gridloadoptions/).) |
| [IsMultiEncoded](../../aspose.cells.gridweb.data/gridtxtloadoptions/ismultiencoded/) { get; set; } | True bedeutet, dass die Datei mehrere Kodierungen enthält. |
| [KeepPrecision](../../aspose.cells.gridweb.data/gridtxtloadoptions/keepprecision/) { get; set; } | Gibt an, ob ein Zeichenkettenwert bei einer Länge von 15 nicht geparst wird. |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | Ob die nicht geparsten Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. Standardwert ist true. (Vererbt von [`GridLoadOptions`](../gridloadoptions/).) |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | Gibt an, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist. (Vererbt von [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | Gibt an, ob Formeln beim Lesen der Datei geparst werden. (Vererbt von [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | Gibt an, ob zwischengespeicherte Pivot‑Datensätze beim Laden der Datei geparst werden. Der Standardwert ist false. (Vererbt von [`GridLoadOptions`](../gridloadoptions/).) |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | Liest und setzt das Passwort der Arbeitsmappe.(Geerbt von [`GridLoadOptions`](../gridloadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | Gibt an, ob die zwischen Formeltoken eingefügten Leerzeichen und Zeilenumbrüche beim Lesen und Schreiben von Formeln beibehalten werden sollen. Standardwert ist false.(Geerbt von [`GridLoadOptions`](../gridloadoptions/).) |
| [Separator](../../aspose.cells.gridweb.data/gridtxtloadoptions/separator/) { get; set; } | Liest und setzt das Zeichen-Trennzeichen der Textdatei. |
| [SeparatorString](../../aspose.cells.gridweb.data/gridtxtloadoptions/separatorstring/) { get; set; } | Liest und setzt einen Zeichenkettenwert als Trennzeichen. |
| [TextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/textqualifier/) { get; set; } | Gibt den Textqualifizierer für Zellenwerte an. Standardqualifizierer ist '"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | Ob aufeinanderfolgende Trennzeichen als eines behandelt werden sollen. |
| [TreatQuotePrefixAsValue](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatquoteprefixasvalue/) { get; set; } | Gibt an, ob das führende einfache Anführungszeichen als Teil des Zellwertes betrachtet werden soll. Standard ist true. Ist es false, wird das führende einfache Anführungszeichen aus dem entsprechenden Zellwert entfernt und [`QuotePrefix`](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) wird für die Zelle auf true gesetzt. |

### Siehe auch

* class [GridLoadOptions](../gridloadoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


