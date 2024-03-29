---
title: WorksheetCollection.RegisterAddInFunction
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Adds addin function into the workbook
type: docs
url: /net/aspose.cells/worksheetcollection/registeraddinfunction/
---
## RegisterAddInFunction(string, string, bool) {#registeraddinfunction}

Adds addin function into the workbook

```csharp
public int RegisterAddInFunction(string addInFile, string functionName, bool lib)
```

| Parameter | Type | Description |
| --- | --- | --- |
| addInFile | String | the file contains the addin functions |
| functionName | String | the addin function name |
| lib | Boolean | whether the given addin file is in the directory or sub-directory of Workbook Add-In library. This flag takes effect and makes difference when given addInFile is of relative path: true denotes the path is relative to Add-In library and false denotes the path is relative to this Workbook. |

### Return Value

ID of the data which contains given addin function

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RegisterAddInFunction(int, string) {#registeraddinfunction_1}

Adds addin function into the workbook

```csharp
public string RegisterAddInFunction(int id, string functionName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| id | Int32 | ID of the data which contains addin functions, can be got by the first call of `RegisterAddInFunction` for the same addin file. |
| functionName | String | the addin function name |

### Return Value

URL of the addin file which contains addin functions

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


