# Red Netto vs Black Netto in OpenStreetMap

In Germany there are two supermarket chains called `Netto`.

The “red Netto” is really called `Netto Marken-Discount` with full name. They have a red-yellow logo:

![Red Netto logo](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f1/Netto_Marken-Discount_2018_logo.svg/320px-Netto_Marken-Discount_2018_logo.svg.png)

The “black Netto” has a black-yellow logo including a dog, and is therefore sometimes called “Hundenetto” (= dog Netto).

![Black Netto logo](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b6/NettoLogo2019-S.svg/320px-NettoLogo2019-S.svg.png)

In OpenStreetMap there are tags `brand` and `brand:wikidata` to mark the brand unambiguously. But sometimes these tags are missing or mistakes happen and the wrong brand is assigned.

The notebook [netto.ipynb](./netto.ipynb) checks the Netto supermarkets in OpenStreetMap against the official location information coming from the supermarkets’ websites. The results are exported into a series of tables in Markdown files.


## How to run the notebook

Clone the repository:

```bash
git clone https://github.com/hfs/osm-netto.git
cd osm-netto
```

Install [uv](https://docs.astral.sh/uv/getting-started/installation/) if you don’t have it, yet.

Create the Python virtual environment and install all dependencies:

```bash
uv sync
```

Activate the virtual environment (Use one of the other activation scripts in the `.venv/bin` directory if you use a different shell than bash):

```bash
. .venv/bin/activate
```

Start the development environment in the browser.

```bash
jupyter-lab
```

Open `netto.ipynb` from the directory tree.
