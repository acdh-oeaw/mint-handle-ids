# mint-handle-ids
repo to mint and update Handle-PIDs


## create PIDs

add URLs to `./create_ids.csv` (just override any existing values but keep the headers) and trigger the [mint_pids Workflow](https://github.com/acdh-oeaw/mint-handle-ids/actions/workflows/mint_pids.yml). The minted PIDS will be written back into `./create_ids.csv`


`create_ids.csv` dummy

```csv
arche_id,handle_id
https://id.acdh.oeaw.ac.at/foo/bar,
https://id.acdh.oeaw.ac.at/bar/foo,
```

`create_ids.csv` after successfull workflow run

```csv
arche_id,handle_id
https://id.acdh.oeaw.ac.at/foo/bar,https://hdl.handle.net/21.11115/0000-000F-FF5C-C
https://id.acdh.oeaw.ac.at/bar/foo,https://hdl.handle.net/21.11115/0000-000F-FF5D-B
```