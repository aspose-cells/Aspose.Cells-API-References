##ReplaceOptions Class
'ReplaceOptions class. Encapsulates the object that represents replaceoptions in Go.'
## ReplaceOptions class
Represent the replace options.
```go
type ReplaceOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewReplaceOptions](./newreplaceoptions/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetCaseSensitive](./getcasesensitive/) | Indicates if the searched string is case sensitive. |
|[SetCaseSensitive](./setcasesensitive/) | Indicates if the searched string is case sensitive. |
|[GetMatchEntireCellContents](./getmatchentirecellcontents/) | Indicates whether to match entire cells contents |
|[SetMatchEntireCellContents](./setmatchentirecellcontents/) | Indicates whether to match entire cells contents |
|[GetRegexKey](./getregexkey/) | Indicates whether the searched key is regex. If true then the searched key will be taken as regex. |
|[SetRegexKey](./setregexkey/) | Indicates whether the searched key is regex. If true then the searched key will be taken as regex. |
|[GetFontSettings](./getfontsettings/) | The rich formatted settings for the replaced text. |
|[SetFontSettings](./setfontsettings/) | The rich formatted settings for the replaced text. |
|[GetStyleFlags](./getstyleflags/) | Gets and sets flags of applying font settings. |
|[SetStyleFlags](./setstyleflags/) | Gets and sets flags of applying font settings. |
