---
title: "PivotArea Klasse"
linktitle: "PivotArea"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PivotArea Klasse. Kapselt das Objekt, das pivotarea in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/pivotarea/
---

## PivotArea class

Stellt den ausgewählten Bereich der Pivot‑Tabelle dar.

```go

type PivotArea struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewPivotArea](./newpivotarea/) | Stellt den ausgewählten Bereich der PivotTable dar. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetFilters](./getfilters/) | Erhält alle Filter für diese PivotArea. |
| [Select](./select/) | Wählen Sie den Bereich mit Filtern aus. |
| [SelectField_PivotFieldType_String](./selectfield_pivotfieldtype_string/) | Wählen Sie ein Feld in der Region als Bereich aus. |
| [SelectField_PivotFieldType_PivotField](./selectfield_pivotfieldtype_pivotfield/) | Wählen Sie ein Feld in der Region als Bereich aus. |
| [GetOnlyData](./getonlydata/) | Gibt an, ob nur die Datenwerte (im Datenbereich der Ansicht) für eine ItemSelection ausgewählt sind und die Elementbeschriftungen nicht enthalten. |
| [SetOnlyData](./setonlydata/) | Gibt an, ob nur die Datenwerte (im Datenbereich der Ansicht) für eine ItemSelection ausgewählt sind und die Elementbeschriftungen nicht enthalten. |
| [GetOnlyLabel](./getonlylabel/) | Gibt an, ob nur die Datenbeschriftungen für eine ItemSelection ausgewählt sind. |
| [SetOnlyLabel](./setonlylabel/) | Gibt an, ob nur die Datenbeschriftungen für eine ItemSelection ausgewählt sind. |
| [IsRowGrandIncluded](./isrowgrandincluded/) | Gibt an, ob die Gesamtsumme der Zeile enthalten ist. |
| [SetIsRowGrandIncluded](./setisrowgrandincluded/) | Gibt an, ob die Gesamtsumme der Zeile enthalten ist. |
| [IsColumnGrandIncluded](./iscolumngrandincluded/) | Gibt an, ob die Gesamtsumme der Spalte enthalten ist. |
| [SetIsColumnGrandIncluded](./setiscolumngrandincluded/) | Gibt an, ob die Gesamtsumme der Spalte enthalten ist. |
| [GetAxisType](./getaxistype/) | Liest und setzt den Bereich der PivotTable, auf den diese Regel angewendet wird. |
| [SetAxisType](./setaxistype/) | Liest und setzt den Bereich der PivotTable, auf den diese Regel angewendet wird. |
| [GetRuleType](./getruletype/) | Liest und setzt den Typ der Auswahlregel. |
| [SetRuleType](./setruletype/) | Liest und setzt den Typ der Auswahlregel. |
| [IsOutline](./isoutline/) | Gibt an, ob sich die Regel auf einen Bereich bezieht, der im Gliederungsmodus ist. |
| [SetIsOutline](./setisoutline/) | Gibt an, ob sich die Regel auf einen Bereich bezieht, der im Gliederungsmodus ist. |
| [GetCellAreas](./getcellareas/) | Liest Zellbereiche dieses Pivot-Bereichs. |
