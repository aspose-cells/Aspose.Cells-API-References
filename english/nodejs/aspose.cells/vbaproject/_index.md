---
title: "VbaProject"
linktitle: "VbaProject"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the VBA project."
type: docs
weight: 4480
url: /nodejs/aspose.cells/vbaproject/
---

## VbaProject class

Represents the VBA project.

## Methods

| Name | Description |
| --- | --- |
| [copy(source)](#copy) | Copy VBA project from other file. |
| [getCertRawData()](#getcertrawdata) | Gets certificate raw data if this VBA project is signed. |
| [getEncoding()](#getencoding) | Gets and sets the encoding of VBA project. |
| [getIslockedForViewing()](#getislockedforviewing) | Indicates whether this VBA project is locked for viewing. |
| [getModules()](#getmodules) | Gets all VbaModule objects. |
| [getName()](#getname) | Gets and sets the name of the VBA project. |
| [getReferences()](#getreferences) | Gets all references of VBA project. |
| [isProtected()](#isprotected) | Indicates whether this VBA project is protected. |
| [isSigned()](#issigned) | Indicates whether VBAcode is signed or not. |
| [isValidSigned()](#isvalidsigned) | Indicates whether the signature of VBA project is valid or not. |
| [protect(islockedForViewing, password)](#protect) | Protects or unprotects this VBA project. If islockedForViewing is true, the password could not be null. |
| [setEncoding()](#setencoding) | Gets and sets the encoding of VBA project. |
| [setName()](#setname) | Gets and sets the name of the VBA project. |
| [sign(digitalSignature)](#sign) | Sign this VBA project by a DigitalSignature |
| [validatePassword(password)](#validatepassword) | Validates protection password. |

### copy(source) {#copy}

Copy VBA project from other file.

| Parameter | Type | Description |
| --- | --- | --- |
| source | VbaProject |  |

### getCertRawData() {#getcertrawdata}

Gets certificate raw data if this VBA project is signed.

### getEncoding() {#getencoding}

Gets and sets the encoding of VBA project.

### getIslockedForViewing() {#getislockedforviewing}

Indicates whether this VBA project is locked for viewing.

### getModules() {#getmodules}

Gets all VbaModule objects.

### getName() {#getname}

Gets and sets the name of the VBA project.

### getReferences() {#getreferences}

Gets all references of VBA project.

### isProtected() {#isprotected}

Indicates whether this VBA project is protected.

### isSigned() {#issigned}

Indicates whether VBAcode is signed or not.

### isValidSigned() {#isvalidsigned}

Indicates whether the signature of VBA project is valid or not.

### protect(islockedForViewing, password) {#protect}

Protects or unprotects this VBA project. If islockedForViewing is true, the password could not be null.

| Parameter | Type | Description |
| --- | --- | --- |
| islockedForViewing | boolean | indicates whether locks project for viewing. |
| password | String | If the value is null, unprotects this VBA project, otherwise projects the this VBA project. |

### setEncoding() {#setencoding}

Gets and sets the encoding of VBA project.

### setName() {#setname}

Gets and sets the name of the VBA project.

### sign(digitalSignature) {#sign}

Sign this VBA project by a DigitalSignature

| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignature | DigitalSignature | DigitalSignature |

### validatePassword(password) {#validatepassword}

Validates protection password.

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | the password |

**Returns:** boolean — `boolean` Whether password is the protection password of this VBA project
