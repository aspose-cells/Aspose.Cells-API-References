---
title: "Enum GridRenameStrategy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridDesktop.Data.GridRenameStrategy enum. Strategieoption für doppelte Spaltennamen"
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridrenamestrategy/
---
## GridRenameStrategy enumeration

Strategieoption für doppelte Spaltennamen.

```csharp
public enum GridRenameStrategy
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Exception | `0` | Wirft eine Ausnahme. |
| Digit | `1` | Benannt mit Ziffer. Doppelte Namen werden zu ...1, ...2 usw. |
| Letter | `2` | Benannt mit Buchstabe. Doppelte Namen werden zu ...A, ...B usw. |

### Hinweise

Beim Verarbeiten von Daten mit Kopfzeilen erfordern einige Szenarien, dass die Kopfzeilen für alle Spalten keine Duplikate aufweisen. Zum Beispiel ist beim Exportieren von Daten in ein DataTable die Kopfzeile als Spaltenname des DataTable erforderlich, sodass doppelte Werte der Kopfzeile ungültig sind. In solchen Situationen kann der Benutzer festlegen, wie damit umgegangen werden soll, indem er diese Strategie angibt.

### Siehe auch

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


