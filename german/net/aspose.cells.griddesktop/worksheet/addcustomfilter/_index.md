---
title: "Worksheet.AddCustomFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Fügt einen benutzerdefinierten Filter für den angegebenen Zeilenbereich vom Startzeile bis zur Endzeile hinzu."
type: docs
url: /de/net/aspose.cells.griddesktop/worksheet/addcustomfilter/
---
## AddCustomFilter(int, int, object[], GridFilterOperatorType[]) {#addcustomfilter}

Fügt einen benutzerdefinierten Filter für den angegebenen Zeilenbereich vom Start‑ bis zum End‑Zeile hinzu.

```csharp
public void AddCustomFilter(int startrow, int startcolumn, object[] critiras, 
    GridFilterOperatorType[] filterOperatorTypes)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startrow | Int32 | Die startrow des Filterbereichs. |
| startcolumn | Int32 | Die startcolumn des Filterbereichs. |
| critiras | Object[] | Das critira-Array für die Spalten, jedes wird auf die jeweilige Spalte angewendet. |
| filterOperatorTypes | GridFilterOperatorType[] | Das filter operate type-Array für die Spalten, jedes wird auf die jeweilige Spalte angewendet. |

### Siehe auch

* enum [GridFilterOperatorType](../../../aspose.cells.griddesktop.data/gridfilteroperatortype/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## AddCustomFilter(int, string) {#addcustomfilter_1}

Fügt einen benutzerdefinierten Filter für die angegebene Zeile hinzu.

```csharp
public void AddCustomFilter(int row, string critira)
```

### Hinweise

Der Filterkriterien-String. Hinweis: Wir verwenden , und ; als Trennzeichen, sodass der Zellenwert diese Trennzeichen nicht enthalten darf. Nachfolgend Beispiele für den Kriterien-String: //Spalte 0 mit Wert 12.3 CELL0 = 12.3 //Spalte 1 mit Wert ABC CELL1 = ABC //Spalte 0 mit Wert 123 oder 456 oder ABC und Spalte 1 mit Wert ABC CELL0 = 123,456,ABC; CELL1 = ABC

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


