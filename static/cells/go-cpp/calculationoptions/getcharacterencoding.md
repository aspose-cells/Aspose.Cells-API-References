##GetCharacterEncoding Method
'GetCharacterEncoding method. Encapsulates the function that represents getcharacterencoding in Go.'
## GetCharacterEncoding function
Specifies the encoding used for encoding/decoding characters when calculating formulas.For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment.With this property user can specify the proper encoding used for those function to get the expected result.
```go
func (instance *CalculationOptions) GetCharacterEncoding()  (EncodingType,  error)
```
## Remarks
## See Also
* Class [CalculationOptions](../)
* Library [Aspose.Cells for Go](../../)
