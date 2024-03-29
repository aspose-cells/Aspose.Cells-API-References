---
title: Add
second_title: Referencia de API de Aspose.Cells para .NET
description: Agrega un hipervínculo a una celda específica o a un rango de celdas.
type: docs
weight: 30
url: /es/net/aspose.cells.gridweb.data/gridhyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Agrega un hipervínculo a una celda específica o a un rango de celdas.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| firstRow | Int32 | Primera fila del rango del hipervínculo. |
| firstColumn | Int32 | Primera columna del rango del hipervínculo. |
| totalRows | Int32 | Número de filas en este rango de hipervínculo. |
| totalColumns | Int32 | Número de columnas de este rango de hipervínculo. |
| address | String | Dirección del hipervínculo. |

### Valor_devuelto

Hyperlink índice de objetos

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

* class [GridHyperlinkCollection](../../gridhyperlinkcollection)
* espacio de nombres [Aspose.Cells.GridWeb.Data](../../gridhyperlinkcollection)
* asamblea [Aspose.Cells.GridWeb](../../../)

---

## Add(string, int, int, string) {#add_1}

Agrega un hipervínculo a una celda específica o a un rango de celdas.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| cellName | String | Nombre de la celda. |
| totalRows | Int32 | Número de filas en este rango de hipervínculo. |
| totalColumns | Int32 | Número de columnas de este rango de hipervínculo. |
| address | String | Dirección del hipervínculo. |

### Valor_devuelto

[`GridHyperlink`](../../gridhyperlink) índice de objetos

### Ver también

* class [GridHyperlinkCollection](../../gridhyperlinkcollection)
* espacio de nombres [Aspose.Cells.GridWeb.Data](../../gridhyperlinkcollection)
* asamblea [Aspose.Cells.GridWeb](../../../)

---

## Add(string, string) {#add_2}

Agrega un hipervínculo a una celda específica .

```csharp
public int Add(string cellName, string address)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| cellName | String | Nombre de la celda. |
| address | String | Dirección del hipervínculo. |

### Valor_devuelto

[`GridHyperlink`](../../gridhyperlink) índice de objetos

### Ver también

* class [GridHyperlinkCollection](../../gridhyperlinkcollection)
* espacio de nombres [Aspose.Cells.GridWeb.Data](../../gridhyperlinkcollection)
* asamblea [Aspose.Cells.GridWeb](../../../)

---

## Add(string, string, string, string, string) {#add_3}

Agrega un hipervínculo a una celda específica o a un rango de celdas.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| startCellName | String | La celda superior izquierda del rango. |
| endCellName | String | La celda inferior derecha del rango. |
| address | String | Dirección del hipervínculo. |
| textToDisplay | String | El texto que se mostrará para el hipervínculo especificado. |
| screenTip | String | El texto de la información en pantalla para el hipervínculo especificado. |

### Valor_devuelto

[`GridHyperlink`](../../gridhyperlink) índice de objetos

### Ver también

* class [GridHyperlinkCollection](../../gridhyperlinkcollection)
* espacio de nombres [Aspose.Cells.GridWeb.Data](../../gridhyperlinkcollection)
* asamblea [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
