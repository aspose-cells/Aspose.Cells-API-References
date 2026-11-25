---
title: "GridCell.Formula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GridCell. Ottiene o imposta una formula della cella"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridcell/formula/
---
## GridCell.Formula property

Ottiene o imposta una formula della cella.

```csharp
public string Formula { get; set; }
```

### Osservazioni

Una stringa di formula inizia sempre con il segno uguale (=). E si prega di utilizzare sempre la virgola (,) come delimitatore dei parametri, ad esempio "=SUM(A1, E1, H2)".

L'utente può impostare qualsiasi formula nel file del designer di Workbook. Aspose.Cells conserverà tutte le formule. Se l'utente utilizza questa proprietà per impostare una formula in una cella, è supportata la maggior parte delle funzioni integrate di Workbook. E ne arriveranno di più. Se hai esigenze particolari per le funzioni integrate di Workbook, faccelo sapere.

### Esempi

```csharp
[C#]
	cell.Formula = "=SUM(A1:C3) + E6*2";
[Visual Basic]
	cell.Formula = "=SUM(A1:C3) + E6*2"
```

### Vedi anche

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


