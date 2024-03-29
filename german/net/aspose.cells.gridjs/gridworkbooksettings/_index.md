---
title: GridWorkbookSettings
second_title: Aspose.Cells für .NET-API-Referenz
description: Stellt Einstellungen der Arbeitsmappe dar.
type: docs
weight: 110
url: /de/net/aspose.cells.gridjs/gridworkbooksettings/
---
## GridWorkbookSettings class

Stellt Einstellungen der Arbeitsmappe dar.

```csharp
public class GridWorkbookSettings
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings)() | Default_Constructor |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Author](../../aspose.cells.gridjs/gridworkbooksettings/author) { get; set; } | Ruft den Autor der Datei ab und legt ihn fest. |
| [CheckCustomNumberFormat](../../aspose.cells.gridjs/gridworkbooksettings/checkcustomnumberformat) { get; set; } | Gibt an, ob das benutzerdefinierte Zahlenformat beim Festlegen von Style.Custom. überprüft wird. |
| [CreateCalcChain](../../aspose.cells.gridjs/gridworkbooksettings/createcalcchain) { get; set; } | Gibt an, ob eine berechnete Formelkette erstellt wird. Standard ist false. |
| [Date1904](../../aspose.cells.gridjs/gridworkbooksettings/date1904) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Arbeitsmappe das Datumssystem 1904 verwendet. |
| [EnableMacros](../../aspose.cells.gridjs/gridworkbooksettings/enablemacros) { get; set; } | Makros aktivieren; Jetzt funktioniert es nur, wenn ein Arbeitsblatt in ein anderes Arbeitsblatt in einer Arbeitsmappe kopiert wird. |
| [ForceFullCalculate](../../aspose.cells.gridjs/gridworkbooksettings/forcefullcalculate) { get; set; } | Gibt an, ob jedes Mal, wenn eine Berechnung ausgelöst wird, vollständig berechnet wird. |
| [Iteration](../../aspose.cells.gridjs/gridworkbooksettings/iteration) { get; set; } | Gibt an, ob Iteration verwendet wird, um Zirkelbezüge aufzulösen. |
| [MaxIteration](../../aspose.cells.gridjs/gridworkbooksettings/maxiteration) { get; set; } | Gibt die maximale Anzahl von Iterationen zurück oder legt sie fest, um einen Zirkelverweis aufzulösen, der Standardwert ist 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridjs/gridworkbooksettings/precisionasdisplayed) { get; set; } | True, wenn Berechnungen in dieser Arbeitsmappe nur mit der Genauigkeit der angezeigten Zahlen durchgeführt werden |
| [ReCalculateOnOpen](../../aspose.cells.gridjs/gridworkbooksettings/recalculateonopen) { get; set; } | Gibt an, ob beim Öffnen der Datei alle Formeln neu berechnet werden. |

### Beispiele

```csharp
[C#]

GridJsWorkbook g = new GridJsWorkbook();

GridWorkbookSettings gsettings = new GridWorkbookSettings();
g.Settings=gsettings;

// Mach dein Geschäft

[Visual Basic]
Dim g as GridJsWorkbook = new GridJsWorkbook()

Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 g.Settings=gsettings;
 
'mach dein Geschäft
```

### Siehe auch

* namensraum [Aspose.Cells.GridJs](../../aspose.cells.gridjs)
* Montage [Aspose.Cells.GridJs](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridJs.dll -->
