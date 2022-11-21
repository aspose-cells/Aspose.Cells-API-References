---
title: Protection
second_title: Aspose.Cells for Java API Reference
description: Represents the various types of protection options available for a worksheet.
type: docs
weight: 442
url: /java/com.aspose.cells/protection/
---

**Inheritance:**
java.lang.Object
```
public class Protection
```

Represents the various types of protection options available for a worksheet.

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Allowing users to select locked cells of the worksheet
         worksheet.getProtection().setAllowSelectingLockedCell(true);
         //Allowing users to select unlocked cells of the worksheet
         worksheet.getProtection().setAllowSelectingUnlockedCell(true);
```
## Methods

| Method | Description |
| --- | --- |
| [copy(Protection source)](#copy-com.aspose.cells.Protection-) | Copy protection info. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDeletingColumn()](#getAllowDeletingColumn--) | Represents if the deletion of columns is allowed on a protected worksheet. |
| [getAllowDeletingRow()](#getAllowDeletingRow--) | Represents if the deletion of rows is allowed on a protected worksheet. |
| [getAllowEditingContent()](#getAllowEditingContent--) | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [getAllowEditingObject()](#getAllowEditingObject--) | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [getAllowEditingScenario()](#getAllowEditingScenario--) | Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [getAllowFiltering()](#getAllowFiltering--) | Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [getAllowFormattingCell()](#getAllowFormattingCell--) | Represents if the formatting of cells is allowed on a protected worksheet. |
| [getAllowFormattingColumn()](#getAllowFormattingColumn--) | Represents if the formatting of columns is allowed on a protected worksheet |
| [getAllowFormattingRow()](#getAllowFormattingRow--) | Represents if the formatting of rows is allowed on a protected worksheet |
| [getAllowInsertingColumn()](#getAllowInsertingColumn--) | Represents if the insertion of columns is allowed on a protected worksheet |
| [getAllowInsertingHyperlink()](#getAllowInsertingHyperlink--) | Represents if the insertion of hyperlinks is allowed on a protected worksheet |
| [getAllowInsertingRow()](#getAllowInsertingRow--) | Represents if the insertion of rows is allowed on a protected worksheet |
| [getAllowSelectingLockedCell()](#getAllowSelectingLockedCell--) | Represents if the user is allowed to select locked cells on a protected worksheet. |
| [getAllowSelectingUnlockedCell()](#getAllowSelectingUnlockedCell--) | Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [getAllowSorting()](#getAllowSorting--) | Represents if the sorting option is allowed on a protected worksheet. |
| [getAllowUsingPivotTable()](#getAllowUsingPivotTable--) | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [getClass()](#getClass--) |  |
| [getPassword()](#getPassword--) | Represents the password to protect the worksheet. |
| [getPasswordHash()](#getPasswordHash--) | Gets the hash of current password. |
| [hashCode()](#hashCode--) |  |
| [isDeletingColumnsAllowed()](#isDeletingColumnsAllowed--) | Represents if the deletion of columns is allowed on a protected worksheet. |
| [isDeletingRowsAllowed()](#isDeletingRowsAllowed--) | Represents if the deletion of rows is allowed on a protected worksheet. |
| [isEditingContentsAllowed()](#isEditingContentsAllowed--) | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [isEditingObjectsAllowed()](#isEditingObjectsAllowed--) | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [isEditingScenariosAllowed()](#isEditingScenariosAllowed--) | Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [isFilteringAllowed()](#isFilteringAllowed--) | Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [isFormattingCellsAllowed()](#isFormattingCellsAllowed--) | Represents if the formatting of cells is allowed on a protected worksheet. |
| [isFormattingColumnsAllowed()](#isFormattingColumnsAllowed--) | Represents if the formatting of columns is allowed on a protected worksheet NOTE: This member is now obsolete. |
| [isFormattingRowsAllowed()](#isFormattingRowsAllowed--) | Represents if the formatting of rows is allowed on a protected worksheet NOTE: This member is now obsolete. |
| [isInsertingColumnsAllowed()](#isInsertingColumnsAllowed--) | Represents if the insertion of columns is allowed on a protected worksheet NOTE: This member is now obsolete. |
| [isInsertingHyperlinksAllowed()](#isInsertingHyperlinksAllowed--) | Represents if the insertion of hyperlinks is allowed on a protected worksheet NOTE: This member is now obsolete. |
| [isInsertingRowsAllowed()](#isInsertingRowsAllowed--) | Represents if the insertion of rows is allowed on a protected worksheet NOTE: This member is now obsolete. |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Indicates whether the worksheets is protected with password. |
| [isSelectingLockedCellsAllowed()](#isSelectingLockedCellsAllowed--) | Represents if the user is allowed to select locked cells on a protected worksheet. |
| [isSelectingUnlockedCellsAllowed()](#isSelectingUnlockedCellsAllowed--) | Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [isSortingAllowed()](#isSortingAllowed--) | Represents if the sorting option is allowed on a protected worksheet. |
| [isUsingPivotTablesAllowed()](#isUsingPivotTablesAllowed--) | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDeletingColumn(boolean value)](#setAllowDeletingColumn-boolean-) | For the description of this property, please see [getAllowDeletingColumn()](../../com.aspose.cells/protection\#getAllowDeletingColumn--) |
| [setAllowDeletingRow(boolean value)](#setAllowDeletingRow-boolean-) | For the description of this property, please see [getAllowDeletingRow()](../../com.aspose.cells/protection\#getAllowDeletingRow--) |
| [setAllowEditingContent(boolean value)](#setAllowEditingContent-boolean-) | For the description of this property, please see [getAllowEditingContent()](../../com.aspose.cells/protection\#getAllowEditingContent--) |
| [setAllowEditingObject(boolean value)](#setAllowEditingObject-boolean-) | For the description of this property, please see [getAllowEditingObject()](../../com.aspose.cells/protection\#getAllowEditingObject--) |
| [setAllowEditingScenario(boolean value)](#setAllowEditingScenario-boolean-) | For the description of this property, please see [getAllowEditingScenario()](../../com.aspose.cells/protection\#getAllowEditingScenario--) |
| [setAllowFiltering(boolean value)](#setAllowFiltering-boolean-) | For the description of this property, please see [getAllowFiltering()](../../com.aspose.cells/protection\#getAllowFiltering--) |
| [setAllowFormattingCell(boolean value)](#setAllowFormattingCell-boolean-) | For the description of this property, please see [getAllowFormattingCell()](../../com.aspose.cells/protection\#getAllowFormattingCell--) |
| [setAllowFormattingColumn(boolean value)](#setAllowFormattingColumn-boolean-) | For the description of this property, please see [getAllowFormattingColumn()](../../com.aspose.cells/protection\#getAllowFormattingColumn--) |
| [setAllowFormattingRow(boolean value)](#setAllowFormattingRow-boolean-) | For the description of this property, please see [getAllowFormattingRow()](../../com.aspose.cells/protection\#getAllowFormattingRow--) |
| [setAllowInsertingColumn(boolean value)](#setAllowInsertingColumn-boolean-) | For the description of this property, please see [getAllowInsertingColumn()](../../com.aspose.cells/protection\#getAllowInsertingColumn--) |
| [setAllowInsertingHyperlink(boolean value)](#setAllowInsertingHyperlink-boolean-) | For the description of this property, please see [getAllowInsertingHyperlink()](../../com.aspose.cells/protection\#getAllowInsertingHyperlink--) |
| [setAllowInsertingRow(boolean value)](#setAllowInsertingRow-boolean-) | For the description of this property, please see [getAllowInsertingRow()](../../com.aspose.cells/protection\#getAllowInsertingRow--) |
| [setAllowSelectingLockedCell(boolean value)](#setAllowSelectingLockedCell-boolean-) | For the description of this property, please see [getAllowSelectingLockedCell()](../../com.aspose.cells/protection\#getAllowSelectingLockedCell--) |
| [setAllowSelectingUnlockedCell(boolean value)](#setAllowSelectingUnlockedCell-boolean-) | For the description of this property, please see [getAllowSelectingUnlockedCell()](../../com.aspose.cells/protection\#getAllowSelectingUnlockedCell--) |
| [setAllowSorting(boolean value)](#setAllowSorting-boolean-) | For the description of this property, please see [getAllowSorting()](../../com.aspose.cells/protection\#getAllowSorting--) |
| [setAllowUsingPivotTable(boolean value)](#setAllowUsingPivotTable-boolean-) | For the description of this property, please see [getAllowUsingPivotTable()](../../com.aspose.cells/protection\#getAllowUsingPivotTable--) |
| [setDeletingColumnsAllowed(boolean value)](#setDeletingColumnsAllowed-boolean-) | For the description of this property, please see [isDeletingColumnsAllowed()](../../com.aspose.cells/protection\#isDeletingColumnsAllowed--) |
| [setDeletingRowsAllowed(boolean value)](#setDeletingRowsAllowed-boolean-) | For the description of this property, please see [isDeletingRowsAllowed()](../../com.aspose.cells/protection\#isDeletingRowsAllowed--) |
| [setEditingContentsAllowed(boolean value)](#setEditingContentsAllowed-boolean-) | For the description of this property, please see [isEditingContentsAllowed()](../../com.aspose.cells/protection\#isEditingContentsAllowed--) |
| [setEditingObjectsAllowed(boolean value)](#setEditingObjectsAllowed-boolean-) | For the description of this property, please see [isEditingObjectsAllowed()](../../com.aspose.cells/protection\#isEditingObjectsAllowed--) |
| [setEditingScenariosAllowed(boolean value)](#setEditingScenariosAllowed-boolean-) | For the description of this property, please see [isEditingScenariosAllowed()](../../com.aspose.cells/protection\#isEditingScenariosAllowed--) |
| [setFilteringAllowed(boolean value)](#setFilteringAllowed-boolean-) | For the description of this property, please see [isFilteringAllowed()](../../com.aspose.cells/protection\#isFilteringAllowed--) |
| [setFormattingCellsAllowed(boolean value)](#setFormattingCellsAllowed-boolean-) | For the description of this property, please see [isFormattingCellsAllowed()](../../com.aspose.cells/protection\#isFormattingCellsAllowed--) |
| [setFormattingColumnsAllowed(boolean value)](#setFormattingColumnsAllowed-boolean-) | For the description of this property, please see [isFormattingColumnsAllowed()](../../com.aspose.cells/protection\#isFormattingColumnsAllowed--) |
| [setFormattingRowsAllowed(boolean value)](#setFormattingRowsAllowed-boolean-) | For the description of this property, please see [isFormattingRowsAllowed()](../../com.aspose.cells/protection\#isFormattingRowsAllowed--) |
| [setInsertingColumnsAllowed(boolean value)](#setInsertingColumnsAllowed-boolean-) | For the description of this property, please see [isInsertingColumnsAllowed()](../../com.aspose.cells/protection\#isInsertingColumnsAllowed--) |
| [setInsertingHyperlinksAllowed(boolean value)](#setInsertingHyperlinksAllowed-boolean-) | For the description of this property, please see [isInsertingHyperlinksAllowed()](../../com.aspose.cells/protection\#isInsertingHyperlinksAllowed--) |
| [setInsertingRowsAllowed(boolean value)](#setInsertingRowsAllowed-boolean-) | For the description of this property, please see [isInsertingRowsAllowed()](../../com.aspose.cells/protection\#isInsertingRowsAllowed--) |
| [setPassword(String value)](#setPassword-java.lang.String-) | For the description of this property, please see [getPassword()](../../com.aspose.cells/protection\#getPassword--) |
| [setSelectingLockedCellsAllowed(boolean value)](#setSelectingLockedCellsAllowed-boolean-) | For the description of this property, please see [isSelectingLockedCellsAllowed()](../../com.aspose.cells/protection\#isSelectingLockedCellsAllowed--) |
| [setSelectingUnlockedCellsAllowed(boolean value)](#setSelectingUnlockedCellsAllowed-boolean-) | For the description of this property, please see [isSelectingUnlockedCellsAllowed()](../../com.aspose.cells/protection\#isSelectingUnlockedCellsAllowed--) |
| [setSortingAllowed(boolean value)](#setSortingAllowed-boolean-) | For the description of this property, please see [isSortingAllowed()](../../com.aspose.cells/protection\#isSortingAllowed--) |
| [setUsingPivotTablesAllowed(boolean value)](#setUsingPivotTablesAllowed-boolean-) | For the description of this property, please see [isUsingPivotTablesAllowed()](../../com.aspose.cells/protection\#isUsingPivotTablesAllowed--) |
| [toString()](#toString--) |  |
| [verifyPassword(String password)](#verifyPassword-java.lang.String-) | Verifies password. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(Protection source) {#copy-com.aspose.cells.Protection-}
```
public void copy(Protection source)
```


Copy protection info.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Protection](../../com.aspose.cells/protection) |  |

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
### getAllowDeletingColumn() {#getAllowDeletingColumn--}
```
public boolean getAllowDeletingColumn()
```


Represents if the deletion of columns is allowed on a protected worksheet. The columns containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.

**Returns:**
boolean
### getAllowDeletingRow() {#getAllowDeletingRow--}
```
public boolean getAllowDeletingRow()
```


Represents if the deletion of rows is allowed on a protected worksheet. The rows containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.

**Returns:**
boolean
### getAllowEditingContent() {#getAllowEditingContent--}
```
public boolean getAllowEditingContent()
```


Represents if the user is allowed to edit contents of locked cells on a protected worksheet.

**Returns:**
boolean
### getAllowEditingObject() {#getAllowEditingObject--}
```
public boolean getAllowEditingObject()
```


Represents if the user is allowed to manipulate drawing objects on a protected worksheet.

**Returns:**
boolean
### getAllowEditingScenario() {#getAllowEditingScenario--}
```
public boolean getAllowEditingScenario()
```


Represents if the user is allowed to edit scenarios on a protected worksheet.

**Returns:**
boolean
### getAllowFiltering() {#getAllowFiltering--}
```
public boolean getAllowFiltering()
```


Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected.

**Returns:**
boolean
### getAllowFormattingCell() {#getAllowFormattingCell--}
```
public boolean getAllowFormattingCell()
```


Represents if the formatting of cells is allowed on a protected worksheet.

**Returns:**
boolean
### getAllowFormattingColumn() {#getAllowFormattingColumn--}
```
public boolean getAllowFormattingColumn()
```


Represents if the formatting of columns is allowed on a protected worksheet

**Returns:**
boolean
### getAllowFormattingRow() {#getAllowFormattingRow--}
```
public boolean getAllowFormattingRow()
```


Represents if the formatting of rows is allowed on a protected worksheet

**Returns:**
boolean
### getAllowInsertingColumn() {#getAllowInsertingColumn--}
```
public boolean getAllowInsertingColumn()
```


Represents if the insertion of columns is allowed on a protected worksheet

**Returns:**
boolean
### getAllowInsertingHyperlink() {#getAllowInsertingHyperlink--}
```
public boolean getAllowInsertingHyperlink()
```


Represents if the insertion of hyperlinks is allowed on a protected worksheet

**Returns:**
boolean
### getAllowInsertingRow() {#getAllowInsertingRow--}
```
public boolean getAllowInsertingRow()
```


Represents if the insertion of rows is allowed on a protected worksheet

**Returns:**
boolean
### getAllowSelectingLockedCell() {#getAllowSelectingLockedCell--}
```
public boolean getAllowSelectingLockedCell()
```


Represents if the user is allowed to select locked cells on a protected worksheet.

**Returns:**
boolean
### getAllowSelectingUnlockedCell() {#getAllowSelectingUnlockedCell--}
```
public boolean getAllowSelectingUnlockedCell()
```


Represents if the user is allowed to select unlocked cells on a protected worksheet.

**Returns:**
boolean
### getAllowSorting() {#getAllowSorting--}
```
public boolean getAllowSorting()
```


Represents if the sorting option is allowed on a protected worksheet.

**Returns:**
boolean
### getAllowUsingPivotTable() {#getAllowUsingPivotTable--}
```
public boolean getAllowUsingPivotTable()
```


Represents if the user is allowed to manipulate pivot tables on a protected worksheet.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPassword() {#getPassword--}
```
public String getPassword()
```


Represents the password to protect the worksheet. If password is set to null or blank string, you can unprotect the worksheet or workbook without using a password. Otherwise, you must specify the password to unprotect the worksheet or workbook.

**Returns:**
java.lang.String
### getPasswordHash() {#getPasswordHash--}
```
public int getPasswordHash()
```


Gets the hash of current password.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDeletingColumnsAllowed() {#isDeletingColumnsAllowed--}
```
public boolean isDeletingColumnsAllowed()
```


Represents if the deletion of columns is allowed on a protected worksheet. NOTE: This member is now obsolete. Instead, please use Protection.AllowDeletingColumn property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isDeletingRowsAllowed() {#isDeletingRowsAllowed--}
```
public boolean isDeletingRowsAllowed()
```


Represents if the deletion of rows is allowed on a protected worksheet. NOTE: This member is now obsolete. Instead, please use Protection.AllowDeletingRow property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isEditingContentsAllowed() {#isEditingContentsAllowed--}
```
public boolean isEditingContentsAllowed()
```


Represents if the user is allowed to edit contents of locked cells on a protected worksheet. NOTE: This member is now obsolete. Instead, please use Protection.AllowEditingContent property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isEditingObjectsAllowed() {#isEditingObjectsAllowed--}
```
public boolean isEditingObjectsAllowed()
```


Represents if the user is allowed to manipulate drawing objects on a protected worksheet. NOTE: This member is now obsolete. Instead, please use Protection.AllowEditingObject property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isEditingScenariosAllowed() {#isEditingScenariosAllowed--}
```
public boolean isEditingScenariosAllowed()
```


Represents if the user is allowed to edit scenarios on a protected worksheet. NOTE: This member is now obsolete. Instead, please use Protection.AllowEditingScenario property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isFilteringAllowed() {#isFilteringAllowed--}
```
public boolean isFilteringAllowed()
```


Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. NOTE: This member is now obsolete. Instead, please use Protection.AllowFiltering property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isFormattingCellsAllowed() {#isFormattingCellsAllowed--}
```
public boolean isFormattingCellsAllowed()
```


Represents if the formatting of cells is allowed on a protected worksheet. NOTE: This member is now obsolete. Instead, please use Protection.AllowFormattingCell property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isFormattingColumnsAllowed() {#isFormattingColumnsAllowed--}
```
public boolean isFormattingColumnsAllowed()
```


Represents if the formatting of columns is allowed on a protected worksheet NOTE: This member is now obsolete. Instead, please use Protection.AllowFormattingColumn property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isFormattingRowsAllowed() {#isFormattingRowsAllowed--}
```
public boolean isFormattingRowsAllowed()
```


Represents if the formatting of rows is allowed on a protected worksheet NOTE: This member is now obsolete. Instead, please use Protection.AllowFormattingRow property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isInsertingColumnsAllowed() {#isInsertingColumnsAllowed--}
```
public boolean isInsertingColumnsAllowed()
```


Represents if the insertion of columns is allowed on a protected worksheet NOTE: This member is now obsolete. Instead, please use Protection.AllowInsertingColumn property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isInsertingHyperlinksAllowed() {#isInsertingHyperlinksAllowed--}
```
public boolean isInsertingHyperlinksAllowed()
```


Represents if the insertion of hyperlinks is allowed on a protected worksheet NOTE: This member is now obsolete. Instead, please use Protection.AllowInsertingHyperlink property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isInsertingRowsAllowed() {#isInsertingRowsAllowed--}
```
public boolean isInsertingRowsAllowed()
```


Represents if the insertion of rows is allowed on a protected worksheet NOTE: This member is now obsolete. Instead, please use Protection.AllowInsertingRow property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


Indicates whether the worksheets is protected with password.

**Returns:**
boolean
### isSelectingLockedCellsAllowed() {#isSelectingLockedCellsAllowed--}
```
public boolean isSelectingLockedCellsAllowed()
```


Represents if the user is allowed to select locked cells on a protected worksheet. NOTE: This member is now obsolete. Instead, please use Protection.AllowSelectingLockedCell property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isSelectingUnlockedCellsAllowed() {#isSelectingUnlockedCellsAllowed--}
```
public boolean isSelectingUnlockedCellsAllowed()
```


Represents if the user is allowed to select unlocked cells on a protected worksheet. NOTE: This member is now obsolete. Instead, please use Protection.AllowSelectingUnlockedCell property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isSortingAllowed() {#isSortingAllowed--}
```
public boolean isSortingAllowed()
```


Represents if the sorting option is allowed on a protected worksheet. NOTE: This member is now obsolete. Instead, please use Protection.AllowSorting property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isUsingPivotTablesAllowed() {#isUsingPivotTablesAllowed--}
```
public boolean isUsingPivotTablesAllowed()
```


Represents if the user is allowed to manipulate pivot tables on a protected worksheet. NOTE: This member is now obsolete. Instead, please use Protection.AllowUsingPivotTable property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllowDeletingColumn(boolean value) {#setAllowDeletingColumn-boolean-}
```
public void setAllowDeletingColumn(boolean value)
```


For the description of this property, please see [getAllowDeletingColumn()](../../com.aspose.cells/protection\#getAllowDeletingColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowDeletingRow(boolean value) {#setAllowDeletingRow-boolean-}
```
public void setAllowDeletingRow(boolean value)
```


For the description of this property, please see [getAllowDeletingRow()](../../com.aspose.cells/protection\#getAllowDeletingRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowEditingContent(boolean value) {#setAllowEditingContent-boolean-}
```
public void setAllowEditingContent(boolean value)
```


For the description of this property, please see [getAllowEditingContent()](../../com.aspose.cells/protection\#getAllowEditingContent--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowEditingObject(boolean value) {#setAllowEditingObject-boolean-}
```
public void setAllowEditingObject(boolean value)
```


For the description of this property, please see [getAllowEditingObject()](../../com.aspose.cells/protection\#getAllowEditingObject--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowEditingScenario(boolean value) {#setAllowEditingScenario-boolean-}
```
public void setAllowEditingScenario(boolean value)
```


For the description of this property, please see [getAllowEditingScenario()](../../com.aspose.cells/protection\#getAllowEditingScenario--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowFiltering(boolean value) {#setAllowFiltering-boolean-}
```
public void setAllowFiltering(boolean value)
```


For the description of this property, please see [getAllowFiltering()](../../com.aspose.cells/protection\#getAllowFiltering--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowFormattingCell(boolean value) {#setAllowFormattingCell-boolean-}
```
public void setAllowFormattingCell(boolean value)
```


For the description of this property, please see [getAllowFormattingCell()](../../com.aspose.cells/protection\#getAllowFormattingCell--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowFormattingColumn(boolean value) {#setAllowFormattingColumn-boolean-}
```
public void setAllowFormattingColumn(boolean value)
```


For the description of this property, please see [getAllowFormattingColumn()](../../com.aspose.cells/protection\#getAllowFormattingColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowFormattingRow(boolean value) {#setAllowFormattingRow-boolean-}
```
public void setAllowFormattingRow(boolean value)
```


For the description of this property, please see [getAllowFormattingRow()](../../com.aspose.cells/protection\#getAllowFormattingRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowInsertingColumn(boolean value) {#setAllowInsertingColumn-boolean-}
```
public void setAllowInsertingColumn(boolean value)
```


For the description of this property, please see [getAllowInsertingColumn()](../../com.aspose.cells/protection\#getAllowInsertingColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowInsertingHyperlink(boolean value) {#setAllowInsertingHyperlink-boolean-}
```
public void setAllowInsertingHyperlink(boolean value)
```


For the description of this property, please see [getAllowInsertingHyperlink()](../../com.aspose.cells/protection\#getAllowInsertingHyperlink--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowInsertingRow(boolean value) {#setAllowInsertingRow-boolean-}
```
public void setAllowInsertingRow(boolean value)
```


For the description of this property, please see [getAllowInsertingRow()](../../com.aspose.cells/protection\#getAllowInsertingRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowSelectingLockedCell(boolean value) {#setAllowSelectingLockedCell-boolean-}
```
public void setAllowSelectingLockedCell(boolean value)
```


For the description of this property, please see [getAllowSelectingLockedCell()](../../com.aspose.cells/protection\#getAllowSelectingLockedCell--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowSelectingUnlockedCell(boolean value) {#setAllowSelectingUnlockedCell-boolean-}
```
public void setAllowSelectingUnlockedCell(boolean value)
```


For the description of this property, please see [getAllowSelectingUnlockedCell()](../../com.aspose.cells/protection\#getAllowSelectingUnlockedCell--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowSorting(boolean value) {#setAllowSorting-boolean-}
```
public void setAllowSorting(boolean value)
```


For the description of this property, please see [getAllowSorting()](../../com.aspose.cells/protection\#getAllowSorting--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAllowUsingPivotTable(boolean value) {#setAllowUsingPivotTable-boolean-}
```
public void setAllowUsingPivotTable(boolean value)
```


For the description of this property, please see [getAllowUsingPivotTable()](../../com.aspose.cells/protection\#getAllowUsingPivotTable--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDeletingColumnsAllowed(boolean value) {#setDeletingColumnsAllowed-boolean-}
```
public void setDeletingColumnsAllowed(boolean value)
```


For the description of this property, please see [isDeletingColumnsAllowed()](../../com.aspose.cells/protection\#isDeletingColumnsAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDeletingRowsAllowed(boolean value) {#setDeletingRowsAllowed-boolean-}
```
public void setDeletingRowsAllowed(boolean value)
```


For the description of this property, please see [isDeletingRowsAllowed()](../../com.aspose.cells/protection\#isDeletingRowsAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEditingContentsAllowed(boolean value) {#setEditingContentsAllowed-boolean-}
```
public void setEditingContentsAllowed(boolean value)
```


For the description of this property, please see [isEditingContentsAllowed()](../../com.aspose.cells/protection\#isEditingContentsAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEditingObjectsAllowed(boolean value) {#setEditingObjectsAllowed-boolean-}
```
public void setEditingObjectsAllowed(boolean value)
```


For the description of this property, please see [isEditingObjectsAllowed()](../../com.aspose.cells/protection\#isEditingObjectsAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEditingScenariosAllowed(boolean value) {#setEditingScenariosAllowed-boolean-}
```
public void setEditingScenariosAllowed(boolean value)
```


For the description of this property, please see [isEditingScenariosAllowed()](../../com.aspose.cells/protection\#isEditingScenariosAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFilteringAllowed(boolean value) {#setFilteringAllowed-boolean-}
```
public void setFilteringAllowed(boolean value)
```


For the description of this property, please see [isFilteringAllowed()](../../com.aspose.cells/protection\#isFilteringAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFormattingCellsAllowed(boolean value) {#setFormattingCellsAllowed-boolean-}
```
public void setFormattingCellsAllowed(boolean value)
```


For the description of this property, please see [isFormattingCellsAllowed()](../../com.aspose.cells/protection\#isFormattingCellsAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFormattingColumnsAllowed(boolean value) {#setFormattingColumnsAllowed-boolean-}
```
public void setFormattingColumnsAllowed(boolean value)
```


For the description of this property, please see [isFormattingColumnsAllowed()](../../com.aspose.cells/protection\#isFormattingColumnsAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFormattingRowsAllowed(boolean value) {#setFormattingRowsAllowed-boolean-}
```
public void setFormattingRowsAllowed(boolean value)
```


For the description of this property, please see [isFormattingRowsAllowed()](../../com.aspose.cells/protection\#isFormattingRowsAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInsertingColumnsAllowed(boolean value) {#setInsertingColumnsAllowed-boolean-}
```
public void setInsertingColumnsAllowed(boolean value)
```


For the description of this property, please see [isInsertingColumnsAllowed()](../../com.aspose.cells/protection\#isInsertingColumnsAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInsertingHyperlinksAllowed(boolean value) {#setInsertingHyperlinksAllowed-boolean-}
```
public void setInsertingHyperlinksAllowed(boolean value)
```


For the description of this property, please see [isInsertingHyperlinksAllowed()](../../com.aspose.cells/protection\#isInsertingHyperlinksAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInsertingRowsAllowed(boolean value) {#setInsertingRowsAllowed-boolean-}
```
public void setInsertingRowsAllowed(boolean value)
```


For the description of this property, please see [isInsertingRowsAllowed()](../../com.aspose.cells/protection\#isInsertingRowsAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


For the description of this property, please see [getPassword()](../../com.aspose.cells/protection\#getPassword--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setSelectingLockedCellsAllowed(boolean value) {#setSelectingLockedCellsAllowed-boolean-}
```
public void setSelectingLockedCellsAllowed(boolean value)
```


For the description of this property, please see [isSelectingLockedCellsAllowed()](../../com.aspose.cells/protection\#isSelectingLockedCellsAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSelectingUnlockedCellsAllowed(boolean value) {#setSelectingUnlockedCellsAllowed-boolean-}
```
public void setSelectingUnlockedCellsAllowed(boolean value)
```


For the description of this property, please see [isSelectingUnlockedCellsAllowed()](../../com.aspose.cells/protection\#isSelectingUnlockedCellsAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSortingAllowed(boolean value) {#setSortingAllowed-boolean-}
```
public void setSortingAllowed(boolean value)
```


For the description of this property, please see [isSortingAllowed()](../../com.aspose.cells/protection\#isSortingAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setUsingPivotTablesAllowed(boolean value) {#setUsingPivotTablesAllowed-boolean-}
```
public void setUsingPivotTablesAllowed(boolean value)
```


For the description of this property, please see [isUsingPivotTablesAllowed()](../../com.aspose.cells/protection\#isUsingPivotTablesAllowed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### verifyPassword(String password) {#verifyPassword-java.lang.String-}
```
public boolean verifyPassword(String password)
```


Verifies password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | The password. |

**Returns:**
boolean - 
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

