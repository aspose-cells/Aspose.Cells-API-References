---
title: Formula
second_title: Aspose.Cells für .NET-API-Referenz
description: Ruft eine Formel von ab oder legt sie festCell .
type: docs
weight: 70
url: /de/net/aspose.cells.gridweb.data/gridcell/formula/
---
## GridCell.Formula property

Ruft eine Formel von ab oder legt sie festCell .

```csharp
public string Formula { get; set; }
```

### Bemerkungen

Ein Formel-String beginnt immer mit einem Gleichheitszeichen (=). Und bitte verwenden Sie als Parameter-Trennzeichen immer ein Komma(,) wie "=SUMME(A1, E1, H2)".

Der Benutzer kann jede Formel in der Arbeitsmappen-Designerdatei festlegen. Aspose.Cells behält alle Formeln bei. Wenn der Benutzer diese Eigenschaft verwendet, um eine Formel für eine Zelle festzulegen, wird ein Großteil der in Workbook integrierten Funktionen unterstützt. Und es kommt noch mehr. Wenn Sie die integrierten Workbook-Funktionen speziell benötigen, teilen Sie uns dies bitte mit.

### Beispiele

```csharp
[C#]
	cell.Formula = "=SUM(A1:C3) + E6*2";
[Visual Basic]
	cell.Formula = "=SUM(A1:C3) + E6*2"
```

### Siehe auch

* class [GridCell](../../gridcell)
* namensraum [Aspose.Cells.GridWeb.Data](../../gridcell)
* Montage [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
