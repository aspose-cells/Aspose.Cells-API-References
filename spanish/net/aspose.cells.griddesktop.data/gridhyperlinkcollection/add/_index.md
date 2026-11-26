---
title: "GridHyperlinkCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridHyperlinkCollection. Añade un hipervínculo a una celda especificada o a un rango de celdas"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridhyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Agrega un hipervínculo a una celda especificada o a un rango de celdas.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | Primera fila del rango de hipervínculo. |
| firstColumn | Int32 | Primera columna del rango de hipervínculo. |
| totalRows | Int32 | Número de filas en este rango de hipervínculo. |
| totalColumns | Int32 | Número de columnas de este rango de hipervínculo. |
| address | String | Dirección del hipervínculo. |

### Valor de retorno

Índice del objeto hipervínculo.

### Ejemplos

```csharp
[C#]

Worksheet worksheet = excel.Worksheets[0];
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com");
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls");

[Visual Basic]

Dim worksheet as Worksheet = excel.Worksheets(0)
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com")
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls")

```

### Ver también

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, int, int, string) {#add_1}

Agrega un hipervínculo a una celda especificada o a un rango de celdas.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | Nombre de la celda. |
| totalRows | Int32 | Número de filas en este rango de hipervínculo. |
| totalColumns | Int32 | Número de columnas de este rango de hipervínculo. |
| address | String | Dirección del hipervínculo. |

### Valor de retorno

Índice del objeto hipervínculo.

### Ver también

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, string) {#add_2}

Agrega un hipervínculo a una celda especificada.

```csharp
public int Add(string cellName, string address)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | Nombre de la celda. |
| address | String | Dirección del hipervínculo. |

### Valor de retorno

Índice del objeto hipervínculo.

### Ver también

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, string, string, string, string) {#add_3}

Agrega un hipervínculo a una celda especificada o a un rango de celdas.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startCellName | String | La celda superior izquierda del rango. |
| endCellName | String | La celda inferior derecha del rango. |
| address | String | Dirección del hipervínculo. |
| textToDisplay | String | El texto que se mostrará para el hipervínculo especificado. |
| screenTip | String | El texto screenTip para el hipervínculo especificado. |

### Valor de retorno

Índice del objeto hipervínculo.

### Ver también

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, string) {#add_4}

Agrega un hipervínculo a una celda especificada en el índice de fila y columna.

```csharp
public void Add(int row, int col, string url)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila de la celda. |
| col | Int32 | Índice de columna de la celda. |
| url | String | URL del hipervínculo. |

### Ver también

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


