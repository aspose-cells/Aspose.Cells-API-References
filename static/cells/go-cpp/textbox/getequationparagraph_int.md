##GetEquationParagraph_Int Method
'GetEquationParagraph_Int method. Encapsulates the function that represents getequationparagraph in Go.'
## GetEquationParagraph_Int function
Get the specified math paragraph from the TextBody property of the TextBox object.Notice:(1) Returns NULL when the index is out of bounds or not found.(2) Also returns NULL if the specified index position is not a math paragraph.
```go
func (instance *TextBox) GetEquationParagraph_Int(index int32)  (*EquationNode,  error)
```
## Remarks
## See Also
* Class [TextBox](../)
* Library [Aspose.Cells for Go](../../)
