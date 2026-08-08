---
title: "BuiltInDocumentPropertyCollection.get"
linktitle: "get"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Returns a DocumentProperty object by the name of the property."
type: docs
weight: 50
url: /nodejs/aspose.cells/builtindocumentpropertycollection/get/
---

## get(name)

Returns a DocumentProperty object by the name of the property. The string names of the properties correspond to the names of the typed properties available from BuiltInDocumentPropertyCollection.If you request a property that is not present in the document, but the name of the property is recognized as a valid built-in name, a new DocumentProperty is created, added to the collection and returned. The newly created property is assigned a default value (empty string, zero, false or DateTime.MinValue depending on the type of the built-in property).If you request a property that is not present in the document and the name is not recognized as a built-in name, a null is returned.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property to retrieve. |
