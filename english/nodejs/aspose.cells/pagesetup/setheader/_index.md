---
title: "PageSetup.setHeader"
linktitle: "setHeader"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Sets a script formatting the header of an Excel file."
type: docs
weight: 780
url: /nodejs/aspose.cells/pagesetup/setheader/
---

## setHeader(section, headerScript)

Sets a script formatting the header of an Excel file. Script commands:CommandDescription&PCurrent page number &NPage count &DCurrent date &TCurrent time&ASheet name&FFile name without path&" "Font name, for example: &"Arial"&" , "Font name and font style, for example: &"Arial,Bold"& Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character.&K Font color, for example(RED): &KFF0000&GImage script For example: "&Arial,Bold&8Header Note"

| Parameter | Type | Description |
| --- | --- | --- |
| section | Number | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | String | Header format script. |
