---
title: "Klasse ComboBox"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridDesktop.ComboBox Klasse. Stellt ein Zellen-ComboBox-Steuerelement dar"
type: docs
url: /de/net/aspose.cells.griddesktop/combobox/
---
## ComboBox class

Stellt ein Zell-ComboBox-Steuerelement dar.

```csharp
public class ComboBox : CellControl
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Height](../../aspose.cells.griddesktop/combobox/height/) { get; set; } | Liest oder setzt die Höhe des Listensteuerelements. |
| [IsInputable](../../aspose.cells.griddesktop/combobox/isinputable/) { get; set; } | Gibt an, ob der Benutzer Text in die ComboBox eingeben kann. Der eingegebene Text wird als Zellwert gespeichert. Der Standardwert ist "false". |
| [Items](../../aspose.cells.griddesktop/combobox/items/) { get; } | Liefert ein Objekt, das die Sammlung der in dieser ComboBox enthaltenen Elemente darstellt. |
| [SelectedIndex](../../aspose.cells.griddesktop/combobox/selectedindex/) { get; set; } | Liest oder setzt den Index, der das aktuell ausgewählte Element angibt. Das Setzen des Index ruft die Methode GridDesktop.RunAllFormulas automatisch auf, wenn die Eigenschaft GridDesktop.RecalculateFormulas true ist. |
| [Text](../../aspose.cells.griddesktop/cellcontrol/text/) { get; set; } | Liest oder setzt den Text, der mit diesem Steuerelement verknüpft ist. (Vererbt von [`CellControl`](../cellcontrol/).) |
| [Values](../../aspose.cells.griddesktop/combobox/values/) { get; } | Liefert ein Objekt, das die Sammlung der in dieser ComboBox enthaltenen Werte darstellt. |
| [Width](../../aspose.cells.griddesktop/combobox/width/) { get; set; } | Liest oder setzt die Breite des Listensteuerelements. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetSelectedIndex](../../aspose.cells.griddesktop/combobox/setselectedindex/)(int) | Setzt den ausgewählten Index der ComboBox. Dadurch wird keine Formel berechnet. Um eine Formel zu berechnen, muss GridDesktop.RunAllFormulas manuell aufgerufen werden. Formeln werden in keinem Fall automatisch berechnet, selbst wenn GridDesktop.RecalculateFormulas true ist. |

### Siehe auch

* class [CellControl](../cellcontrol/)
* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


