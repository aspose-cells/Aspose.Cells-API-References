---
title: SetBorderPosition
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta la posizione del bordo da impostare di un intervallo di celle.
type: docs
weight: 900
url: /it/net/aspose.cells.gridweb/setborderposition/
---
## SetBorderPosition enumeration

Rappresenta la posizione del bordo da impostare di un intervallo di celle.

```csharp
public enum SetBorderPosition
```

### I valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Top | `0` | Bordo superiore |
| Bottom | `1` | Bordo inferiore |
| Left | `2` | Bordo sinistro |
| Right | `3` | Bordo destro |
| HorizontalMiddle | `4` | Bordo inferiore |
| VerticalMiddle | `5` | Bordi centrali orizzontali |
| Outline | `6` | Bordi centrali verticali |
| Cross | `7` | Oltre confine |
| None | `8` | Nessun bordo |

### Esempi

```csharp
[C#]
	GridWeb1.WebWorksheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1);

[VB]
	GridWeb1.WebWorksheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1)
```

### Guarda anche

* spazio dei nomi [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* assemblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->