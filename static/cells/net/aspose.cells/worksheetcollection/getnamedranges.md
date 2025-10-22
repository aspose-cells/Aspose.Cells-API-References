##WorksheetCollection.GetNamedRanges
WorksheetCollection method. Gets all predefined named ranges in the spreadsheet
## WorksheetCollection.GetNamedRanges method
Gets all pre-defined named ranges in the spreadsheet.
```csharp
public Range[] GetNamedRanges()
```
### Return Value
An array of Range objects. If the defined Name's reference is external or has multiple ranges, no Range object will be returned for this Name.
Returns null if the named range does not exist.
### See Also
* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
