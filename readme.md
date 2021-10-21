BPGP Maven aggregator project
=============================
Used to develop BPGP together with
- BPjs-Context
- BPjs
- ECJ (its pom.xml should be in `ecj-git/ecj`)

Instructions
------------
- `git clone` the directories, as siblings of this
- modify each `pom.xml` `version` tag to contain `-SNAPSHOT`
- modify BPGP-wumpus' `pom.xml` to use the `-SNAPSHOT` versions
- comment out the `itpack.io` `repository` section in BPGP-wumpus' `pom.xml`, as it interferes
- IntelliJ, optional:
  - Ctrl-Shift-A -> Delegate IDE build/run actions to Maven -> (enable)
    - easier for debugging compilation problems; but worse on running phase...
  - You might also want to "Skip Tests" at the same Maven-Runner dialog 
  - and also add a property ("+" icon beneath it: `maven.javadoc.skip` value `true`)