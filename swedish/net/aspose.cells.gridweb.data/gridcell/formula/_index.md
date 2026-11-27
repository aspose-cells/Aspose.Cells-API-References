---
title: "GridCell.Formula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCell-egenskap. Hämtar eller anger en formel för GridCell"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridcell/formula/
---
## GridCell.Formula property

Hämtar eller anger en formel för [`GridCell`](../).

```csharp
public string Formula { get; set; }
```

### Anmärkningar

En formelsträng börjar alltid med ett likhetstecken (=). Och vänligen använd alltid kommatecken (,) som parameteravgränsare, till exempel "=SUM(A1, E1, H2)".

Användaren kan ange vilken formel som helst i Workbook-designerfilen. Aspose.Cells behåller alla formler. Om användaren använder denna egenskap för att ange en formel i en cell, stöds en stor del av Workbook:s inbyggda funktioner. Och mer kommer. Om du har några speciella behov för Workbook:s inbyggda funktioner, vänligen meddela oss.

### Exempel

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

### Se även

* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


