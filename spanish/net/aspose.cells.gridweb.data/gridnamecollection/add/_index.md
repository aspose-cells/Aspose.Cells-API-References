---
title: "GridNameCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "GridNameCollection método. Define un nuevo nombre global"
type: docs
url: /es/net/aspose.cells.gridweb.data/gridnamecollection/add/
---
## Add(string, string) {#add_1}

Define un nuevo nombre global.

```csharp
public int Add(string text, string refersTo)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | String | Name texto. Puede tener nombre de hoja. |
| refersTo | String | La fórmula a la que se define el nombre para referirse. Debe tener un nombre de hoja. ej.'sheet hello!'A1:B2. |

### Valor de retorno

Índice del objeto Name.

### Ver también

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(int, string, string) {#add}

Define un nuevo nombre en la hoja especificada.

```csharp
public int Add(int sheetIndex, string text, string refersTo)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | Int32 | El índice de hoja en el que se aplica el nombre. |
| texto | String | Name texto. No puede tener nombre de hoja. |
| refersTo | String | La fórmula a la que se define el nombre para referirse. Debe tener un nombre de hoja. ej.'sheet hello!'A1:B2. |

### Valor de retorno

Índice del objeto Name.

### Ver también

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


