---
title: "PivotCache.CreatePivotTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotCache method. Erstellt einen PivotTable-Bericht auf einem neuen Blatt"
type: docs
url: /de/net/aspose.cells.gridweb.data/pivotcache/createpivottable/
---
## CreatePivotTable() {#createpivottable}

Erstellt einen PivotTable-Bericht in ein neues Blatt.

```csharp
public PivotTable CreatePivotTable()
```

### Rückgabewert

Das PivotTable-Objekt

### Hinweise

Durch Aufrufen dieser Methode wird ein PivotTable-Objekt und ein neues Arbeitsblatt erstellt. Anschließend wird das PivotTable-Objekt an der letzten Position von GridWeb.Worksheets.PivotTables hinzugefügt. Wenn Sie die Methode PivotTable.DataBind() aufrufen, wird der PivotTable-Bericht auf das erstellte Arbeitsblatt gezeichnet.

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(string) {#createpivottable_3}

Erstellt einen PivotTable-Bericht in ein neues Blatt. Der Name des pivotTable-Objekts

```csharp
public PivotTable CreatePivotTable(string tableName)
```

### Rückgabewert

Das PivotTable-Objekt

### Hinweise

Durch Aufrufen dieser Methode wird ein PivotTable-Objekt und ein neues Arbeitsblatt erstellt. Anschließend wird das PivotTable-Objekt an der letzten Position von GridWeb.Worksheets.PivotTables hinzugefügt. Wenn Sie die Methode PivotTable.DataBind() aufrufen, wird der PivotTable-Bericht auf das erstellte Arbeitsblatt gezeichnet.

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell) {#createpivottable_1}

Erstellt einen PivotTable-Bericht im targetSheet.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| targetSheet | WebWorksheet | Das Blatt, auf das der pivotTable-Bericht gezeichnet wird |
| targetCell | WebCell | Die Startzelle, auf die der pivotTable-Bericht gezeichnet wird |

### Rückgabewert

Das PivotTable-Objekt

### Hinweise

Durch Aufrufen dieser Methode wird ein PivotTable-Objekt erstellt. Anschließend wird das PivotTable-Objekt an der letzten Position von GridWeb.Worksheets.PivotTables hinzugefügt. Wenn Sie die Methode PivotTable.DataBind() aufrufen, wird der PivotTable-Bericht auf das targetSheet beginnend bei der targetCell gezeichnet.

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell, string) {#createpivottable_2}

Erstellt einen PivotTable-Bericht im targetSheet.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| targetSheet | WebWorksheet | Das Blatt, auf das der pivotTable-Bericht gezeichnet wird |
| targetCell | WebCell | Die Startzelle, auf die der pivotTable-Bericht gezeichnet wird |
| tableName | String | Der Name des pivotTable-Objekts |

### Rückgabewert

Das PivotTable-Objekt

### Hinweise

Durch Aufrufen dieser Methode wird ein PivotTable-Objekt mit dem Namen tableName erstellt. Anschließend wird das PivotTable-Objekt an der letzten Position von GridWeb.Worksheets.PivotTables hinzugefügt. Wenn Sie die Methode PivotTable.DataBind() aufrufen, wird der PivotTable-Bericht auf das targetSheet beginnend bei der targetCell gezeichnet.

### Siehe auch

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


