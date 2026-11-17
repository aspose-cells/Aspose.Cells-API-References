---
title: "Classe PivotArea"
linktitle: "PivotArea"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe PivotArea. Incapsula l'oggetto che rappresenta pivotarea in Go."
type: docs
weight: 200
url: /it/go-cpp/pivotarea/
---

## PivotArea class

Presenta l'area selezionata della tabella pivot.

```go

type PivotArea struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewPivotArea](./newpivotarea/) | Presenta l'area selezionata della PivotTable. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetFilters](./getfilters/) | Ottiene tutti i filtri per questa PivotArea. |
| [Select](./select/) | Seleziona l'area con i filtri. |
| [SelectField_PivotFieldType_String](./selectfield_pivotfieldtype_string/) | Seleziona un campo nella regione come area. |
| [SelectField_PivotFieldType_PivotField](./selectfield_pivotfieldtype_pivotfield/) | Seleziona un campo nella regione come area. |
| [GetOnlyData](./getonlydata/) | Indica se sono selezionati solo i valori dei dati (nell'area dati della vista) per una selezione di elementi e non includono le etichette degli elementi. |
| [SetOnlyData](./setonlydata/) | Indica se sono selezionati solo i valori dei dati (nell'area dati della vista) per una selezione di elementi e non includono le etichette degli elementi. |
| [GetOnlyLabel](./getonlylabel/) | Indica se sono selezionate solo le etichette dei dati per una selezione di elementi. |
| [SetOnlyLabel](./setonlylabel/) | Indica se sono selezionate solo le etichette dei dati per una selezione di elementi. |
| [IsRowGrandIncluded](./isrowgrandincluded/) | Indica se il totale generale della riga è incluso. |
| [SetIsRowGrandIncluded](./setisrowgrandincluded/) | Indica se il totale generale della riga è incluso. |
| [IsColumnGrandIncluded](./iscolumngrandincluded/) | Indica se il totale generale della colonna è incluso. |
| [SetIsColumnGrandIncluded](./setiscolumngrandincluded/) | Indica se il totale generale della colonna è incluso. |
| [GetAxisType](./getaxistype/) | Ottiene e imposta la regione della PivotTable a cui si applica questa regola. |
| [SetAxisType](./setaxistype/) | Ottiene e imposta la regione della PivotTable a cui si applica questa regola. |
| [GetRuleType](./getruletype/) | Ottiene e imposta il tipo di regola di selezione. |
| [SetRuleType](./setruletype/) | Ottiene e imposta il tipo di regola di selezione. |
| [IsOutline](./isoutline/) | Indica se la regola si riferisce a un'area in modalità contorno. |
| [SetIsOutline](./setisoutline/) | Indica se la regola si riferisce a un'area in modalità contorno. |
| [GetCellAreas](./getcellareas/) | Ottiene le aree delle celle di quest'area pivot. |
