---
title: "Clase PivotGlobalizationSettings"
linktitle: "PivotGlobalizationSettings"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase PivotGlobalizationSettings. Encapsula el objeto que representa pivotglobalizationsettings en Go."
type: docs
weight: 200
url: /es/go-cpp/pivotglobalizationsettings/
---

## PivotGlobalizationSettings class

Represents the globalization settings for pivot tables.

```go

type PivotGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewPivotGlobalizationSettings](./newpivotglobalizationsettings/) | Default constructor. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetTextOfTotal](./gettextoftotal/) | Obtiene el texto de la etiqueta "Total" en la PivotTable. Necesita sobrescribir este método cuando la PivotTable contiene dos o más PivotFields en el área de datos. |
| [GetTextOfGrandTotal](./gettextofgrandtotal/) | Obtiene el texto de la etiqueta "Grand Total" en la PivotTable. |
| [GetTextOfMultipleItems](./gettextofmultipleitems/) | Obtiene el texto de la etiqueta "(Multiple Items)" en la PivotTable. |
| [GetTextOfAll](./gettextofall/) | Obtiene el texto de la etiqueta "(All)" en la PivotTable. |
| [GetTextOfProtectedName](./gettextofprotectedname/) | Obtiene el texto para el nombre protegido especificado. |
| [GetTextOfColumnLabels](./gettextofcolumnlabels/) | Obtiene el texto de la etiqueta "Column Labels" en la PivotTable. |
| [GetTextOfRowLabels](./gettextofrowlabels/) | Obtiene el texto de la etiqueta "Row Labels" en la PivotTable. |
| [GetTextOfEmptyData](./gettextofemptydata/) | Obtiene el texto de la etiqueta "(blank)" en la PivotTable. |
| [GetTextOfDataFieldHeader](./gettextofdatafieldheader/) | Obtiene el texto del encabezado del campo del área de valores en la PivotTable. |
| [GetShortTextOf12Months](./getshorttextof12months/) | Obtiene todas las cadenas formateadas cortas de los 12 meses. |
| [GetTextOf24Hours](./gettextof24hours/) | Obtiene todas las cadenas formateadas localmente de 24 horas. El valor predeterminado es 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM. |
| [GetTextOfOr](./gettextofor/) | Obtiene todas las cadenas formateadas localmente de "or". |
| [GetFormatOfDayGroup](./getformatofdaygroup/) | Obtiene el formato numérico del grupo de día de pivote. Solo se usa al agrupar el campo pivote por días. El valor predeterminado es "d-MMM"; |
| [GetTextOf4Quaters](./gettextof4quaters/) | Obtiene el texto local de 4 trimestres. |
| [GetTextOf4Quarters](./gettextof4quarters/) | Obtiene el texto local de 4 trimestres. |
| [GetTextOfYears](./gettextofyears/) | Obtiene el texto local de "Years". |
| [GetTextOfQuarters](./gettextofquarters/) | Obtenga el texto local de "Quarters". |
| [GetTextOfMonths](./gettextofmonths/) | Obtiene el texto local de "Months". |
| [GetTextOfDays](./gettextofdays/) | Obtiene el texto local de "Days". |
| [GetTextOfHours](./gettextofhours/) | Obtiene el texto local de "Hours". |
| [GetTextOfMinutes](./gettextofminutes/) | Obtiene el texto local de "Minutes". |
| [GetTextOfSeconds](./gettextofseconds/) | Obtiene el texto local de "Seconds" |
| [GetTextOfRange](./gettextofrange/) | Obtiene el texto local de "Range" |
| [GetTextOfAllPeriods](./gettextofallperiods/) | Obtiene el texto local de "All Periods" |
| [GetTextOfSubTotal](./gettextofsubtotal/) | Obtiene el texto del tipo PivotFieldSubtotalType en la PivotTable. |
| [GetNameOfDataField](./getnameofdatafield/) | Obtiene el nombre para mostrar del campo pivote de datos.El formato predeterminado es "Sum Of Field". |
