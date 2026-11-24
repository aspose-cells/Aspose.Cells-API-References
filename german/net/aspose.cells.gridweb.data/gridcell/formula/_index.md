---
title: "GridCell.Formula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCell-Eigenschaft. Liest oder legt eine Formel des GridCell fest."
type: docs
url: /de/net/aspose.cells.gridweb.data/gridcell/formula/
---
## GridCell.Formula property

Liest oder legt eine Formel des [`GridCell`](../) fest.

```csharp
public string Formula { get; set; }
```

### Hinweise

Ein Formelkette beginnt immer mit einem Gleichheitszeichen (=). Und bitte immer ein Komma (,) als Parametertrennzeichen verwenden, zum Beispiel "=SUM(A1, E1, H2)".

Benutzer können jede Formel in der Workbook-Designer-Datei festlegen. Aspose.Cells behält alle Formeln bei. Wenn der Benutzer diese Eigenschaft verwendet, um einer Zelle eine Formel zuzuweisen, wird ein großer Teil der integrierten Workbook-Funktionen unterstützt. Und es kommt noch mehr. Wenn Sie spezielle Anforderungen an die integrierten Workbook-Funktionen haben, lassen Sie es uns bitte wissen.

### Beispiele

```csharp
[C#]

ridWeb GridWeb1 = new GridWeb();
ridWorksheet sheet = GridWeb1.ActiveSheet;
heet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1";

Visual Basic]

im GridWeb1 As GridWeb =  New GridWeb() 
im sheet As GridWorksheet =  GridWeb1.ActiveSheet 
heet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1"
```

### Siehe auch

* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


