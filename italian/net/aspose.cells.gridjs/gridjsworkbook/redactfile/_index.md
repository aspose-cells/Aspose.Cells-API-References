---
title: "GridJsWorkbook.RedactFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridJsWorkbook. Esegue la redazione di un file Excel basata su un array di operazioni JSON."
type: docs
url: /it/net/aspose.cells.gridjs/gridjsworkbook/redactfile/
---
## GridJsWorkbook.RedactFile method

Esegue la redazione di un file Excel basata su un array di operazioni JSON.

```csharp
public void RedactFile(string excelFilePath, string uid, string[] arrayOfRedactionOpr)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| excelFilePath | String | Il percorso del file Excel da redigere. |
| uid | String | L'identificatore univoco per la cartella di lavoro. Se null o vuoto, verrà generato un nuovo uid basato sul percorso del file. |
| arrayOfRedactionOpr | String[] | Un array di stringhe JSON che rappresentano le operazioni di redazione da applicare. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [GridCellException](../../gridcellexception/) | Generato quando si verifica una CellsException durante l'operazione di redazione. |
| Exception | Generato quando si verifica un'eccezione generale durante l'operazione di redazione. |

### Vedi anche

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


