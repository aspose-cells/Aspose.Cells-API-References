---
title: Formula
second_title: Aspose.Cells för .NET API-referens
description: Hämtar eller ställer in en formel förCell .
type: docs
weight: 70
url: /sv/net/aspose.cells.griddesktop.data/gridcell/formula/
---
## GridCell.Formula property

Hämtar eller ställer in en formel förCell .

```csharp
public string Formula { get; set; }
```

### Anmärkningar

En formelsträng börjar alltid med ett likhetstecken (=). Och använd alltid kommatecken(,) som parametrar avgränsare, till exempel "=SUM(A1, E1, H2)".

Användaren kan ställa in valfri formel i arbetsbokdesignerfilen. Aspose.Cells kommer att behålla alla formler. Om användaren använder den här egenskapen för att ställa in en formel till en cell, stöds större delen av arbetsbokens inbyggda funktioner . Och mer kommer. Om du har något speciellt behov av arbetsbokens inbyggda funktioner, vänligen meddela oss.

### Exempel

```csharp
[C#]
	cell.Formula = "=SUM(A1:C3) + E6*2";
[Visual Basic]
	cell.Formula = "=SUM(A1:C3) + E6*2"
```

### Se även

* class [GridCell](../../gridcell)
* namnutrymme [Aspose.Cells.GridDesktop.Data](../../gridcell)
* hopsättning [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
