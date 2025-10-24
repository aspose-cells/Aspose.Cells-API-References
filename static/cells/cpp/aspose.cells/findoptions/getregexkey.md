##Aspose::Cells::FindOptions::GetRegexKey method
'Aspose::Cells::FindOptions::GetRegexKey method. Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel in C++.'
## FindOptions::GetRegexKey method
Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel.
```cpp
bool Aspose::Cells::FindOptions::GetRegexKey()
```
## Remarks
Even though the search key has been specified as regex, it may be refactored according to specified [LookAtType](../../lookattype/). For example, when the type is [LookAtType.Contains](../../lookattype/)(this is the default value for this options), wildcards will be added at the beginning and end of the search key automatically to ensure the match will be checked as "contains". In this case, the regular expressions will become more complex and the performance will also decrease. So, for performance consideration, if user has specified the exact rule for the regex, then there is no need to use [LookAtType](../../lookattype/) as additional constraint and user may set it as [LookAtType.EntireContent](../../lookattype/) to get better performance.
## See Also
* Class [Vector](../../vector/)
* Class [FindOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
