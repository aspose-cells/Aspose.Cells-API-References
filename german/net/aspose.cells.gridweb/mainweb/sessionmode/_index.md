---
title: "MainWeb.SessionMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MainWeb-Eigenschaft. Gibt den Sitzungsmodus des Rasters zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells.gridweb/mainweb/sessionmode/
---
## MainWeb.SessionMode property

Legt den Sitzungsmodus des Rasters fest.

```csharp
public SessionMode SessionMode { get; set; }
```

### Hinweise

Es gibt 4 Arten von Sitzungsmodus: 1. Session (Standard): System‑Session verwenden, um Blattdaten zu speichern. In der Regel verwendet ASP.NET den InProc‑Sitzungsstatus. Das Raster unterstützt außerdem den \"StateServer\"‑Out‑Process‑Sitzungsstatus und den SQLServer‑Sitzungsstatus. 2. ViewState: ViewState der Seite verwenden, um Blattdaten zu speichern. 3. Custom: LoadCustomData‑ und SheetDataUpdated‑Ereignisse verwenden, um Blattdaten zu speichern/wiederherzustellen. 4. File: Blattdaten im SessionStorePath speichern/wiederherstellen. Dies ist der empfohlene Weg und kann die Datei dauerhaft behalten. Beim Verwenden von SessionMode.ViewState speichert das Raster einige Daten im ViewState der Seite. Das reduziert den Speicherverbrauch des Servers, erhöht jedoch die Seitengröße und wirkt sich auf die Gesamtleistung aus.

### Beispiele

```csharp
[C#]
	GridWeb1.SessionMode = SessionMode.ViewState;
	
[Visual Basic]
	GridWeb1.SessionMode = SessionMode.ViewState
```

### Siehe auch

* enum [SessionMode](../../sessionmode/)
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


