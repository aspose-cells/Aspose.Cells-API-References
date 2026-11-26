---
title: "PivotFieldGroupOptions.GroupType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFieldGroupOptions. Obtiene o establece el tipo de agrupación para el campo dinámico. Solo para agrupar campos dinámicos de fecha y hora"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldgroupoptions/grouptype/
---
## PivotFieldGroupOptions.GroupType property

Obtiene o establece el tipo de agrupación para el campo dinámico. Solo para campos dinámicos de fecha y hora.

```csharp
public PivotGroupByType GroupType { get; set; }
```

### Ejemplos

```csharp
//init
PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
// Agrupar por año y mes juntos
PivotGroupByType pivotGroupByType = pivotFieldGroupOptions.GroupType;
pivotGroupByType = PivotGroupByType.Years | PivotGroupByType.Months;
pivotFieldGroupOptions.GroupType = pivotGroupByType;
```

### Ver también

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotFieldGroupOptions](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


