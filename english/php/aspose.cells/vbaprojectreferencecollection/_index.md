---
title: "VbaProjectReferenceCollection Class"
linktitle: "VbaProjectReferenceCollection"
articleTitle: "VbaProjectReferenceCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents all references of VBA project."
type: docs
weight: 7320
url: /php/aspose.cells/vbaprojectreferencecollection/
---

## VbaProjectReferenceCollection class

Represents all references of VBA project.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number |  |
| [Item (int)](#itemint) | VbaProjectReference | Get the reference in the list by the index. |

## Methods

| Name | Description |
| --- | --- |
| [addRegisteredReference](#addregisteredreference) | Add a reference to an Automation type library. |
| [addControlRefrernce](#addcontrolrefrernce) | Add a reference to a twiddled type library and its extended type library. |
| [addProjectRefrernce](#addprojectrefrernce) | Adds a reference to an external VBA project. |
| [copy](#copy) | Copies references from other VBA project. |
| [clear](#clear) |  |
| [removeAt](#removeat) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [add](#add) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### VbaProjectReferenceCollection.Count property {#count}

**Type:** Number

### VbaProjectReferenceCollection.Item (int) property {#itemint}

Get the reference in the list by the index.

**Type:** VbaProjectReference

### addRegisteredReference(name, libid) {#addregisteredreference}

Add a reference to an Automation type library.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of reference. |
| libid | String | The identifier of an Automation type library. |

### addControlRefrernce(name, libid, twiddledlibid, extendedLibid) {#addcontrolrefrernce}

Add a reference to a twiddled type library and its extended type library.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of reference. |
| libid | String | The identifier of an Automation type library. |
| twiddledlibid | String | The identifier of a twiddled type library |
| extendedLibid | String | The identifier of an extended type library |

### addProjectRefrernce(name, absoluteLibid, relativeLibid) {#addprojectrefrernce}

Adds a reference to an external VBA project.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of reference. |
| absoluteLibid | String | The referenced VBA project's identifier with an absolute path. |
| relativeLibid | String | The referenced VBA project's identifier with an relative path. |

### copy(source) {#copy}

Copies references from other VBA project.

| Parameter | Type | Description |
| --- | --- | --- |
| source | VbaProjectReferenceCollection | The source references. |

### clear() {#clear}

### removeAt(index) {#removeat}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### add(value) {#add}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
