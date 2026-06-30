# Local Data Layout

Large local datasets, virtual-screening outputs, and runtime artifacts are kept outside this Git repository under:

```text
/mnt/data/KarmaDock/
```

Current layout:

```text
/mnt/data/KarmaDock/
  datasets/          PDBbind and DEKOIS2 datasets and archives
  screening_runs/    KarmaDock screening inputs, generated graphs, scores, poses, and notebooks
  api_runtime/       Local API uploads, results, and task history
  inputs/            Local KRAS G12D/G12V protein and ligand input files
  notebooks/         Local exploratory notebooks
  test_data/         Local test structures and generated graph files
  archives/          Local backups and old app archives
  scratch/           Python caches and temporary local files
```

The repository keeps source code, environment files, documentation, and the bundled KarmaDock screening model. New datasets and run outputs should stay in `/mnt/data/KarmaDock` or another external data directory, not in Git.
