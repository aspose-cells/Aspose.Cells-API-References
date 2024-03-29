---
title: AddSpinner
second_title: Aspose.Cells für .NET-API-Referenz
description: Fügt dem Arbeitsblatt ein Kreisel hinzu.
type: docs
weight: 290
url: /de/net/aspose.cells.drawing/shapecollection/addspinner/
---
## ShapeCollection.AddSpinner method

Fügt dem Arbeitsblatt ein Kreisel hinzu.

```csharp
public Spinner AddSpinner(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | Int32 | Zeilenindex oben links. |
| top | Int32 | Stellt den vertikalen Versatz von Spinner von seiner linken Zeile in Pixeleinheiten dar. |
| upperLeftColumn | Int32 | Spaltenindex oben links. |
| left | Int32 | Stellt den horizontalen Versatz von Spinner von seiner linken Spalte in Pixeleinheiten dar. |
| height | Int32 | Repräsentiert die Höhe von Spinner in Pixeleinheiten. |
| width | Int32 | Repräsentiert die Breite von Spinner in Pixeleinheiten. |

### Rückgabewert

Ein Spinner-Objekt.

### Beispiele

```csharp

[C#]
// einen Spinner hinzufügen
Spinner spinner = shapes.AddSpinner(1, 0, 1, 0, 100, 50);
```

### Siehe auch

* class [Spinner](../../spinner)
* class [ShapeCollection](../../shapecollection)
* namensraum [Aspose.Cells.Drawing](../../shapecollection)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
