---
title: "IGridJsService.AddImage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IGridJsService Methode. Führt die Operation zum Hinzufügen eines Bildes aus einer lokalen Datei aus, wobei die Bildbytes direkt verwendet werden."
type: docs
url: /de/net/aspose.cells.gridjs/igridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

Wendet die Operation zum Hinzufügen eines Bildes aus einer lokalen Datei an und verwendet die Bildbytes direkt.

```csharp
public string AddImage(string p, string uid, string iscontrol, byte[] fileBytes)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| p | String | Der JSON‑String‑Parameter |
| uid | String | Die eindeutige ID für den Dateicache. |
| iscontrol | String | Geben Sie an, ob es sich um ein Steuerelement handelt. |
| fileBytes | Byte[] | Die rohen Bytes der Bilddatei |

### Rückgabewert

Das JSON‑String‑Ergebnis

### Siehe auch

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

Wendet die Operation zum Hinzufügen eines Bildes aus einer lokalen Datei an und verwendet die hochgeladenen Formulardateien.

```csharp
public string AddImage(string p, string uid, string iscontrol, IFormFileCollection files)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| p | String | Der JSON‑String‑Parameter |
| uid | String | Die eindeutige ID für den Dateicache. |
| iscontrol | String | Geben Sie an, ob es sich um ein Steuerelement handelt. |
| Dateien | IFormFileCollection | Die Formdatei des Bildes |

### Rückgabewert

Das JSON‑String‑Ergebnis

### Siehe auch

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


