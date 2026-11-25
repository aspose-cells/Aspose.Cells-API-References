---
title: "PivotField.Top10AutoShow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Configura le impostazioni Top10 AutoShow per questo campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/top10autoshow/
---
## PivotField.Top10AutoShow method

Configura le impostazioni Top10 AutoShow per questo campo pivot.

```csharp
public void Top10AutoShow(bool isAutoShow, bool isTop, int count, int rankBy)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isAutoShow | Booleano | true per abilitare AutoShow; false per disabilitarlo. |
| isTop | Booleano | Se true, mostra gli elementi superiori; false mostra gli elementi inferiori. |
| conteggio | Int32 | Numero di elementi superiori/inferiori da visualizzare. |
| rankBy | Int32 | Indice del campo dati utilizzato per il ranking. Usa -1 per classificare in base ai valori propri del pivot item. |

### Osservazioni

Questo metodo configura il [`PivotFieldTop10AutoShowSettings`](../../pivotfieldtop10autoshowsettings/).

Formato binario XLS: AutoShow (Top10) è l'opzione nativa e l'unica supportata.

XLSX (OpenXML): Il formato di file sottostante supporta Top10 AutoShow, ma l'interfaccia utente di Excel 2007 e successive espone questa funzionalità solo tramite filtro Top10. Se la compatibilità XLS non è necessaria, si consiglia di utilizzare invece il filtro Top10.

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


