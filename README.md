# Cometd Dist

The cometd repository is not very friendly to js projects. Some alternatives exist with distributions of cometd, but they don't follow the same versioning.

## Preparing a tag

Requires maven.

 - Init submodule and check out desired tag
 - `(cd cometd/cometd-javascript/common && mvn install)`
 - Replace {{ tag }} on the following and run
 - `jar -xf ~/.m2/repository/org/cometd/javascript/cometd-javascript-common/{{ tag }}/cometd-javascript-common-{{ tag }}.war org/cometd.js`
 - `mv org/cometd.js . && rmdir org`
 - `cp cometd/cometd-javascript/jquery/src/main/webapp/jquery/jquery.cometd.js .`
