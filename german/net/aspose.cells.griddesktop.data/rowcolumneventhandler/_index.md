---
title: "Delegate RowColumnEventHandler"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Stellt die Schnittstelle dar, die Zeilen-/Spaltenereignisse behandeln soll"
type: docs
url: /de/net/aspose.cells.griddesktop.data/rowcolumneventhandler/
---
## RowColumnEventHandler delegate

Stellt die Schnittstelle dar, die Zeilen-/Spalten‑Ereignisse behandeln soll.

void **handleCellEvent**(Object sender, RowColumnEventArgs e);

```csharp
public delegate void RowColumnEventHandler(object sender, RowColumnEventArgs e);
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sender | Object | Die Quelle des Ereignisses. |
| e | RowColumnEventArgs | Das Ereignisargument. Rufen Sie e.RejectOperation() auf, wenn Sie den Löschvorgang in den RowDeleting- oder ColumnDeleting-Ereignishandlern abbrechen möchten. |

### Siehe auch

* class [RowColumnEventArgs](../../aspose.cells.griddesktop/rowcolumneventargs/)
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


