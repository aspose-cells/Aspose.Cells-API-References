---
title: "AbstractCalculationMonitor.BeforeCalculate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractCalculationMonitor-metod. Implementera den här metoden för att utföra affärslogik innan en cell beräknas."
type: docs
url: /sv/net/aspose.cells/abstractcalculationmonitor/beforecalculate/
---
## AbstractCalculationMonitor.BeforeCalculate method

Implementera den här metoden för att utföra affärslogik innan en cell beräknas.

```csharp
public virtual void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | Int32 | Index för bladet som cellen tillhör. |
| rowIndex | Int32 | Radindex för cellen |
| colIndex | Int32 | Kolumnindex för cellen |

### Anmärkningar

För celler i matrisformler kan den här metoden eventuellt inte köras eftersom dessa celler vanligtvis beräknas tillsammans.

### Se även

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


