##ConnectionDataSourceType Enum
'ConnectionDataSourceType enum. Encapsulates the object that represents connectiondatasourcetype in Go.'
## ConnectionDataSourceType Enum
Specifies external database source type
```go
type ConnectionDataSourceType int32
```
## Fields
| Field | Description |
| --- | --- |
|[ODBCBasedSource](./odbcbasedsource/) | ODBC-based source |
|[DAOBasedSource](./daobasedsource/) | DAO-based source |
|[FileBasedDataBaseSource](./filebaseddatabasesource/) | File based database source |
|[WebQuery](./webquery/) | Web query |
|[OLEDBBasedSource](./oledbbasedsource/) | OLE DB-based source |
|[TextBasedSource](./textbasedsource/) | Text-based source |
|[ADORecordSet](./adorecordset/) | ADO record set |
|[DSP](./dsp/) | DSP |
|[OLEDBDataModel](./oledbdatamodel/) | OLE DB data source created by the Spreadsheet Data Model. |
|[DataFeedDataModel](./datafeeddatamodel/) | Data feed data source created by the Spreadsheet Data Model. |
|[WorksheetDataModel](./worksheetdatamodel/) | Worksheet data source created by the Spreadsheet Data Model. |
|[TextDataModel](./textdatamodel/) | Text data source created by the Spreadsheet Data Model. |
|[Unknown](./unknown/) | Text data source created by the Spreadsheet Data Model. |
