---
title: "GridWorksheet.FilterString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridWorksheet. Establece el filtro para la columna. Nota: debemos llamar a AddAutoFilter antes de llamar a filterString. La cadena de criterios del filtro. Nota: usamos la coma como carácter separador, por lo que el valor de celda que desea filtrar no debe contener comas. filterString10123456 significa que la columna 10 debe contener 123 o 456. filterString10123 significa que la columna 10 debe contener 123. El índice de columna se divide con comas, por ejemplo 123456789 o abc."
type: docs
url: /es/net/aspose.cells.gridweb.data/gridworksheet/filterstring/
---
## GridWorksheet.FilterString method

Establece el filtro para la columna. Observe que debemos llamar a AddAutoFilter antes de llamar a filterString. La cadena de criterios de filtro. Observe que usamos la coma-&gt;"," como carácter separador, por lo que el valor de celda que desea filtrar no debe contener comas. filterString(10,"123,456") significa que la columna 10 debe contener 123 o 456, filterString(10,"123") significa que la columna 10 debe contener 123. El índice de columna se separa con comas, p. ej. 123,456,789 o abc.

```csharp
public void FilterString(int column, string criteria)
```

### Ver también

* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


