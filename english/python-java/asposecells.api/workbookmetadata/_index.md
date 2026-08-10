---
title: "WorkbookMetadata Class"
linktitle: "WorkbookMetadata"
articleTitle: "WorkbookMetadata"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the meta data."
type: docs
weight: 7560
url: /python-java/asposecells.api/workbookmetadata/
---

## WorkbookMetadata class

Represents the meta data.

## Constructors

| Name | Description |
| --- | --- |
| [WorkbookMetadata](#constructor) | Create the meta data object. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Options](#options) | MetadataOptions | Gets the options of the metadata. |
| [BuiltInDocumentProperties](#builtindocumentproperties) | BuiltInDocumentPropertyCollection | Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. |
| [CustomDocumentProperties](#customdocumentproperties) | CustomDocumentPropertyCollection | Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet. |

## Methods

| Name | Description |
| --- | --- |
| [save](#save) | Save the modified metadata to the file. |

### WorkbookMetadata(fileName, options) {#constructor}

Create the meta data object.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String |  |
| options | MetadataOptions |  |

### WorkbookMetadata.Options property {#options}

Gets the options of the metadata.

**Type:** MetadataOptions

### WorkbookMetadata.BuiltInDocumentProperties property {#builtindocumentproperties}

Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet.

**Type:** BuiltInDocumentPropertyCollection

### WorkbookMetadata.CustomDocumentProperties property {#customdocumentproperties}

Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet.

**Type:** CustomDocumentPropertyCollection

### save(fileName) {#save}

Save the modified metadata to the file.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |
