# observable-data-tools
[Random Fractals Inc.](https://observablehq.com/@randomfractals?tab=collections) stash of [Observable](https://observablehq.com/explore) Data Toools and [Notebooks](https://twitter.com/hashtag/dataNotebooks?src=hashtag_click) 📚 in `.js`, `.nb.json`, `.ojs`, `.omd` and `.qmd` document formats for Data Previews in [VSCode](https://code.visualstudio.com/) with [Observable JS](https://marketplace.visualstudio.com/items?itemName=GordonSmith.observable-js) extension, [Quarto](https://marketplace.visualstudio.com/items?itemName=quarto.quarto) extension, and new [Quarto publishing](https://quarto.org/docs/publishing/) tools.

## Observable Data Notebooks

[**Tables Notebook Collection**](https://observablehq.com/collection/@randomfractals/tables)

| Notebook | Description |
| --- | --- |
| [Data Table Viewer](https://observablehq.com/@randomfractals/data-table-viewer?collection=@randomfractals/tables) | Simple data notebook to view public data files in `.csv`, `.arrow`, `.json` array, and `.geojson` data formats. Allows to load a data file accessible via `https://` with `dataUrl` query parameter and share data table viewer notebook with the loaded data with others. Provides a list of sample [vega-datasets](https://github.com/vega/vega-datasets/tree/next/data) to preview. Includes simple Observable [`Inputs.table`](https://observablehq.com/@observablehq/input-table) data view cell and [Summary Table](https://observablehq.com/@observablehq/summary-table) cell for a quick overview of dataset columns, total rows, data snapshot graph, missing, mean, median and standard deviation info for the numeric data fields. |
| ... | ... |
| [DuckDB Data Tables](https://observablehq.com/@randomfractals/duckdb-data-tables?collection=@randomfractals/duckdb) | DuckDB Data Tables notebook covers sample `.json`, `.csv`, and .`parquet` data loading from Observable [FileAttachments](https://observablehq.com/@observablehq/file-attachments). It lists created DuckDB tables, lets you pick a table and view table schema and data summary with Observable [Summary Table](https://observablehq.com/@observablehq/summary-table) data tool. You can also view and search table data results via standard Observable [`Inputs.search`](https://observablehq.com/@observablehq/input-search) and [`Inputs.table`](https://observablehq.com/@observablehq/input-table) controls, using [Data Wrangler](https://observablehq.com/@observablehq/data-wrangler) with [Arguero](https://uwdata.github.io/arquero/), or query selected table data with new Observable [`SQL cell`](https://observablehq.com/@observablehq/sql-cell). This DuckDB Data Tables intro notebook also creates Tables diagrams from the loaded data files with  [Graphviz html tables](https://graphviz.org/doc/info/shapes.html#html) and [Mermaid ER Diagram](https://mermaid-js.github.io/mermaid/#/entityRelationshipDiagram), and briefly covers DuckDB [Information Schema](https://duckdb.org/docs/sql/information_schema) views, [Pragmas](https://duckdb.org/docs/sql/pragmas), and created DuckDB instance [Configuration Options](https://duckdb.org/docs/sql/configuration). |
| [Datapackage DuckDB](https://observablehq.com/@randomfractals/datapackage-duckdb?collection=@randomfractals/duckdb) | DataPackage DuckDB notebook lets you load tabular data described in [Data Package](https://specs.frictionlessdata.io/data-package/) format by changing `datapackage.json` Url. It creates tabular data resources list, data package tables diagram, lists selected table data, imports tabular data into new DuckDB instance, shows db tables diagram, and lets you filter and query imported data with Observable [Data table cell](https://observablehq.com/@observablehq/data-table-cell) and [SQL cell](https://observablehq.com/@observablehq/sql-cell) tools. You can learn more about Data Package format in our [Datapackage Observable notebooks](https://observablehq.com/@randomfractals/data-package?collection=@randomfractals/datapackage) collection. |
| [DuckDB Data Import](https://observablehq.com/@randomfractals/duckdb-data-import?collection=@randomfractals/duckdb) | This notebook lets you import data into new DuckDB instance from public data Url. Supported data files include: `.csv`, `.json` array, `.geojson`, `.arrow` and `.parquet`. In case of GeoJSON we flatten it similar to how [github flat data viewer](https://github.com/githubocto/flat-viewer) handles geo data loading and display. The usual set of Observable data table, SQL cell, and Table Summary data tools are provided in this notebook to preview loaded data and created DuckDB tables. Try Sample Data Files in that notebook and loading your own data and sharing it with notebook `dataUrl` query param. |
| [SQLite to DuckDB](https://observablehq.com/@randomfractals/sqlite-to-duckdb?collection=@randomfractals/duckdb) | The last notebook in this collection loads sample [SQLite](https://www.sqlite.org/about.html) `chinook.db` from Observable [FileAttachments](https://observablehq.com/@observablehq/file-attachments), lists loaded SQLite DB tables, creates SQLite Tables Diagram, DuckDB [`CREATE TABLE`](https://duckdb.org/docs/sql/statements/create_table) statements, creates new DuckDB instance and tables and shows created DuckDB Tables Diagram. The last remaining task to finish that notebook is bulk data insert pending `PRAGMA foreign_keys = on/off` (#4201) and `ALTER TABLE ADD CONSTRAINT .. FOREIGN KEY` (#4203) features implementation. |
| ... | ... |