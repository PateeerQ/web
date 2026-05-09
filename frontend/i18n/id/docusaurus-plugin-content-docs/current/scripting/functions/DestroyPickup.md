---
title: DestroyPickup
sidebar_label: DestroyPickup
description: Menghancurkan item yang dibuat dengan CreatePickup.
tags: ["pickup"]
---

## Deskripsi

Menghancurkan item yang dibuat dengan CreatePickup.

| Nama   | Deskripsi                                                              |
| ------ | ---------------------------------------------------------------------- |
| pickup | ID dari pickup yang akan dihancurkan (dikembalikan oleh CreatePickup). |

## Returns

**true** - The function executed successfully.

**false** - The function failed to execute. The pickup specified doesn't exist.

## Examples

```c
new g_PickupArmour;

// Buat item untuk armor.
g_PickupArmour = CreatePickup(1242, 2, 1503.3359, 1432.3585, 10.1191);

// Sewaktu-waktu ingin digunakan
DestroyPickup(g_PickupArmour);
```

## Related Functions

- [CreatePickup](CreatePickup): Membuat Pickup.
- [IsValidPickup](IsValidPickup): Cek apakah Pickup valid.

## Related Callbacks

- [OnPlayerPickUpPickup](../callbacks/OnPlayerPickUpPickup): Dipanggil saat player menyentuh pickup.
