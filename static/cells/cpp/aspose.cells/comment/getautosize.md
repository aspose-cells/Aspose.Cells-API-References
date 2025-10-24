##Aspose::Cells::Comment::GetAutoSize method
'Aspose::Cells::Comment::GetAutoSize method. Indicates if size of comment is adjusted automatically according to its content. Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize() in C++.'
## Comment::GetAutoSize method
Indicates if size of comment is adjusted automatically according to its content. Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize().
```cpp
bool Aspose::Cells::Comment::GetAutoSize()
```
## Examples
```cpp
if (!comment1.GetAutoSize())
{
//The size of the comment varies with the content
comment1.SetAutoSize(true);
}
```
## See Also
* Class [Vector](../../vector/)
* Class [Comment](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
