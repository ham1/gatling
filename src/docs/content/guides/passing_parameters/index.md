---
title: "Passing Parameters"
description: "Using Java options in a Gatling Simulation"
lead: "Using Java options in a Gatling Simulation"
date: 2021-04-20T18:30:56+02:00
lastmod: 2021-04-20T18:30:56+02:00
weight: 010
---

You might want to pass parameters from the command line to the Simulation, for example the number of users, the duration of the ramp...

This can be done very easily with additional `JAVA_OPTS` in the launch script:

```shell
JAVA_OPTS="-Dusers=500 -Dramp=3600"
```

{{< include-code "PassingParametersSample.scala#injection-from-props" scala >}}

Of course, passing a String is just as easy as:

```shell
JAVA_OPTS="-Dfoo=bar"
```

{{< include-code "PassingParametersSample.scala#string-property" scala >}}
