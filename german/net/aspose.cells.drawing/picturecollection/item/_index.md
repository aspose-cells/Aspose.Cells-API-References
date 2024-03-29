---
title: Item
second_title: Aspose.Cells für .NET-API-Referenz
description: Ruft die abPictureaspose.cells.drawing/picture Element am angegebenen Index.
type: docs
weight: 10
url: /de/net/aspose.cells.drawing/picturecollection/item/
---
## PictureCollection indexer

Ruft die ab[`Picture`](../../picture) Element am angegebenen Index.

```csharp
public Picture this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp

[C#]
// Bildsammlung abrufen
//PictureCollection Bilder = Arbeitsmappe.Arbeitsblätter[0].Bilder;
//Bild hinzufügen
int index = pictures.Add(1, 1, "image.png");
//verstehe
Picture pic = pictures[index];
```

### Siehe auch

* class [Picture](../../picture)
* class [PictureCollection](../../picturecollection)
* namensraum [Aspose.Cells.Drawing](../../picturecollection)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
