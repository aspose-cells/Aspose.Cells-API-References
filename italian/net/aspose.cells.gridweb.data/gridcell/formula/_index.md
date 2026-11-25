---
title: "GridCell.Formula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GridCell. Ottiene o imposta una formula della GridCell"
type: docs
url: /it/net/aspose.cells.gridweb.data/gridcell/formula/
---
## GridCell.Formula property

Ottiene o imposta una formula del [`GridCell`](../).

```csharp
public string Formula { get; set; }
```

### Osservazioni

Una stringa di formula inizia sempre con il segno uguale (=). E si prega di utilizzare sempre la virgola (,) come delimitatore dei parametri, ad esempio "=SUM(A1, E1, H2)".

L'utente può impostare qualsiasi formula nel file del designer di Workbook. Aspose.Cells conserverà tutte le formule. Se l'utente utilizza questa proprietà per impostare una formula in una cella, è supportata la maggior parte delle funzioni integrate di Workbook. E ne arriveranno di più. Se hai esigenze particolari per le funzioni integrate di Workbook, faccelo sapere.

### Esempi

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

### Vedi anche

* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


