---
title: "VbaProjectReferenceCollection"
linktitle: "VbaProjectReferenceCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents all references of VBA project."
type: docs
weight: 4500
url: /nodejs/aspose.cells/vbaprojectreferencecollection/
---

## VbaProjectReferenceCollection class

Represents all references of VBA project.

## Methods

| Name | Description |
| --- | --- |
| [add()](#add) | Reserved for internal use. |
| [addControlRefrernce(name, libid, twiddledlibid, extendedLibid)](#addcontrolrefrernce) | Add a reference to a twiddled type library and its extended type library. |
| [addProjectRefrernce(name, absoluteLibid, relativeLibid)](#addprojectrefrernce) | Adds a reference to an external VBA project. |
| [addRegisteredReference(name, libid)](#addregisteredreference) | Add a reference to an Automation type library. |
| [clear()](#clear) |  |
| [contains()](#contains) | Reserved for internal use. |
| [copy(source)](#copy) | Copies references from other VBA project. |
| [get(i)](#get) | Get the reference in the list by the index. |
| [get()](#get-1) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [removeAt()](#removeat) |  |

### add() {#add}

Reserved for internal use.

### addControlRefrernce(name, libid, twiddledlibid, extendedLibid) {#addcontrolrefrernce}

Add a reference to a twiddled type library and its extended type library.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of reference. |
| libid | String | The identifier of an Automation type library. |
| twiddledlibid | String | The identifier of a twiddled type library |
| extendedLibid | String | The identifier of an extended type library |

**Returns:** Number — `Number`

### addProjectRefrernce(name, absoluteLibid, relativeLibid) {#addprojectrefrernce}

Adds a reference to an external VBA project.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of reference. |
| absoluteLibid | String | The referenced VBA project's identifier with an absolute path. |
| relativeLibid | String | The referenced VBA project's identifier with an relative path. |

**Returns:** Number — `Number`

### addRegisteredReference(name, libid) {#addregisteredreference}

Add a reference to an Automation type library.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of reference. |
| libid | String | The identifier of an Automation type library. |

**Returns:** Number — `Number`

### clear() {#clear}

### contains() {#contains}

Reserved for internal use.

### copy(source) {#copy}

Copies references from other VBA project.

| Parameter | Type | Description |
| --- | --- | --- |
| source | VbaProjectReferenceCollection | The source references. |

### get(i) {#get}

Get the reference in the list by the index.

| Parameter | Type | Description |
| --- | --- | --- |
| i | Number | The index. |

**Returns:** VbaProjectReference — `VbaProjectReference`

### get() {#get-1}

Reserved for internal use.

### getCount() {#getcount}

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### removeAt() {#removeat}
