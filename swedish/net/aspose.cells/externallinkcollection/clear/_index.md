---
title: Clear
second_title: Aspose.Cells för .NET API-referens
description: Tar bort alla externa länkar.
type: docs
weight: 40
url: /sv/net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

Tar bort alla externa länkar.

```csharp
public void Clear()
```

### Anmärkningar

När du tar bort externa länkar kommer alla formler som refererar till dem att tas bort också eftersom referenserna blir ogiltiga.

### Se även

* class [ExternalLinkCollection](../../externallinkcollection)
* namnutrymme [Aspose.Cells](../../externallinkcollection)
* hopsättning [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

Tar bort alla externa länkar.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| updateReferencesAsLocal | Boolean | Om du uppdaterar alla referenser till externa länkar som referenser till den aktuella arbetsboken själv. |

### Anmärkningar

Om referenser måste uppdateras kommer referenser till externa länkar i formler att ändras till aktuell arbetsbok. Till exempel är en cells ursprungliga formel "='externalsource.xlam'!customfunction()", efter att ha tagit bort externa länkar, formeln blir "=customfunction()". Om referenser inte behöver uppdateras kommer alla formler med referenser till externa länkar att tas bort också eftersom dessa referenser blir ogiltiga.

### Se även

* class [ExternalLinkCollection](../../externallinkcollection)
* namnutrymme [Aspose.Cells](../../externallinkcollection)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
