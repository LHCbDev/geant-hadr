# Test project for handling job results in LHCbPR

```
$> ./scripts/bootstrap # should be run at lxplus
```

, run GEANT standalone hadronic test in different configurations:

```python
configs = [
    {
        'slot': 'lhcb-gauss-dev',
        'cmtconfig': 'x86_64-slc6-gcc48-opt',
        'version': 'HEAD',

    },
    {
        'cmtconfig': 'x86_64-slc6-gcc48-opt',
        'version': 'v96r4p2'
    },
    {
        'cmtconfig': 'x86_64-slc6-gcc49-opt',
        'version': 'v96r4p2'
    }
]
```

At the end print commands that should be run for producing zip files for LHCbPR using [collectRunResults.py](https://gitlab.cern.ch/lhcb-core/LHCbPR2HD/blob/master/collectRunResults.py) script and [GeantStandaloneHandler](https://gitlab.cern.ch/lhcb-core/LHCbPR2HD/blob/master/handlers/GeantStandaloneHandler.py) handler from [LHCbPR2HD](https://gitlab.cern.ch/lhcb-core/LHCbPR2HD) project.

Next step you need to [import zip files](https://gitlab.cern.ch/lhcb-core/LHCbPR2BE#import-zip-files) into database

