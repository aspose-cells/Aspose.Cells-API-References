---
title: "PivotItem Klasse"
linktitle: "PivotItem"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PivotItem Klasse. Kapselt das Objekt, das pivotitem in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/pivotitem/
---

## PivotItem class

Stellt ein Element in einem PivotField-Bericht dar.

```go

type PivotItem struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [IsHidden](./ishidden/) | Liest und setzt, ob das Pivot-Element ausgeblendet ist. |
| [SetIsHidden](./setishidden/) | Liest und setzt, ob das Pivot-Element ausgeblendet ist. |
| [GetPosition](./getposition/) | Angabe des Index dieses Elements in allen PivotItems des Feldes. |
| [SetPosition](./setposition/) | Angabe des Index dieses Elements in allen PivotItems des Feldes. |
| [GetPositionInSameParentNode](./getpositioninsameparentnode/) | Angabe des Positionsindex in den PivotItems unter demselben übergeordneten Knoten. |
| [SetPositionInSameParentNode](./setpositioninsameparentnode/) | Angabe des Positionsindex in den PivotItems unter demselben übergeordneten Knoten. |
| [Move](./move/) | Verschiebt das Element nach oben oder unten |
| [IsDetailHidden](./isdetailhidden/) | Liest und setzt, ob das Detail dieses Pivot-Elements ausgeblendet ist. |
| [SetIsDetailHidden](./setisdetailhidden/) | Liest und setzt, ob das Detail dieses Pivot-Elements ausgeblendet ist. |
| [IsCalculatedItem](./iscalculateditem/) | Gibt an, ob dieses Pivot-Element ein berechnetes Formelelement ist. |
| [GetFormula](./getformula/) | Liest die Formel dieses berechneten Elements. Funktioniert nur, wenn dieses Element ein berechnetes Element ist. |
| [IsMissing](./ismissing/) | Gibt an, ob das Element aus der Datenquelle entfernt wurde. |
| [GetStringValue](./getstringvalue/) | Liest den Zeichenkettenwert des Pivot-Elements. Wenn der Wert null ist, wird "" zurückgegeben. |
| [GetDoubleValue](./getdoublevalue/) | Liest den Doppelwert des Pivot-Elements. Wenn der Wert null oder keine Zahl ist, wird 0 zurückgegeben. |
| [GetDateTimeValue](./getdatetimevalue/) | Liest den Datums‑Uhrzeit‑Wert des Pivot-Elements. Wenn der Wert null ist, wird DateTime.MinValue zurückgegeben. |
| [GetValue](./getvalue/) | Liest den Wert des Pivot-Elements |
| [GetName](./getname/) | Liest den Namen des Pivot-Elements. |
| [SetName](./setname/) | Liest den Namen des Pivot-Elements. |
