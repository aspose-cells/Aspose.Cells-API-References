---
title: "PivotCache.CreatePivotTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotCache. Crea un informe PivotTable en una nueva hoja"
type: docs
url: /es/net/aspose.cells.gridweb.data/pivotcache/createpivottable/
---
## CreatePivotTable() {#createpivottable}

Crea un informe PivotTable en una hoja nueva.

```csharp
public PivotTable CreatePivotTable()
```

### Valor de retorno

El objeto PivotTable

### Observaciones

Al llamar a este método se creará un objeto PivotTable y una nueva hoja de cálculo. Luego se agrega el objeto PivotTable a la última posición de GridWeb.Worksheets.PivotTables. Si llama al método PivotTable.DataBind(), el informe PivotTable se dibujará en la hoja creada.

### Ver también

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(string) {#createpivottable_3}

Crea un informe PivotTable en una hoja nueva. El nombre del objeto pivotTable

```csharp
public PivotTable CreatePivotTable(string tableName)
```

### Valor de retorno

El objeto PivotTable

### Observaciones

Al llamar a este método se creará un objeto PivotTable y una nueva hoja de cálculo. Luego se agrega el objeto PivotTable a la última posición de GridWeb.Worksheets.PivotTables. Si llama al método PivotTable.DataBind(), el informe PivotTable se dibujará en la hoja creada.

### Ver también

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell) {#createpivottable_1}

Crea un informe PivotTable en la hoja objetivo.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| targetSheet | WebWorksheet | La hoja en la que se dibujará el informe pivotTable |
| targetCell | WebCell | La celda de inicio en la que se dibujará el informe pivotTable |

### Valor de retorno

El objeto PivotTable

### Observaciones

Al llamar a este método se creará un objeto PivotTable y luego se agrega el objeto PivotTable a la última posición de GridWeb.Worksheets.PivotTables. Si llama al método PivotTable.DataBind(), el informe PivotTable se dibujará en targetSheet comenzando en targetCell.

### Ver también

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell, string) {#createpivottable_2}

Crea un informe PivotTable en la hoja objetivo.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell, string tableName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| targetSheet | WebWorksheet | La hoja en la que se dibujará el informe pivotTable |
| targetCell | WebCell | La celda de inicio en la que se dibujará el informe pivotTable |
| tableName | String | El nombre del objeto pivotTable |

### Valor de retorno

El objeto PivotTable

### Observaciones

Al llamar a este método se creará un objeto PivotTable con el nombre tableName y luego se agrega el objeto PivotTable a la última posición de GridWeb.Worksheets.PivotTables. Si llama al método PivotTable.DataBind(), el informe PivotTable se dibujará en targetSheet comenzando en targetCell.

### Ver también

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


