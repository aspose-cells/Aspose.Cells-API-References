---
title: Aspose::Cells::ExternalConnections::ExternalConnectionCollection class
linktitle: ExternalConnectionCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::ExternalConnections::ExternalConnectionCollection class. Specifies the ExternalConnection collection in C++.'
type: docs
weight: 600
url: /cpp/aspose.cells.externalconnections/externalconnectioncollection/
---
## ExternalConnectionCollection class


Specifies the [ExternalConnection](../externalconnection/) collection.

```cpp
class ExternalConnectionCollection
```

## Methods

| Method | Description |
| --- | --- |
| [ExternalConnectionCollection(ExternalConnectionCollection_Impl* impl)](./externalconnectioncollection/) | Constructs from an implementation object. |
| [ExternalConnectionCollection(const ExternalConnectionCollection\& src)](./externalconnectioncollection/) | Copy constructor. |
| [Get(int32_t index)](./get/) | Gets the [ExternalConnection](../externalconnection/) element at the specified index. |
| [Get(const U16String\& connectionName)](./get/) | Gets the [ExternalConnection](../externalconnection/) element with the specified name. |
| [Get(const char16_t* connectionName)](./get/) | Gets the [ExternalConnection](../externalconnection/) element with the specified name. |
| [GetCount()](./getcount/) |  |
| [GetExternalConnectionById(int32_t connId)](./getexternalconnectionbyid/) | Gets the [ExternalConnection](../externalconnection/) element with the specified id. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ExternalConnectionCollection\& src)](./operator_asm/) | operator= |
| [~ExternalConnectionCollection()](./~externalconnectioncollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
Workbook wb(u"connection.xlsx");
ExternalConnectionCollection dataConns = wb.GetDataConnections();
for (int i = 0; i < dataConns.GetCount(); i++)
{
    ExternalConnection dataConn = dataConns.Get(i);
    //get external connection id
    int id = dataConn.GetConnectionId();
}

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::ExternalConnections](../)
* Library [Aspose.Cells for C++](../../)
