---
title: "GridWorkbookSettings.CheckExcelRestriction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridWorkbookSettings-Eigenschaft. Gibt an, ob die Beschränkungen der Excel-Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht das Eingeben eines Zeichenkettenwerts, der länger als 32 KB ist. Wenn Sie einen Wert eingeben, der länger als 32 KB ist, etwa über Cell.PutValuestring, und diese Eigenschaft ist true, erhalten Sie eine Ausnahme. Ist die Eigenschaft false, akzeptieren wir Ihren Eingabe‑Stringwert als Zellwert, sodass Sie später den vollständigen Stringwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen solchen Wert setzen, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen. Standardwert ist false."
type: docs
url: /de/net/aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/
---
## GridWorkbookSettings.CheckExcelRestriction property

Gibt an, ob die Beschränkungen einer Excel‑Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB über Cell.PutValue(string) eingeben und diese Eigenschaft auf true gesetzt ist, erhalten Sie eine Ausnahme. Ist die Eigenschaft false, wird der eingegebene Zeichenkettenwert als Zellenwert akzeptiert, sodass Sie später den vollständigen Zeichenkettenwert in anderen Dateiformaten wie CSV ausgeben können. Wenn Sie jedoch einen Wert gesetzt haben, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen. Standard ist false.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Siehe auch

* class [GridWorkbookSettings](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


