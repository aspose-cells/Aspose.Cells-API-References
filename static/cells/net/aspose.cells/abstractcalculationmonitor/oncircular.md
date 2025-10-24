##AbstractCalculationMonitor.OnCircular
AbstractCalculationMonitor method. Implement this method to do business when calculating formulas with circular references
## AbstractCalculationMonitor.OnCircular method
Implement this method to do business when calculating formulas with circular references.
```csharp
public virtual bool OnCircular(IEnumerator circularCellsData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| circularCellsData | IEnumerator | IEnumerator with [`CalculationCell`](../../calculationcell/) items representing cells that depend on circular references. |
### Return Value
Whether the formula engine needs to calculate those cells in circular after this call. True to let the formula engine continue to do calculation for them. False to let the formula engine just mark those cells as Calculated.
### Remarks
In the implementation user may also set the expected value as calculated result for part/all of those cells so the formula engine will not calculate them recursively.
### See Also
* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
