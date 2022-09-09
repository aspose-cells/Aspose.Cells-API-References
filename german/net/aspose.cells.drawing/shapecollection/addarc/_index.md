---
title: AddArc
second_title: Aspose.Cells für .NET-API-Referenz
description: Fügt dem Arbeitsblatt eine Bogenform hinzu.
type: docs
weight: 30
url: /de/net/aspose.cells.drawing/shapecollection/addarc/
---
## ShapeCollection.AddArc method

Fügt dem Arbeitsblatt eine Bogenform hinzu.

```csharp
public ArcShape AddArc(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | Int32 | Zeilenindex oben links. |
| top | Int32 | Stellt den vertikalen Versatz von ArcShape von seiner linken Zeile in Pixeleinheiten dar. |
| upperLeftColumn | Int32 | Spaltenindex oben links. |
| left | Int32 | Stellt den horizontalen Versatz von ArcShape von seiner linken Spalte in Pixeleinheiten dar. |
| height | Int32 | Stellt die Höhe von ArcShape in Pixeleinheiten dar. |
| width | Int32 | Stellt die Breite von ArcShape in Pixeleinheiten dar. |

### Rückgabewert

Ein ArcShape-Objekt.

### Beispiele

```csharp

[C#]
// einen Bogen hinzufügen
ArcShape arcShape = shapes.AddArc(1, 0, 1, 0, 100, 50);
```

### Siehe auch

* class [ArcShape](../../arcshape)
* class [ShapeCollection](../../shapecollection)
* namensraum [Aspose.Cells.Drawing](../../shapecollection)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->