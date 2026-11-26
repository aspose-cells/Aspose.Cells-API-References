---
title: "PivotField.Top10AutoShow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotField. Configura la configuración Top10 AutoShow para este pivot field"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/top10autoshow/
---
## PivotField.Top10AutoShow method

Configura la configuración AutoShow Top10 para este campo dinámico.

```csharp
public void Top10AutoShow(bool isAutoShow, bool isTop, int count, int rankBy)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isAutoShow | Booleano | true para habilitar AutoShow; false para deshabilitar. |
| isTop | Booleano | Si es true, muestra los elementos superiores; false muestra los elementos inferiores. |
| contar | Int32 | Número de elementos superiores/inferiores a mostrar. |
| rankBy | Int32 | Índice del campo de datos usado para el ranking. Use -1 para clasificar por los propios valores del pivot item's. |

### Observaciones

Este método configura el [`PivotFieldTop10AutoShowSettings`](../../pivotfieldtop10autoshowsettings/).

Formato binario XLS: AutoShow (Top10) es la opción nativa y única compatible.

XLSX (OpenXML): El formato de archivo subyacente admite Top10 AutoShow, pero la interfaz de usuario de Excel 2007 y posteriores solo lo expone mediante el filtro Top10. Si no se requiere compatibilidad con XLS, se recomienda usar el filtro Top10 en su lugar.

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


