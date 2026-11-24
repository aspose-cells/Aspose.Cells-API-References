---
title: "GridValidation.GetListValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridValidation-Methode. Gibt den Wert für die Liste der Validierung für die angegebene Zelle zurück"
type: docs
url: /de/net/aspose.cells.gridweb.data/gridvalidation/getlistvalue/
---
## GridValidation.GetListValue method

Liest den Wert für die Liste der Validierung für die angegebene Zelle.

```csharp
public object GetListValue(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |

### Rückgabewert

Der Wert, um die Liste dieser Validierung für die angegebene Zelle zu erzeugen. Wenn die Liste auf einen Bereich verweist, wird der zurückgegebene Wert ein ReferredArea-Objekt sein; andernfalls kann der zurückgegebene Wert null, object[] oder ein einfaches Objekt sein.

### Hinweise

Nur für Validierungen, deren Typ List ist und die auf die angegebene Zelle angewendet wurden; andernfalls wird null zurückgegeben.

### Siehe auch

* class [GridValidation](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


