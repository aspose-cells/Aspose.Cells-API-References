##UnionRange.ApplyStyle
UnionRange method. Applies formats for a whole range
## UnionRange.ApplyStyle method
Applies formats for a whole range.
```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |
### Remarks
Each cell in this range will contains a [`Style`](../../style/) object. So this is a memory-consuming method. Please use it carefully.
### See Also
* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
