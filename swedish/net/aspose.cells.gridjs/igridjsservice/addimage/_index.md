---
title: "IGridJsService.AddImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IGridJsService-metod. Utför tillägg av bild från lokal fil genom att ta bildbytarna direkt."
type: docs
url: /sv/net/aspose.cells.gridjs/igridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

Tillämpar operationen för att lägga till bild från lokal fil, genom att ta bildbytarna direkt.

```csharp
public string AddImage(string p, string uid, string iscontrol, byte[] fileBytes)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| p | String | JSON-strängparameter |
| uid | String | Det unika id:t för filcachen. |
| iscontrol | String | Ange om det är en kontroll. |
| fileBytes | Byte[] | De råa bytena för bildfilen |

### Returvärde

JSON-strängresultat

### Se även

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

Tillämpar operationen för att lägga till bild från lokal fil, med de uppladdade formulärfilerna.

```csharp
public string AddImage(string p, string uid, string iscontrol, IFormFileCollection files)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| p | String | JSON-strängparameter |
| uid | String | Det unika id:t för filcachen. |
| iscontrol | String | Ange om det är en kontroll. |
| filer | IFormFileCollection | Formulärfilen för bilden |

### Returvärde

JSON-strängresultat

### Se även

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


