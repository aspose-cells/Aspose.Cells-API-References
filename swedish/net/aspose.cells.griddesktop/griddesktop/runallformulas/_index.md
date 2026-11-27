---
title: "GridDesktop.RunAllFormulas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridDesktop metod. Kör alla cellernas formler"
type: docs
url: /sv/net/aspose.cells.griddesktop/griddesktop/runallformulas/
---
## GridDesktop.RunAllFormulas method

Kör alla cellers formler.

```csharp
public void RunAllFormulas()
```

### Exempel

```csharp
[C#]
gridDesktop1.Worksheets[0].Cells[0, 0].Value = "2";
gridDesktop1.Worksheets[0].Cells[1, 0].Value = "3";
gridDesktop1.Worksheets[0].Cells[2, 1].Value = "=a1*a2";
gridDesktop1.RunAllFormulas();
gridDesktop1.Invalidate();

[Visual Basic]
gridDesktop1.Worksheets(0).Cells(0, 0).Value = "2"
gridDesktop1.Worksheets(0).Cells(1, 0).Value = "3"
gridDesktop1.Worksheets(0).Cells(2, 1).Value = "=a1*a2"
gridDesktop1.RunAllFormulas()
gridDesktop1.Invalidate()

```

### Se även

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


