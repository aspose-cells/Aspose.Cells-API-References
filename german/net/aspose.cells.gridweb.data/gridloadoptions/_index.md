---
title: "Klasse GridLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.GridLoadOptions‑Klasse. Stellt die Optionen für das Laden der Datei dar. Veraltet: Diese Klasse wird nach der Verwendung der eigenständigen DLL des öffentlichen API von Cells obsolet sein; stattdessen können Sie Aspose.Cells.LodOptions verwenden."
type: docs
url: /de/net/aspose.cells.gridweb.data/gridloadoptions/
---
## GridLoadOptions class

Stellt die Optionen zum Laden der Datei dar. [Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.LodOptions ")]

```csharp
public class GridLoadOptions : ISerializable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GridLoadOptions](gridloadoptions/)() | Erstellt eine Option zum Laden der Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | Überprüft, ob die Daten in der Vorlagendatei gültig sind. |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | Ob die Beschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht, einen Zeichenfolgenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K eingeben, etwa mit Cell.PutValue(string), erhalten Sie bei true dieser Eigenschaft eine Exception. Ist die Eigenschaft false, akzeptieren wir Ihren Eingabestring als Zellwert, sodass Sie später den vollständigen Zeichenfolgenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel-Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel-Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel-Datei kommen. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | Ignoriere die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird. |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | Ob die nicht geparsten Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. Standard ist true. |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | Gibt an, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist. |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | Gibt an, ob Formeln beim Lesen der Datei geparst werden. |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. Der Standardwert ist false. |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | Liest und legt das Passwort der Arbeitsmappe fest. |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | Gibt an, ob Leerzeichen und Zeilenumbrüche, die zwischen Formeltoken eingefügt sind, beim Lesen und Schreiben von Formeln erhalten bleiben sollen. Der Standardwert ist false. |

### Siehe auch

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


