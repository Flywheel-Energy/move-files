## Usage

move files and artifacts via SSH as below.

```yaml
name: move files
on: [push]
jobs:

  move:
    name: Move
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@master
    - name: move file
      uses: Flywheel-Energy/move-files-action@master
      with:
        source: "tests/a.txt"
        target: "tests/files/a.txt"
```
