---
title: "WebCells.SetBorders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WebCells. Establece bordes para un rango de celdas"
type: docs
url: /es/net/aspose.cells.gridweb.data/webcells/setborders/
---
## WebCells.SetBorders method

Establece bordes para un rango de celdas.

```csharp
public void SetBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, 
    SetBorderPosition position, WebBorderStyle borderStyle)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | El número de la primera fila del rango (basado en cero). |
| firstColumn | Int32 | El número de la primera columna del rango (basado en cero). |
| rowNumber | Int32 | El número de filas. |
| columnNumber | Int32 | El número de columnas. |
| posición | SetBorderPosition | La posición del borde. |
| borderStyle | WebBorderStyle | El estilo del borde. |

### Ejemplos

```csharp
[C#]
	GridWeb1.WebWorksheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1);

[VB]
	GridWeb1.WebWorksheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1)
```

### Ver también

* enum [SetBorderPosition](../../../aspose.cells.gridweb/setborderposition/)
* class [WebBorderStyle](../../../aspose.cells.gridweb/webborderstyle/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


