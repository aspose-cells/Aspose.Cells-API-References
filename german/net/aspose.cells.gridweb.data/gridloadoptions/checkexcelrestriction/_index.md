---
title: "GridLoadOptions.CheckExcelRestriction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridLoadOptions-Eigenschaft. Gibt an, ob die Beschränkungen der Excel‑Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht, einen Zeichenfolgenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB eingeben, etwa über Cell.PutValuestring, erhalten Sie bei true eine Ausnahme. Ist diese Eigenschaft false, wird der eingegebene Zeichenfolgenwert als Zellenwert akzeptiert, sodass Sie später den vollständigen Zeichenfolgenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen."
type: docs
url: /de/net/aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/
---
## GridLoadOptions.CheckExcelRestriction property

Ob die Beschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht, einen Zeichenfolgenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K eingeben, etwa mit Cell.PutValue(string), erhalten Sie bei true dieser Eigenschaft eine Exception. Ist die Eigenschaft false, akzeptieren wir Ihren Eingabestring als Zellwert, sodass Sie später den vollständigen Zeichenfolgenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel-Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel-Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel-Datei kommen.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Siehe auch

* class [GridLoadOptions](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


