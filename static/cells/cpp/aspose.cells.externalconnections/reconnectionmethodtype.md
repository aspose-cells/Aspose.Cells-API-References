##Aspose::Cells::ExternalConnections::ReConnectionMethodType enum
'Aspose::Cells::ExternalConnections::ReConnectionMethodType enum. Specifies what the spreadsheet application should do when a connection fails in C++.'
## ReConnectionMethodType enum
Specifies what the spreadsheet application should do when a connection fails.
```cpp
enum class ReConnectionMethodType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Required | 1 | <br>On refresh use the existing connection information and if it ends up being invalid then get updated connection information, if available from the external connection file. |
| Always | 2 | <br>On every refresh get updated connection information from the external connection file, if available, and use that instead of the existing connection information. In this case the data refresh will fail if the external connection file is unavailable. |
| Never | 3 | <br>Never get updated connection information from the external connection file even if it is available and even if the existing connection information is invalid. |
## See Also
* Namespace [Aspose::Cells::ExternalConnections](../)
* Library [Aspose.Cells for C++](../../)
