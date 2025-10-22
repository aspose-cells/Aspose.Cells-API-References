##Aspose::Cells::Drawing::ActiveXControls::TextBoxActiveXControl::GetEnterFieldBehavior method
'Aspose::Cells::Drawing::ActiveXControls::TextBoxActiveXControl::GetEnterFieldBehavior method. Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control in C++.'
## TextBoxActiveXControl::GetEnterFieldBehavior method
Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control.
```cpp
bool Aspose::Cells::Drawing::ActiveXControls::TextBoxActiveXControl::GetEnterFieldBehavior()
```
## Examples
```cpp
if (!activeXControl.GetEnterFieldBehavior())
{
activeXControl.SetEnterFieldBehavior(true);
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [TextBoxActiveXControl](../)
* Namespace [Aspose::Cells::Drawing::ActiveXControls](../../)
* Library [Aspose.Cells for C++](../../../)
