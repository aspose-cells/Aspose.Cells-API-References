---
title: "ExternalLink Class"
linktitle: "ExternalLink"
articleTitle: "ExternalLink"
second_title: "Aspose.Cells for Python via Java"
description: "Represents an external link in a workbook."
type: docs
weight: 2200
url: /python-java/asposecells.api/externallink/
---

## ExternalLink class

Represents an external link in a workbook.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Type](#type) | int | Gets the type of external link. The value of the property is ExternalLinkType integer constant. |
| [PathType](#pathtype) | String | Get the path type of this external link |
| [OriginalDataSource](#originaldatasource) | String | Represents stored data source of the external link. |
| [DataSource](#datasource) | String | Represents data source of the external link. |
| [IsReferred](#isreferred) | boolean | Indicates whether this external link is referenced by others. |
| [IsVisible](#isvisible) | boolean | Indicates whether this external link is visible in MS Excel. |

## Methods

| Name | Description |
| --- | --- |
| [addExternalName](#addexternalname) | Adds an external name. |

### ExternalLink.Type property {#type}

Gets the type of external link. The value of the property is ExternalLinkType integer constant.

**Type:** int

### ExternalLink.PathType property {#pathtype}

Get the path type of this external link

**Type:** String

### ExternalLink.OriginalDataSource property {#originaldatasource}

Represents stored data source of the external link.

**Type:** String

### ExternalLink.DataSource property {#datasource}

Represents data source of the external link.

**Type:** String

### ExternalLink.IsReferred property {#isreferred}

Indicates whether this external link is referenced by others.

**Type:** boolean

### ExternalLink.IsVisible property {#isvisible}

Indicates whether this external link is visible in MS Excel.

**Type:** boolean

### addExternalName(text, referTo) {#addexternalname}

Adds an external name.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of the external name. If the external name belongs to a worksheet, the text should be as Sheet1!Text. |
| referTo | String | The referTo of the external name. It must be a cell or the range. |
