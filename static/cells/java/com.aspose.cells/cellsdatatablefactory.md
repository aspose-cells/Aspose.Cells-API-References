##CellsDataTableFactory
Utility to build ICellsDataTable from custom objects for users convenience.
**Inheritance:**
java.lang.Object
```
public class CellsDataTableFactory
```
Utility to build ICellsDataTable from custom objects for user's convenience.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getInstance(double[] vals, boolean vertial)](#getInstance-double---boolean-) | Creates ICellsDataTable from given sequence of double values. |
| [getInstance(double[] vals, String[] columnNames)](#getInstance-double---java.lang.String---) | Creates ICellsDataTable from given sequence of double values. |
| [getInstance(double[][] vals)](#getInstance-double-----) | Creates ICellsDataTable from given 2D array. |
| [getInstance(int[] vals, boolean vertial)](#getInstance-int---boolean-) | Creates ICellsDataTable from given sequence of int values. |
| [getInstance(int[] vals, String[] columnNames)](#getInstance-int---java.lang.String---) | Creates ICellsDataTable from given sequence of int values. |
| [getInstance(int[][] vals)](#getInstance-int-----) | Creates ICellsDataTable from given 2D array. |
| [getInstance(Object[] vals, boolean vertial)](#getInstance-java.lang.Object---boolean-) | Creates ICellsDataTable from given sequence of objects. |
| [getInstance(Object[] vals, String[] columnNames)](#getInstance-java.lang.Object---java.lang.String---) | Creates ICellsDataTable from given sequence of objects. |
| [getInstance(Object[][] vals)](#getInstance-java.lang.Object-----) | Creates ICellsDataTable from given 2D array. |
| [getInstance(Object[][] vals, boolean hasHeader, String[] columnNames)](#getInstance-java.lang.Object-----boolean-java.lang.String---) | Creates ICellsDataTable from given sequence of objects. |
| [getInstance(Collection collection)](#getInstance-java.util.Collection-) | Creates ICellsDataTable from given collection. |
| [getInstance(Collection collection, boolean hasHeader)](#getInstance-java.util.Collection-boolean-) | Creates ICellsDataTable from given collection. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getInstance(double[] vals, boolean vertial) {#getInstance-double---boolean-}
```
public ICellsDataTable getInstance(double[] vals, boolean vertial)
```
Creates ICellsDataTable from given sequence of double values.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vals | double[] | double values to build table |
| vertial | boolean | whether build table by the double values vertiacally(true) or horizontally(false) |
**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(double[] vals, String[] columnNames) {#getInstance-double---java.lang.String---}
```
public ICellsDataTable getInstance(double[] vals, String[] columnNames)
```
Creates ICellsDataTable from given sequence of double values.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vals | double[] | double values to build table |
| columnNames | java.lang.String[] | Column names of the table. Its length can only be either 1(build table by the double values vertically) or length of the double values(build table by the double values horizontally) |
**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(double[][] vals) {#getInstance-double-----}
```
public ICellsDataTable getInstance(double[][] vals)
```
Creates ICellsDataTable from given 2D array.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vals | double[][] | double values to build table |
**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(int[] vals, boolean vertial) {#getInstance-int---boolean-}
```
public ICellsDataTable getInstance(int[] vals, boolean vertial)
```
Creates ICellsDataTable from given sequence of int values.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vals | int[] | int values to build table |
| vertial | boolean | whether build table by the int values vertiacally(true) or horizontally(false) |
**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(int[] vals, String[] columnNames) {#getInstance-int---java.lang.String---}
```
public ICellsDataTable getInstance(int[] vals, String[] columnNames)
```
Creates ICellsDataTable from given sequence of int values.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vals | int[] | int values to build table |
| columnNames | java.lang.String[] | Column names of the table. Its length can only be either 1(build table by the int values vertically) or length of the int values(build table by the int values horizontally) |
**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(int[][] vals) {#getInstance-int-----}
```
public ICellsDataTable getInstance(int[][] vals)
```
Creates ICellsDataTable from given 2D array.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vals | int[][] | int values to build table |
**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Object[] vals, boolean vertial) {#getInstance-java.lang.Object---boolean-}
```
public ICellsDataTable getInstance(Object[] vals, boolean vertial)
```
Creates ICellsDataTable from given sequence of objects.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vals | java.lang.Object[] | objects to build table |
| vertial | boolean | whether build table by the objects vertiacally(true) or horizontally(false) |
**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Object[] vals, String[] columnNames) {#getInstance-java.lang.Object---java.lang.String---}
```
public ICellsDataTable getInstance(Object[] vals, String[] columnNames)
```
Creates ICellsDataTable from given sequence of objects.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vals | java.lang.Object[] | objects to build table |
| columnNames | java.lang.String[] | Column names of the table. Its length can only be either 1(build table by the objects vertically) or length of the objects(build table by the objects horizontally) |
**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Object[][] vals) {#getInstance-java.lang.Object-----}
```
public ICellsDataTable getInstance(Object[][] vals)
```
Creates ICellsDataTable from given 2D array.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vals | java.lang.Object[][] | objects to build table |
**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Object[][] vals, boolean hasHeader, String[] columnNames) {#getInstance-java.lang.Object-----boolean-java.lang.String---}
```
public ICellsDataTable getInstance(Object[][] vals, boolean hasHeader, String[] columnNames)
```
Creates ICellsDataTable from given sequence of objects.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vals | java.lang.Object[][] | objects to build table |
| hasHeader | boolean | Indicates whether the first row is header row. |
| columnNames | java.lang.String[] | Column names of the table. Its length can only be either 1(build table by the objects vertically) or length of the objects(build table by the objects horizontally) |
**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Collection collection) {#getInstance-java.util.Collection-}
```
public ICellsDataTable getInstance(Collection collection)
```
Creates ICellsDataTable from given collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| collection | java.util.Collection | the collection to build table |
**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### getInstance(Collection collection, boolean hasHeader) {#getInstance-java.util.Collection-boolean-}
```
public ICellsDataTable getInstance(Collection collection, boolean hasHeader)
```
Creates ICellsDataTable from given collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| collection | java.util.Collection | the collection to build table |
| hasHeader | boolean | Indicates whether the first row is header |
**Returns:**
[ICellsDataTable](../../com.aspose.cells/icellsdatatable) - Instance of ICellsDataTable
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
