---
title: "GridCell.Formula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCell property. Gibt eine Formel der Zelle zurück oder setzt sie"
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridcell/formula/
---
## GridCell.Formula property

Liest oder setzt eine Formel der Zelle.

```csharp
public string Formula { get; set; }
```

### Hinweise

Ein Formelkette beginnt immer mit einem Gleichheitszeichen (=). Und bitte immer ein Komma (,) als Parametertrennzeichen verwenden, zum Beispiel "=SUM(A1, E1, H2)".

Benutzer können jede Formel in der Workbook-Designer-Datei festlegen. Aspose.Cells behält alle Formeln bei. Wenn der Benutzer diese Eigenschaft verwendet, um einer Zelle eine Formel zuzuweisen, wird ein großer Teil der integrierten Workbook-Funktionen unterstützt. Und es kommt noch mehr. Wenn Sie spezielle Anforderungen an die integrierten Workbook-Funktionen haben, lassen Sie es uns bitte wissen.

### Beispiele

```csharp
[C#]
	cell.Formula = "=SUM(A1:C3) + E6*2";
[Visual Basic]
	cell.Formula = "=SUM(A1:C3) + E6*2"
```

### Siehe auch

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


