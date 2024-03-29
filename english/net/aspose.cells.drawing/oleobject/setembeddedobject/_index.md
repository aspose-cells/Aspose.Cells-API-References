---
title: OleObject.SetEmbeddedObject
second_title: Aspose.Cells for .NET API Reference
description: OleObject method. Sets embedded object data
type: docs
url: /net/aspose.cells.drawing/oleobject/setembeddedobject/
---
## SetEmbeddedObject(bool, byte[], string, bool, string) {#setembeddedobject}

Sets embedded object data.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label)
```

| Parameter | Type | Description |
| --- | --- | --- |
| linkToFile | Boolean | Indicates whether the object links to the file. If true, the parameter objectData is ignored. |
| objectData | Byte[] | The embedded object data. |
| sourceFileName | String | The file name. |
| displayAsIcon | Boolean | Indicates whether diplaying object as an icon. If true, the orginal image data will be covered by icon. |
| label | String | The icon label. Only works when displayAsIcon as true. |

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetEmbeddedObject(bool, byte[], string, bool, string, bool) {#setembeddedobject_1}

Sets embedded object data.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label, bool updateIcon)
```

| Parameter | Type | Description |
| --- | --- | --- |
| linkToFile | Boolean | Indicates whether the object links to the file. If true, the parameter objectData is ignored. |
| objectData | Byte[] | The embedded object data. |
| sourceFileName | String | The file name. |
| displayAsIcon | Boolean | Indicates whether diplaying object as an icon. If true, the orginal image data will be covered by icon. |
| label | String | The icon label. Only works when displayAsIcon as true. |
| updateIcon | Boolean | Indicates whether automatically updating icon. |

### Remarks

As Aspose can update embedd all file icons, so it's better that you can add correct icon with *updateIcon* as false.

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


