# Mixed-bike repositioning data

This repository contains 25 instances with 30, 60, 120, 240, or 480 stations. Each size has five instances.

Each instance folder contains `inventory.csv` and `capacity.csv`. Travel times are extracted from the two shared hlns matrices at the repository root。

## Inventory columns

| Column | Meaning |
|---|---|
| `node_id` | Station identifier within the instance |
| `initial_conventional` | Initial inventory of man-powered bikes |
| `target_conventional` | Target inventory of man-powered bikes |
| `initial_usable_ebikes` | Initial inventory of usable e-bikes |
| `target_usable_ebikes` | Target inventory of usable e-bikes |
| `initial_low_battery_ebikes` | Initial inventory of low-battery e-bikes |

## Capacity columns

| Column | Meaning |
|---|---|
| `node_id` | Station identifier within the instance |
| `capacity` | Station capacity |

## Travel-time data and source

Travel times are extracted from the **hlns-set3** dataset used by Ho and Szeto (2017).

Original dataset: https://www.dropbox.com/s/jbsfefi2wqsssrr/hlns-set3.zip?dl=1.


| File | Matrix dimensions | Used by |
|---|---|---|
| `n302.txt` | 303 × 303, including the depot | `n30_*`, `n60_*`, `n120_*` |
| `n518.txt` | 519 × 519, including the depot | `n240_*`, `n480_*` |
