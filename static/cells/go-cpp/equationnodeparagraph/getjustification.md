##GetJustification Method
'GetJustification method. Encapsulates the function that represents getjustification in Go.'
## GetJustification function
This specifies justification of the math paragraph (a series of adjacent equations within the same paragraph). A math paragraph can be Left Justified, Right Justified, Centered, or Centered as Group. By default, the math paragraph is Centered as Group. This means that the equations can be aligned with respect to each other, but the entire group of equations is centered as a whole.
```go
func (instance *EquationNodeParagraph) GetJustification()  (EquationHorizontalJustificationType,  error)
```
## Remarks
## See Also
* Class [EquationNodeParagraph](../)
* Library [Aspose.Cells for Go](../../)
