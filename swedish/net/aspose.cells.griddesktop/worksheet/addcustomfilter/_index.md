---
title: "Worksheet.AddCustomFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Lägg till anpassat filter för det angivna radintervallet från startrad till slutrad."
type: docs
url: /sv/net/aspose.cells.griddesktop/worksheet/addcustomfilter/
---
## AddCustomFilter(int, int, object[], GridFilterOperatorType[]) {#addcustomfilter}

Lägg till anpassat filter för det angivna radintervallet från startrad till slutrad.

```csharp
public void AddCustomFilter(int startrow, int startcolumn, object[] critiras, 
    GridFilterOperatorType[] filterOperatorTypes)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startrow | Int32 | Startraden för filterintervallet. |
| startcolumn | Int32 | Startkolumnen för filterintervallet. |
| critiras | Object[] | Kriteriearrayen för kolumnerna, varje element tillämpas på respektive kolumn. |
| filterOperatorTypes | GridFilterOperatorType[] | Filteroperatortyp‑arrayen för kolumnerna, varje tillämpas på respektive kolumn |

### Se även

* enum [GridFilterOperatorType](../../../aspose.cells.griddesktop.data/gridfilteroperatortype/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## AddCustomFilter(int, string) {#addcustomfilter_1}

Lägg till anpassat filter för den angivna raden.

```csharp
public void AddCustomFilter(int row, string critira)
```

### Anmärkningar

Filterkriteriesträngen. Observera att vi använder , och ; som avgränsningstecken, så cellvärdet får inte innehålla dessa tecken. Nedan är exempel på kriteriesträngar: //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


