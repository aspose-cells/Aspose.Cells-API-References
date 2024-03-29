---
title: TrimLeadingBlankRowAndColumn
second_title: Aspose.Cells für .NET-API-Referenz
description: Gibt an ob führende leere Zeilen und Spalten gekürzt werden sollen wie es MS Excel tut. Standard ist wahr.
type: docs
weight: 120
url: /de/net/aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/
---
## TxtSaveOptions.TrimLeadingBlankRowAndColumn property

Gibt an, ob führende leere Zeilen und Spalten gekürzt werden sollen, wie es MS Excel tut. Standard ist wahr.

```csharp
public bool TrimLeadingBlankRowAndColumn { get; set; }
```

### Bemerkungen

Dasselbe gilt für die Regel in MS Excel, eine Zeile/Spalte wird nicht als leer angesehen, wenn sie einen benutzerdefinierten Stil hat, selbst wenn sie keine Zelldaten enthält. Beim Speichern im LightCells-Modus hat diese Option keine Auswirkung. Der Benutzer sollte Steuerung des Ausgabebereichs durch die Implementierung von[`LightCellsDataProvider`](../lightcellsdataprovider) oder durch Angabe[`ExportArea`](../exportarea)

### Siehe auch

* class [TxtSaveOptions](../../txtsaveoptions)
* namensraum [Aspose.Cells](../../txtsaveoptions)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
