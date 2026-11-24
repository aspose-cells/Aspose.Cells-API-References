---
title: "GridJsWorkbook.InsertImage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridJsWorkbook-Methode. Fügt ein Bild in das Arbeitsblatt aus einem Dateistream oder einer URL ein; entweder muss der Dateistream oder die URL bereitgestellt werden, oder fügt eine Form ein, wenn p.type einer der AutoShapeType ist."
type: docs
url: /de/net/aspose.cells.gridjs/gridjsworkbook/insertimage/
---
## GridJsWorkbook.InsertImage method

Fügt ein Bild im Arbeitsblatt aus einem Dateistream oder einer URL ein (entweder der Dateistream oder die URL muss bereitgestellt werden) oder fügt eine Form ein, wenn p.type einer der AutoShapeType ist.

```csharp
public string InsertImage(string uid, string p, Stream s, string imageUrl)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | String | Die eindeutige ID für den Dateicache. |
| p | String | Der JSON-Format-String für die Operation, die den Zellort angibt, den Arbeitsblattnamen, die obere linke Zeile, die obere linke Spalte für das Bild usw. {name:'sheet1',ri:1,ci:1} |
| s | Stream | Der Dateistream der Bilddatei |
| imageUrl | String | Die URL der Bilddatei |

### Rückgabewert

Der JSON‑Format‑String des eingefügten Bildes

### Siehe auch

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


