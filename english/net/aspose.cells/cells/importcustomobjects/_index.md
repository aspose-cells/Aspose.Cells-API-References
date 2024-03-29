---
title: Cells.ImportCustomObjects
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Imports custom objects
type: docs
url: /net/aspose.cells/cells/importcustomobjects/
---
## ImportCustomObjects(ICollection, string[], bool, int, int, int, bool, string, bool) {#importcustomobjects_1}

Imports custom objects.

```csharp
public int ImportCustomObjects(ICollection list, string[] propertyNames, bool isPropertyNameShown, 
    int firstRow, int firstColumn, int rowNumber, bool insertRows, string dateFormatString, 
    bool convertStringToNumber)
```

| Parameter | Type | Description |
| --- | --- | --- |
| list | ICollection | The custom object |
| propertyNames | String[] | The property names.If it is null,we will import all properties of the object. |
| isPropertyNameShown | Boolean | Indicates whether the property name will be imported to the first row. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| rowNumber | Int32 | Number of rows to be imported. |
| insertRows | Boolean | Indicates whether extra rows are added to fit data. |
| dateFormatString | String | Date format string for cells. |
| convertStringToNumber | Boolean | Indicates if this method will try to convert string to number. |

### Return Value

Total number of rows imported.

### Remarks

The custom objects should be the same type.

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCustomObjects(ICollection, int, int, ImportTableOptions) {#importcustomobjects}

Imports custom objects.

```csharp
public int ImportCustomObjects(ICollection list, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| list | ICollection | The custom object |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| options | ImportTableOptions | The import options. |

### Return Value

Total number of rows imported.

### Remarks

The custom objects should be the same type.

### See Also

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


