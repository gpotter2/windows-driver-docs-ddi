---
UID: NS:acpitabl._ACPI_PLD_SPATIAL_BUFFER
title: _ACPI_PLD_SPATIAL_BUFFER structure (acpitabl.h)
description: Describes the ACPI PLD spatial descriptor buffer, revision 1 (Microsoft custom PLD buffer extension, 128-bits).
ms.date: 11/19/2020
keywords: ["ACPI_PLD_SPATIAL_BUFFER structure"]
ms.keywords: _ACPI_PLD_SPATIAL_BUFFER, ACPI_PLD_SPATIAL_BUFFER, *PACPI_PLD_SPATIAL_BUFFER,
req.header: acpitabl.h
req.include-header: 
req.target-type: 
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.lib: 
req.dll: 
req.ddi-compliance: 
req.unicode-ansi: 
req.max-support: 
req.typenames: ACPI_PLD_SPATIAL_BUFFER, *PACPI_PLD_SPATIAL_BUFFER
targetos: Windows
tech.root: acpi
f1_keywords:
 - _ACPI_PLD_SPATIAL_BUFFER
 - acpitabl/_ACPI_PLD_SPATIAL_BUFFER
 - PACPI_PLD_SPATIAL_BUFFER
 - acpitabl/PACPI_PLD_SPATIAL_BUFFER
 - ACPI_PLD_SPATIAL_BUFFER
 - acpitabl/ACPI_PLD_SPATIAL_BUFFER
topic_type:
 - apiref
api_type:
 - HeaderDef
api_location:
 - acpitabl.h
api_name:
 - _ACPI_PLD_SPATIAL_BUFFER
---

# _ACPI_PLD_SPATIAL_BUFFER structure

## -description

Describes the ACPI PLD spatial descriptor buffer, revision 1 (Microsoft custom PLD buffer extension, 128-bits).

## -struct-fields

### -field Revision

### -field RollRotation

### -field PitchRotation

### -field YawRotation

### -field Width

### -field Height

### -field Length

### -field HorizontalOffset

### -field VerticalOffset

### -field DepthOffset

## -remarks

```cpp
DEFINE_GUID(ACPI_PLD_SPATIAL_BUFFER_GUID,
    0x59af1a1f, 0xaba4, 0x4bb8, 0x81, 0xef, 0x55, 0x93, 0x8e, 0x9b, 0xc5, 0x3a);
```

## -see-also
