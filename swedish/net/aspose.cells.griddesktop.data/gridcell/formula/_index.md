---
title: "GridCell.Formula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCell-egenskap. Hämtar eller anger en formel för cellen"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridcell/formula/
---
## GridCell.Formula property

Hämtar eller anger en formel för cellen.

```csharp
public string Formula { get; set; }
```

### Anmärkningar

En formelsträng börjar alltid med ett likhetstecken (=). Och vänligen använd alltid kommatecken (,) som parameteravgränsare, till exempel "=SUM(A1, E1, H2)".

Användaren kan ange vilken formel som helst i Workbook-designerfilen. Aspose.Cells behåller alla formler. Om användaren använder denna egenskap för att ange en formel i en cell, stöds en stor del av Workbook:s inbyggda funktioner. Och mer kommer. Om du har några speciella behov för Workbook:s inbyggda funktioner, vänligen meddela oss.

### Exempel

```csharp
[C#]
	cell.Formula = "=SUM(A1:C3) + E6*2";
[Visual Basic]
	cell.Formula = "=SUM(A1:C3) + E6*2"
```

### Se även

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


