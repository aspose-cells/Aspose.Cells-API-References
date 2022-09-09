---
title: RowColumnEventHandler
second_title: Aspose.Cells für .NET-API-Referenz
description: Stellt die Schnittstelle dar die beabsichtigt Zeilen-/Spaltenereignisse zu verarbeiten.
type: docs
weight: 670
url: /de/net/aspose.cells.gridweb.data/rowcolumneventhandler/
---
## RowColumnEventHandler delegate

Stellt die Schnittstelle dar, die beabsichtigt, Zeilen-/Spaltenereignisse zu verarbeiten.

Leere **handleCellEvent**(Objektsender, RowColumnEventArgs e);

```csharp
public delegate void RowColumnEventHandler(object sender, RowColumnEventArgs e);
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sender | Object | Die Quelle des Ereignisses. |
| e | RowColumnEventArgs | Das Ereignisargument. Rufen Sie e.RejectOperation() auf, wenn Sie den Löschvorgang in den Ereignishandlern RowDeleting oder ColumnDeleting abbrechen möchten. |

### Siehe auch

* class [RowColumnEventArgs](../../aspose.cells.gridweb/rowcolumneventargs)
* namensraum [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* Montage [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->