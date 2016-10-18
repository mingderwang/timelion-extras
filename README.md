# timelion-extras

This is where I dump random functions that for, whatever reason, I haven't gotten merged into Kibana core. Its my playground, try not to get sand everywhere.

### .aggregate(functionName)
`.aggregate()` creates a flat line based on a function, the names of which are probably self explanatory: avg, min, max, last, sum, cardinality

### .orderby(functionName, direction)
`.orderby()` orders a multiple series list by a function, the names of which are probably self explanatory: avg, min, max, last, sum, cardinality, label. The list can be sorted in ascending (asc) or descending (desc) order.

## Installing
I don't usually publish packages for this, but installing directly from Github is fairly simple:

1. cd to your `kibana/plugins` directory.
2. `wget https://github.com/rashidkpc/timelion-extras/archive/master.zip`
3. `unzip master.zip`
4. `rm timelion-extras-master/gulpfile.js` (This is a dev environment thing. Kibana won't start if you don't remove `gulpfile.js`)
5. Edit `timelion-extras-master/package.json` and change `version` to match, exactly, your Kibana version. Eg `5.0.0-rc1` 
6. Start kibana (and delete that master.zip if you want, or not, it won't break anything)
