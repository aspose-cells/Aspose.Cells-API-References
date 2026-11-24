---
title: "Klasse GridWorkbookSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.GridWorkbookSettings Klasse. Stellt die Einstellungen der Arbeitsmappe dar"
type: docs
url: /de/net/aspose.cells.gridweb.data/gridworkbooksettings/
---
## GridWorkbookSettings class

Stellt die Einstellungen der Arbeitsmappe dar.

```csharp
public class GridWorkbookSettings : ISerializable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | Standardkonstruktor |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Author](../../aspose.cells.gridweb.data/gridworkbooksettings/author/) { get; set; } | Liest und setzt den Autor der Datei. |
| [CheckCustomNumberFormat](../../aspose.cells.gridweb.data/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Gibt an oder legt fest, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat überprüft wird. |
| [CreateCalcChain](../../aspose.cells.gridweb.data/gridworkbooksettings/createcalcchain/) { get; set; } | Gibt an oder legt fest, ob eine Kette berechneter Formeln erstellt wird. Standardwert ist false. |
| [Date1904](../../aspose.cells.gridweb.data/gridworkbooksettings/date1904/) { get; set; } | Gibt den Wert an oder legt ihn fest, der angibt, ob die Arbeitsmappe das 1904-Datumsystem verwendet. |
| [EnableMacros](../../aspose.cells.gridweb.data/gridworkbooksettings/enablemacros/) { get; set; } | Gibt an oder legt fest, ob Makros aktiviert werden; derzeit funktioniert es nur beim Kopieren eines Arbeitsblatts in ein anderes Arbeitsblatt einer Arbeitsmappe. |
| [ForceFullCalculate](../../aspose.cells.gridweb.data/gridworkbooksettings/forcefullcalculate/) { get; set; } | Gibt an oder legt fest, ob bei jeder Auslösung einer Berechnung vollständig neu berechnet wird. |
| [Iteration](../../aspose.cells.gridweb.data/gridworkbooksettings/iteration/) { get; set; } | Gibt an oder legt fest, ob Iterationen zur Auflösung zirkulärer Verweise verwendet werden. |
| [MaxIteration](../../aspose.cells.gridweb.data/gridworkbooksettings/maxiteration/) { get; set; } | Gibt die maximale Anzahl von Iterationen zur Auflösung eines zirkulären Verweises an oder legt sie fest, der Standardwert ist 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridweb.data/gridworkbooksettings/precisionasdisplayed/) { get; set; } | True, wenn Berechnungen in dieser Arbeitsmappe nur mit der Genauigkeit der angezeigten Zahlen durchgeführt werden. |
| [PreservePaddingSpaces](../../aspose.cells.gridweb.data/gridworkbooksettings/preservepaddingspaces/) { get; set; } | Gibt an, ob Leerzeichen und Zeilenumbrüche, die zwischen Formeltoken eingefügt sind, beim Lesen und Schreiben von Formeln erhalten bleiben sollen. Der Standardwert ist false. |
| [ReCalculateOnOpen](../../aspose.cells.gridweb.data/gridworkbooksettings/recalculateonopen/) { get; set; } | Gibt an oder legt fest, ob beim Öffnen der Datei alle Formeln neu berechnet werden. |

### Beispiele

```csharp
[C#]

 
GridWeb gridweb = new GridWeb();
GridWorkbookSettings gsettings = new GridWorkbookSettings();
gridweb.Settings=gsettings;

//Erledigen Sie Ihr Geschäft.

[Visual Basic]


Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 gridweb.Settings=gsettings;
 
'do your business
```

### Siehe auch

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


