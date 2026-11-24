---
title: "AbstractCalculationMonitor.BeforeCalculate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractCalculationMonitor-Methode. Implementieren Sie diese Methode, um Vorgänge auszuführen, bevor eine Zelle berechnet wird."
type: docs
url: /de/net/aspose.cells/abstractcalculationmonitor/beforecalculate/
---
## AbstractCalculationMonitor.BeforeCalculate method

Implementieren Sie diese Methode, um vor der Berechnung einer Zelle geschäftliche Logik auszuführen.

```csharp
public virtual void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | Int32 | Index des Blatts, zu dem die Zelle gehört. |
| rowIndex | Int32 | Zeilenindex der Zelle |
| colIndex | Int32 | Spaltenindex der Zelle |

### Hinweise

Für Zellen in Array-Formeln wird diese Methode möglicherweise nicht ausgeführt, da diese Zellen in der Regel zusammen berechnet werden.

### Siehe auch

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


