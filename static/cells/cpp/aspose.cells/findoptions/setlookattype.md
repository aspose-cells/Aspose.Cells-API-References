##Aspose::Cells::FindOptions::SetLookAtType method
'Aspose::Cells::FindOptions::SetLookAtType method. Look at type in C++.'
## FindOptions::SetLookAtType method
Look at type.
```cpp
void Aspose::Cells::FindOptions::SetLookAtType(LookAtType value)
```
## Remarks
When RegexKey is true and user has specified the exact rule for the regex, for performance consideration this property should be set as [LookAtType.EntireContent](../../lookattype/). Otherwise we will refactor the search key to ensure it can be matched according to the specific type. For example, when the type is [LookAtType.Contains](../../lookattype/)(this is the default value for this property), we will add wildcards at the beginning and end of the search key automatically. In this case, the regular expressions will become more complex and the performance will also decrease.
## See Also
* Class [Vector](../../vector/)
* Enum [LookAtType](../../lookattype/)
* Class [FindOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
