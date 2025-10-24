##ICustomParser
Allows users to add their custom value parser for parsing string values to other proper cell value object.
```
public interface ICustomParser
```
Allows users to add their custom value parser for parsing string values to other proper cell value object.
## Methods
| Method | Description |
| --- | --- |
| [getFormat()](#getFormat--) | Gets the formatting pattern corresponding to the parsed value by last invocation of [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-). |
| [parseObject(String value)](#parseObject-java.lang.String-) | Parses given string to proper value object. |
### getFormat() {#getFormat--}
```
public abstract String getFormat()
```
Gets the formatting pattern corresponding to the parsed value by last invocation of [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-).
**Remarks**
The returned formatting pattern may be used to format corresponding cell(set to Style.Custom for the cell).
**Returns:**
java.lang.String
### parseObject(String value) {#parseObject-java.lang.String-}
```
public abstract Object parseObject(String value)
```
Parses given string to proper value object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The string value to be parsed |
**Returns:**
java.lang.Object - Parsed value object from given string. If given string cannot be parsed to proper value object, returns null.
