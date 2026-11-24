---
title: "Klasse GridWorkbookSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Klasse Aspose.Cells.GridJs.GridWorkbookSettings. Stellt die Einstellungen der Arbeitsmappe dar."
type: docs
url: /de/net/aspose.cells.gridjs/gridworkbooksettings/
---
## GridWorkbookSettings class

Stellt die Einstellungen der Arbeitsmappe dar.

```csharp
public class GridWorkbookSettings
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Author](../../aspose.cells.gridjs/gridworkbooksettings/author/) { get; set; } | Liest/Setzt den Autor der Datei. |
| [CheckCustomNumberFormat](../../aspose.cells.gridjs/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Gibt an, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat geprüft wird, Standard ist false. |
| [CheckExcelRestriction](../../aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/) { get; set; } | Gibt an, ob die Beschränkungen einer Excel‑Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB über Cell.PutValue(string) eingeben und diese Eigenschaft auf true gesetzt ist, erhalten Sie eine Ausnahme. Ist die Eigenschaft false, wird der eingegebene Zeichenkettenwert als Zellenwert akzeptiert, sodass Sie später den vollständigen Zeichenkettenwert in anderen Dateiformaten wie CSV ausgeben können. Wenn Sie jedoch einen Wert gesetzt haben, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen. Standard ist false. |
| [CreateCalcChain](../../aspose.cells.gridjs/gridworkbooksettings/createcalcchain/) { get; set; } | Gibt an, ob eine Kette berechneter Formeln erstellt wird. Standard ist false. |
| [Date1904](../../aspose.cells.gridjs/gridworkbooksettings/date1904/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob das Workbook das 1904-Datumsystem verwendet. |
| [EnableMacros](../../aspose.cells.gridjs/gridworkbooksettings/enablemacros/) { get; set; } | Makros aktivieren; funktioniert derzeit nur beim Kopieren eines Arbeitsblatts in ein anderes Arbeitsblatt innerhalb einer Arbeitsmappe. |
| [ForceFullCalculate](../../aspose.cells.gridjs/gridworkbooksettings/forcefullcalculate/) { get; set; } | Gibt an, ob bei jeder Auslösung einer Berechnung vollständig neu berechnet wird. |
| [Iteration](../../aspose.cells.gridjs/gridworkbooksettings/iteration/) { get; set; } | Gibt an, ob eine Iteration verwendet wird, um zirkuläre Referenzen zu lösen. |
| [MaxIteration](../../aspose.cells.gridjs/gridworkbooksettings/maxiteration/) { get; set; } | Gibt die maximale Anzahl von Iterationen zurück oder legt sie fest, um eine zirkuläre Referenz zu lösen; der Standardwert ist 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridjs/gridworkbooksettings/precisionasdisplayed/) { get; set; } | True, wenn Berechnungen in dieser Arbeitsmappe nur mit der Genauigkeit der angezeigten Zahlen durchgeführt werden. |
| [ReCalculateOnOpen](../../aspose.cells.gridjs/gridworkbooksettings/recalculateonopen/) { get; set; } | Gibt an, ob beim Öffnen der Datei alle Formeln neu berechnet werden sollen. Standard ist true. |

### Beispiele

```csharp
[C#]

GridJsWorkbook g = new GridJsWorkbook();

GridWorkbookSettings gsettings = new GridWorkbookSettings();
g.Settings=gsettings;

//Erledigen Sie Ihr Geschäft.

[Visual Basic]
Dim g as GridJsWorkbook = new GridJsWorkbook()

Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 g.Settings=gsettings;
 
'do your business
```

### Siehe auch

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


