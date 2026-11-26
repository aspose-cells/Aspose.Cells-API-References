---
title: "GridDesktop.RunAllFormulas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "GridDesktop método. Ejecuta todas las fórmulas de las celdas"
type: docs
url: /es/net/aspose.cells.griddesktop/griddesktop/runallformulas/
---
## GridDesktop.RunAllFormulas method

Ejecuta todas las fórmulas de las celdas.

```csharp
public void RunAllFormulas()
```

### Ejemplos

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

### Ver también

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


