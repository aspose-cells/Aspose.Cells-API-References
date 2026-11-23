---
title: "GridDesktop.RunAllFormulas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridDesktop méthode. Exécute toutes les formules des cellules"
type: docs
url: /fr/net/aspose.cells.griddesktop/griddesktop/runallformulas/
---
## GridDesktop.RunAllFormulas method

Exécute les formules de toutes les cellules.

```csharp
public void RunAllFormulas()
```

### Exemples

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

### Voir aussi

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


