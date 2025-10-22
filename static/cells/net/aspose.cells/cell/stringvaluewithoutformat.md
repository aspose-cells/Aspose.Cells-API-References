##Cell.StringValueWithoutFormat
Cell property. Gets cells value as string without any format
## Cell.StringValueWithoutFormat property
Gets cell's value as string without any format.
```csharp
[Obsolete("Use GetStringValue(CellValueFormatStrategy) with CellValueFormatStrategy.None instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValueWithoutFormat { get; }
```
### Remarks
NOTE: This method is now obsolete. Instead, User should get the value object and format it according to the value type and the specific requirement. This property will be removed 12 months later since December 2020. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
