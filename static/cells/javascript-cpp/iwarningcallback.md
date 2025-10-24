##IWarningCallback
Callback interface of warning.
## IWarningCallback interface
Callback interface of warning.
## Methods
| Method | Description |
| --- | --- |
| [warning(WarningInfo)](#warning-warninginfo-)| Our callback only needs to implement the "Warning" method. |
### warning(WarningInfo) {#warning-warninginfo-}
Our callback only needs to implement the "Warning" method.
```javascript
warning(warningInfo: WarningInfo) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| warningInfo | [WarningInfo](../warninginfo/) | warning info |
