# Asset Management System
A Python + SQLite CRUD mini-project with basic analytics to manage organizational assets.
## Features
- Add, update, delete, and view assets (name, category, value, status).
- Category-wise value summary using Pandas.
- Runs in Google Colab or locally with zero external setup.
## Tech Stack
- Python, SQLite, Pandas, NumPy, Jupyter/Colab.
## Quickstart (Colab)
1. Open a new Colab notebook.
2. Paste the project code cell and run it.
3. Use the provided functions to add/update/delete/view assets.
4. Run `asset_summary()` to see category totals.
## Quickstart (Local)
1. Create and activate a virtual environment.
2. `pip install pandas`
3. Save the script as `asset_manager.py`.
4. Run with `python asset_manager.py` (or import in a Jupyter notebook).
## Core Functions
- `add_asset(asset_name, category, value, status="Active")` → insert a new asset.
- `update_asset(asset_id, asset_name=None, category=None, value=None, status=None)` → modify fields.
- `delete_asset(asset_id)` → remove an asset.
- `view_assets()` → display all assets as a table.
- `asset_summary()` → show category-wise value totals.
## Example Usage
```python
add_asset("Laptop Dell XPS","Electronics",1200,"Active")
update_asset(1,value=1300)
view_assets()
asset_summary()
