# oracledb-pb version 1.12

oracledb-pb is a fork of [node-oracledb](https://github.com/oracle/node-oracledb) which I have published to npm for the benefit of allowing the community to get up and running with oracledb quickly. It's only external non-npm dependency is the Microsoft Visual C++ Runtime. The module even downloads and installs the necessary Oracle Instant Client Packages for you and adds the folder to your PATH environment variable.

oracledb-pb is located within my node-oracledb fork: [easy_pb](https://github.com/bchr02/node-oracledb/tree/easy_pb) which is based on the work of my node-oracledb fork: [prebuild_support](https://github.com/bchr02/node-oracledb/tree/prebuild_support). easy_pb's only differnce is that it has a dependency on [instantclient](https://github.com/bchr02/instantclient), so that upon installation the Oracle Instant Client Packages get installed, and lib/oracledb is modified to add Instant Client to path.

## Install:
npm install oracledb-pb

## Use:
var oracledb = require('oracledb-pb');


*Disclaimer: For small projects, testing or rapid prototyping I recommend oracledb-pb but for anything large scale or something that you will be publishing to npm I don't recommend it. The main reason is because it is not officially supported by Oracle and another reason is because I can't make any guarantees as to how frequently or how long term I can maintain it. Although, I do plan to automate the publishing of upstream node-oracledb changes which should significantly reduce the maintaince needed.* 
