##ISmartMarkerCallBack
Represents callback interface of processing smartmarker.
```
public interface ISmartMarkerCallBack
```
Represents callback interface of processing smartmarker.
## Methods
| Method | Description |
| --- | --- |
| [process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)](#process-int-int-int-java.lang.String-java.lang.String-) | Callback for processing a smart marker. |
### process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName) {#process-int-int-int-java.lang.String-java.lang.String-}
```
public abstract void process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)
```
Callback for processing a smart marker.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | int | The sheet index. |
| rowIndex | int | The row index. |
| colIndex | int | The column index. |
| tableName | java.lang.String | The table name of smartmarker. |
| columnName | java.lang.String | The table name of smartmarker. |
