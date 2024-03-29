---
title: AbstractInterruptMonitor
second_title: Aspose.Cells für .NET-API-Referenz
description: Überwachen Sie alle zeitaufwändigen Vorgänge auf Unterbrechungsanforderungen.
type: docs
weight: 50
url: /de/net/aspose.cells/abstractinterruptmonitor/
---
## AbstractInterruptMonitor class

Überwachen Sie alle zeitaufwändigen Vorgänge auf Unterbrechungsanforderungen.

```csharp
public abstract class AbstractInterruptMonitor
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| abstract [IsInterruptionRequested](../../aspose.cells/abstractinterruptmonitor/isinterruptionrequested) { get; } | Gibt an, ob eine Unterbrechung für den aktuellen Betrieb angefordert wird. Wenn wahr, wird der aktuelle Betrieb unterbrochen. Die Implementierung sollte hier eine schnelle und effiziente Überprüfung durchführen, da dies sonst zu einem weiteren Engpass für das Verfahren werden kann. |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception) { get; } | Wenn die Prozedur unterbrochen wird, ob die Prozedur ruhig beendet oder eine Ausnahme ausgelöst wird. Der Standardwert ist falsch, dh wann[`IsInterruptionRequested`](./isinterruptionrequested) ist wahr, a[`CellsException`](../cellsexception) mit CodeInterrupted wird geworfen. |

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
