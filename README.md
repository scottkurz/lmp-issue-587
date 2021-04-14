# lmp-issue-587
Workaround for https://github.com/OpenLiberty/ci.maven/issues/587



1.  mvn   resources:copy-resources liberty:dev
2. https://localhost:9443/ibm/api/config/jndiEntry/TidalJNDI
3. https://localhost:9443/ibm/api/config/
4.  mvn  -Pprod resources:copy-resources liberty:dev
5. <check browser again> 


IDEAS
1. use separate config file not managed by liberty-maven-plugin
2. use shared config dir to not get overwritten.
