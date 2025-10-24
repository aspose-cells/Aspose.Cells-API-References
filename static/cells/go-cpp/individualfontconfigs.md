##IndividualFontConfigs Class
'IndividualFontConfigs class. Encapsulates the object that represents individualfontconfigs in Go.'
## IndividualFontConfigs class
Font configs for each <see cref="Workbook"/> object.
```go
type IndividualFontConfigs struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewIndividualFontConfigs](./newindividualfontconfigs/) | Ctor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[SetFontSubstitutes](./setfontsubstitutes/) | Font substitute names for given original font name. |
|[GetFontSubstitutes](./getfontsubstitutes/) | Returns array containing font substitute names to be used if original font is not presented. |
|[SetFontFolder](./setfontfolder/) | Sets the fonts folder |
|[SetFontFolders](./setfontfolders/) | Sets the fonts folders |
|[SetFontSources](./setfontsources/) | Sets the fonts sources. |
|[GetFontSources](./getfontsources/) | Gets a copy of the array that contains the list of sources |
