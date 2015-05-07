**Status: DEV**

PINF.Logic
==========

PINF.Logic is a branch of [Logic](http://en.wikipedia.org/wiki/Logic) that concerns itself with natural learning.

PINF.Logic is deriving its meaning by continuously abstracting patterns from its [spawned ecosystem](https://genesis.pinf.org) and the application of this ecosystem to real world problems.

PINF.Logic is concerned with understanding decision points through contextual data with the objective of making the best decision possible at any moment in time.

PINF.Logic is seeking a symbiotic relationship with the human condition and operations of the mind to maximize the potential of liberated thought in every user.

PINF.Logic will accomplish this vision by focusing on one area at a time.


Focus 1: Software Cloud Configuration
=====================================

> There are no sensible solutions to configure software and thus infrastructure in the cloud.

Every working solution is heavy and restrictive. PINF.Logic is seeking an enlightened abstraction to the current software cloud configuration state of the art.

PINF.Logic is accomplishing this through implementation of plugins that may be used in the [PINF Toolchain](http://pinf.org).

Configuration Language
----------------------

> We all have our preferences but we can all settle on one standard from which we can bi-directionally generate all other preferences.

The PINF configuration language for Software Systems aims to embody the primary patterns required to provide a sensible solution to configure software and thus infrastructure in the cloud.

````
TODO
````


DNS Management
--------------

> We entrust our DNS providers with the root mappings for our systems. Where do we get the root mappings from?

Too many people are using DNS services as root repositories for their DNS configurations. This means that they entrust the DNS provider with their data and forget about it themselves.

PINF.Logic is seeking a root configuration pattern for DNS that can be used to describe all DNS use-cases.

#### Proposed

````
	{
		"github.com/pinf-logic/pinf.logic-for-dns/0": {
			"records": {
			    "pinf.me": {
			        "domain": "pinf.me",
			        "type": "A",
			        "data": "{{$from.live.app.ip}}"
			    },
			    "*.pinf.me": {
			        "domain": "pinf.me",
			        "type": "CNAME",
			        "data": "pinf.me"
			    }
			}
		}
	}
````

Plugin: [pinf.logic-for-dns](https://github.com/pinf-logic/pinf.logic-for-dns)


#### Feedback

To collaborate on this configuration pattern please [get involved](https://github.com/pinf-logic/pinf.logic-for-dns). Most importantly, please post your DNS configurations for your systems (if you are allowed to and can) to the [issue tracker](https://github.com/pinf-logic/pinf.logic-for-dns/issues) so we can learn all the different permutations.


Definitions
===========

All thinking in PINF.Logic is done within the context of a *System*.

#### System

An orchestrated set of nodes.

Plugin: [pinf.logic-for-system](https://github.com/pinf-logic/pinf.logic-for-system)


#### Orchestration

The act of embuing non-machine meaning upon a *System*. This means using human creativity and thought to create new patterns and encoding these into a language that a software system can understand.

Plugin: [pinf.logic-for-orchestration](https://github.com/pinf-logic/pinf.logic-for-orchestration)


#### Node

Describes the *Source Logic* entity or referenced instance thereof within a *System*. When talking about a *Node* you must clearly specify its *Context* as a *Node* without *Context* is meaningless.

Plugin: [pinf.logic-for-node](https://github.com/pinf-logic/pinf.logic-for-node)


#### Source Logic

The same logic pattern only exists in the one place within a *System*. It gets referenced everywhere else within the same system and potentially other *Systems*.

Plugin: [pinf.logic-for-source-logic](https://github.com/pinf-logic/pinf.logic-for-source-logic)


#### Context

The *Mapping* of our *Node* to one or more other *Nodes* and their *Mappings* to further *Nodes* up to a *Limit*.

Plugin: [pinf.logic-for-context](https://github.com/pinf-logic/pinf.logic-for-context)


#### Mapping

Connects two *Nodes*.

Plugin: [pinf.logic-for-mapping](https://github.com/pinf-logic/pinf.logic-for-mapping)


#### Limit

The boundary set for a *Context* when traversing *Mappings* for the purpose of providing meaning for a *Node*. Limits are necessary as all-aspect distributed nodal platforms can never be viewed from all angles at the same time.


Provenance
==========

Original *Source Logic* [UNLICENSED](http://unlicense.org/) by [Christoph Dorn](http://christophdorn.com).

