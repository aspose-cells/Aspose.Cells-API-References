---
title: "Worksheet.FilterString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Worksheet method. Establece el filtro para la columna. Nota: debemos llamar a AddAutoFilter antes de usar filterString. La cadena de criterios del filtro. Nota: usamos la coma como carácter separador, por lo que el valor de la celda que desea filtrar no debe contener comas. filterString10123456 significa que la columna 10 debe contener 123 o 456. filterString10123 significa que la columna 10 debe contener 123. Los valores se separan con comas, p. ej., 123456789 o abc"
type: docs
url: /es/net/aspose.cells.griddesktop/worksheet/filterstring/
---
## Worksheet.FilterString method

Establece el filtro para la columna. Nota: debemos llamar a AddAutoFilter antes de llamar a filterString. La cadena de criterios del filtro. Nota: usamos la coma-&gt;\",\" como carácter separador, por lo que el valor de celda que desea filtrar no debe contener comas. filterString(10,\"123,456\") significa que la columna 10 debe contener 123 o 456, filterString(10,\"123\") significa que la columna 10 debe contener el valor 123 separado por comas, p. ej. 123,456,789 o abc

```csharp
public void FilterString(int column, string criteria)
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


