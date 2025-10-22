##Aspose::Cells::Drawing::Equations::EquationNode::CreateNode method
'Aspose::Cells::Drawing::Equations::EquationNode::CreateNode method. Create a node of the specified type in C++.'
## EquationNode::CreateNode method
Create a node of the specified type.
```cpp
static EquationNode Aspose::Cells::Drawing::Equations::EquationNode::CreateNode(EquationNodeType equationType, const Workbook &workbook, const EquationNode &parent)
```
| Parameter | Type | Description |
| --- | --- | --- |
| equationType | EquationNodeType | Types of Equation Nodes |
| workbook | const Workbook\& | The workbook object associated with the equation |
| parent | const EquationNode\& | The parent node where this node is located |
## ReturnValue
If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
## See Also
* Class [EquationNode](../)
* Enum [EquationNodeType](../../equationnodetype/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [Workbook](../../../aspose.cells/workbook/)
* Class [EquationNode](../)
* Namespace [Aspose::Cells::Drawing::Equations](../../)
* Library [Aspose.Cells for C++](../../../)
