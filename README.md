# Data Quick Look

Press **space** in Finder to preview data files, the same way you preview images and PDFs.

**[⬇️ Download the latest version (.dmg)](https://github.com/matthewslopecki/data-quicklook-releases/releases/latest/download/DataQuickLook.dmg)**

| Format | Extensions |
|:---|:---:|
| Parquet | `.parquet`, `.parq` |
| JSON Lines | `.jsonl`, `.ndjson` |
| DuckDB database | `.duckdb`, `.ddb` |
| SQLite database | `.sqlite`, `.sqlite3`, `.db`, `.db3` |
| NumPy | `.npy`, `.npz` |
| Arrow / Feather v2 | `.arrow`, `.feather`, `.ipc`, `.arrows` |
| HDF5 | `.h5`, `.hdf5`, `.he5` |
| MATLAB | `.mat` (v5–v7.3) |
| C3D motion capture | `.c3d` |

Each preview shows a summary (rows, columns, size and format details), the first 500 rows, and the
schema. Files that hold several tables, such as databases, HDF5 and C3D files, show each table in its
own section. Only the start of each file is read, so even multi-GB files open instantly.

## Install

1. Download the `.dmg`, open it, and drag **Data Quick Look** into **Applications**.
2. Open **Data Quick Look** from Applications once. This registers the previewer with macOS.
3. Select a data file in Finder and press space.

The app isn't notarized by Apple, so the first time you open it macOS says it can't check it for
malicious software. To open it anyway, go to **System Settings › Privacy & Security**, scroll down,
click **Open Anyway** next to the message about Data Quick Look, then confirm with **Open**.

If previews don't appear, check **System Settings › General › Login Items & Extensions › Quick Look**
and make sure Data Quick Look is turned on.

Requires macOS 13 or later, on Apple silicon or Intel.

## Privacy

Previews run entirely on your Mac, inside Quick Look's sandbox. The app has no network access and
collects nothing.

## Open-source software

Data Quick Look uses DuckDB, HDF5, LZ4 and Zstandard. Their licenses are in the app under
**Data Quick Look › About Data Quick Look**.
