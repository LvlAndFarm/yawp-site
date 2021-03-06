---
layout: guides
title: "Tutorials: Scaffolding"
description: List and details of the available YAWP!'s scaffold options
---
# Scaffolding

Before you get used to the __YAWP!__ features API, the scaffold plugin can make your life a 
little bit easier =)

### Endpoint

~~~ bash
mvn yawp:endpoint -Dmodel=person
~~~

This will create the endpoint model __Person__. It also will create placeholders for its test suite and
the security Shield.

### Shield

~~~ bash
mvn yawp:shield -Dmodel=person
~~~

Create a __PersonShield__ if the endpoint model is not already shielded.

### Action

~~~ bash
mvn yawp:action -Dmodel=person -Dname=activate
~~~

Creates a __PersonActivateAction__ custom action for the endpoint model.

### Transformer

~~~ bash
mvn yawp:transformer -Dmodel=person -Dname=upperCase
~~~

Create a __PersonUpperCaseTransformer__ transformer for the endpoint model.


### Hook

~~~ bash
mvn yawp:hook -Dmodel=person -Dname=setUser
~~~

Create a __PersonSetUserHook__ hook for the endpoint model.

### Pipe

~~~ bash
mvn yawp:pipe -Dmodel=person -Dname=counter -Dsink=personCounter
~~~

Create a __PersonCounterPipe__ pipe from the source endpoint model Person 
to the sink endpoint model PersonCounter.


