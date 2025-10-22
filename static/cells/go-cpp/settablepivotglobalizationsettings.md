##SettablePivotGlobalizationSettings Class
'SettablePivotGlobalizationSettings class. Encapsulates the object that represents settablepivotglobalizationsettings in Go.'
## SettablePivotGlobalizationSettings class
Implementation of PivotGlobalizationSettings that supports user to set/change pre-defined texts.
```go
type SettablePivotGlobalizationSettings struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewSettablePivotGlobalizationSettings](./newsettablepivotglobalizationsettings/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetTextOfTotal](./gettextoftotal/) | Gets the text of "Total" label in the PivotTable.You need to override this method when the PivotTable contains two or more PivotFields in the data area. |
|[SetTextOfTotal](./settextoftotal/) | Sets the text of "Total" label in the PivotTable. |
|[GetTextOfGrandTotal](./gettextofgrandtotal/) | Gets the text of "Grand Total" label in the PivotTable. |
|[SetTextOfGrandTotal](./settextofgrandtotal/) | Sets the text of "Grand Total" label in the PivotTable. |
|[GetTextOfMultipleItems](./gettextofmultipleitems/) | Gets the text of "(Multiple Items)" label in the PivotTable. |
|[SetTextOfMultipleItems](./settextofmultipleitems/) | Sets the text of "(Multiple Items)" label in the PivotTable. |
|[GetTextOfAll](./gettextofall/) | Gets the text of "(All)" label in the PivotTable. |
|[SetTextOfAll](./settextofall/) | Sets the text of "(All)" label in the PivotTable. |
|[GetTextOfProtectedName](./gettextofprotectedname/) | Gets the text for specified protected name. |
|[SetTextOfProtectedName](./settextofprotectedname/) | Sets the text for specific protected name. |
|[GetTextOfColumnLabels](./gettextofcolumnlabels/) | Gets the text of "Column Labels" label in the PivotTable. |
|[SetTextOfColumnLabels](./settextofcolumnlabels/) | Gets the text of "Column Labels" label in the PivotTable. |
|[GetTextOfRowLabels](./gettextofrowlabels/) | Gets the text of "Row Labels" label in the PivotTable. |
|[SetTextOfRowLabels](./settextofrowlabels/) | Sets the text of "Row Labels" label in the PivotTable. |
|[GetTextOfEmptyData](./gettextofemptydata/) | Gets the text of "(blank)" label in the PivotTable. |
|[SetTextOfEmptyData](./settextofemptydata/) | Sets the text of "(blank)" label in the PivotTable. |
|[GetTextOfDataFieldHeader](./gettextofdatafieldheader/) | Gets the the text of the value area field header in the PivotTable. |
|[SetTextOfDataFieldHeader](./settextofdatafieldheader/) | Sets the the text of the value area field header in the PivotTable. |
|[GetTextOfSubTotal](./gettextofsubtotal/) | Gets the text of PivotFieldSubtotalType type in the PivotTable. |
|[SetTextOfSubTotal](./settextofsubtotal/) | Sets the text of PivotFieldSubtotalType type in the PivotTable. |
