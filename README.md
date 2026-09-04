# EOQ / Reorder Point / Safety Stock Model

A Python + SQLite tool that calculates optimal inventory ordering parameters — Economic Order Quantity (EOQ), Reorder Point (ROP), and Safety Stock — across a multi-product dataset.

## What it does

- Calculates **EOQ** (how much to order each time) by balancing ordering costs vs. holding costs
- Calculates **ROP** (when to reorder) based on daily demand and supplier lead time
- Calculates **Safety Stock** (buffer inventory) to protect against demand variability
- Loads results into a **SQLite database** and queries them with SQL (filtering, sorting)

## Tech used

- Python (pandas, math)
- SQLite (sqlite3)
- SQL (SELECT, WHERE, ORDER BY)

## Example output

Products sorted by reorder urgency (lowest ROP = needs reordering soonest):

| Product | ROP | EOQ |
|---|---|---|
| Widget D | 6 | 77.46 |
| Widget B | 15 | 89.44 |
| Widget A | 28 | 244.95 |
| Widget E | 30 | 268.33 |
| Widget C | 60 | 316.23 |

## Files

- `eoq_reorder_safety_stock_model.ipynb` — full notebook with functions, dataset, calculations, and SQL queries
