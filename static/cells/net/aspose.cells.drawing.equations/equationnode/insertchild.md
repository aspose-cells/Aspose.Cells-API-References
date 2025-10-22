##EquationNode.InsertChild
EquationNode method. Inserts a node of the specified type at the specified index position in the current nodes child node list
## EquationNode.InsertChild method
Inserts a node of the specified type at the specified index position in the current node's child node list.
```csharp
public EquationNode InsertChild(int index, EquationNodeType equationType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | index value |
| equationType | EquationNodeType | Types of Equation Nodes |
### Return Value
If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### See Also
* enum [EquationNodeType](../../equationnodetype/)
* class [EquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)
