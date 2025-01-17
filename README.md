# GC-Net Visualizer

An interactive environment for visualizing the L1 data of the GC-Net ([link](https://github.com/GEUS-Glaciology-and-Climate/GC-Net-level-1-data-processing/tree/main/L1)).

### TODO:

- [ ] Deploy to different PaaS (or via GitHub pages)
- [ ] Improve performance when loading hourly data 
  - [ ] Add memoization caching
  - [ ] Implement clientside and background callbacks
  - [ ] Speed up serialization to JSON
- [ ] Rearrange filters
- [ ] Refactoring
- [ ] Visualize climatologies
- [ ] Visualize uncertainty

## How to run this app locally

1. Clone the git repository 

```
git clone https://github.com/silorepos/gcnvis.git
```

2. Create and activate new virtual environment (recommended)

```
python3 -m venv venv
source /venv/bin/activate  # On Windows: .\venv\Scripts\activate.bat
```

2. Install all dependencies 

```
pip install -r requirements.txt
```

3. Download the latest L1 data

```
bash /scripts/download_data.sh
```

4. Run the app (and visit http://127.0.0.1:8050/ in your browser)

```
python app.py
```

