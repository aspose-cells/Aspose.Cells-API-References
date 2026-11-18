---
title: "PivotArea klass"
linktitle: "PivotArea"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PivotArea-klass. Inkapslar objektet som representerar pivotarea i Go."
type: docs
weight: 200
url: /sv/go-cpp/pivotarea/
---

## PivotArea class

Visar det valda området i pivottabellen.

```go

type PivotArea struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewPivotArea](./newpivotarea/) | Visar det valda området i PivotTable. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetFilters](./getfilters/) | Hämtar alla filter för denna PivotArea. |
| [Select](./select/) | Välj området med filter. |
| [SelectField_PivotFieldType_String](./selectfield_pivotfieldtype_string/) | Välj ett fält i regionen som ett område. |
| [SelectField_PivotFieldType_PivotField](./selectfield_pivotfieldtype_pivotfield/) | Välj ett fält i regionen som ett område. |
| [GetOnlyData](./getonlydata/) | Indikerar om endast datavärdena (i dataområdet i vyn) för ett objektval är markerade och inte inkluderar objektetiketterna. |
| [SetOnlyData](./setonlydata/) | Indikerar om endast datavärdena (i dataområdet i vyn) för ett objektval är markerade och inte inkluderar objektetiketterna. |
| [GetOnlyLabel](./getonlylabel/) | Anger om endast datamärkningarna för ett objektval är markerade. |
| [SetOnlyLabel](./setonlylabel/) | Anger om endast datamärkningarna för ett objektval är markerade. |
| [IsRowGrandIncluded](./isrowgrandincluded/) | Anger om radens totalsumma inkluderas. |
| [SetIsRowGrandIncluded](./setisrowgrandincluded/) | Anger om radens totalsumma inkluderas. |
| [IsColumnGrandIncluded](./iscolumngrandincluded/) | Anger om kolumnens totalsumma inkluderas. |
| [SetIsColumnGrandIncluded](./setiscolumngrandincluded/) | Anger om kolumnens totalsumma inkluderas. |
| [GetAxisType](./getaxistype/) | Hämtar och anger regionen för pivottabellen som denna regel gäller för. |
| [SetAxisType](./setaxistype/) | Hämtar och anger regionen för pivottabellen som denna regel gäller för. |
| [GetRuleType](./getruletype/) | Hämtar och anger typen av urvalsregel. |
| [SetRuleType](./setruletype/) | Hämtar och anger typen av urvalsregel. |
| [IsOutline](./isoutline/) | Anger om regeln hänvisar till ett område som är i konturläge. |
| [SetIsOutline](./setisoutline/) | Anger om regeln hänvisar till ett område som är i konturläge. |
| [GetCellAreas](./getcellareas/) | Hämtar cellområden för detta pivotområde. |
