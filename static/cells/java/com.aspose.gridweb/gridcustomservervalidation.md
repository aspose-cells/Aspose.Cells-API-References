##GridCustomServerValidation
the interface you need to implement when use server side validation.
```
public interface GridCustomServerValidation
```
the interface you need to implement when use server side validation. CustomServerFunction.
## Methods
| Method | Description |
| --- | --- |
| [validate(GridWorksheet sheet, int row, int col, String value)](#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-) | **Remarks** |
### validate(GridWorksheet sheet, int row, int col, String value) {#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-}
```
public abstract String validate(GridWorksheet sheet, int row, int col, String value)
```
**Remarks**
if return string.empty the validate is passed,else you can return any related message which can be deal in ClientCallback function
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | the GridWorksheet |
| row | int | the row index of the cell |
| col | int | the column index of the cell |
| value | java.lang.String | the value to do validation |
**Returns:**
java.lang.String - string based result value
