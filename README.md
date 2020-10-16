# Nano public roadmap

This repository holds the broader connecting issues and network upgrade details found in the [official Nano node & protocol roadmap](https://github.com/orgs/nanocurrency/projects/5). Although issues from other repositories can be included in the roadmap, they will be of a more granular nature than the items found here. This extra layer provides more flexibility for oulining progress on features spanning multiple releases or network upgrades, while keeping issue backlogs cleaner in all repositories.

Issues here are read-only with conversations locked as the discussions will be more helpful if done within the more granular tickets found in other repositories.

If you have questions or comments about the roadmap we'd encourage you to join discussions on the [Nano forum](https://forum.nano.org) or [connect directly with the Nano Foundation](https://nano.org/connect).

## Roadmap labels

Because the roadmap has a mix of broader and more granular issues across a variety of functional areas it can be useful to filter to a particular set of items. This can be done with the use of labels:

* The **functional areas** particular features target will be added as labels as well to allow for better grouping. See below for a guide to functional areas.

* The **network upgrade** details will also be labeled due to some functionality requiring multiple phases to fully enable across the network. See below for a guide on how network upgrades are labeled.

## Target releases

Columns in the project with a version number (e.g. `V23.0`) will contain features currently targeted to be included in that release. As resources and scope shift during development, all features are subject to target release changes (see the [disclaimer](#disclaimer)). As changes to the ticket are tracked below the description, each change can be easily followed.

In addition to version-specific columns, the **Exploratory** column is reserved for features which have a high interest and are being considered, but which have no estimate target release yet.

## Functional areas

The following cover the major functional areas of the Nano node and help illustrate progress in a specific area through grouping of tickets under the related labels.

* **Protocol messaging** (label: `protocol`) - updates to the requirements for direct communication between nodes on the network

* **ORV consensus** (label: `orv consensus`) - changes to the mechanisms contributing to consensus including voting behavior, weight and quorum calculations and election management 

* **Boostrapping** (label: `bootstrapping`) - modifications to how an out-of-sync node gets their missing blocks from the network to reconciles their ledger

* **Peering & network structure** (label: `peering & network`) - the mechanisms for establishing individual connections between nodes based on broader network structure rules

* **Node communications** (label: `node comms`) - updates to the IPC, RPC, CLI, WebSocket and other methods used for communicating commands to the node

* **Ledger management** (label: `ledger management`) - changes affecting the ledger structure, contents, formats and other database related details

* **Node architecture** (label: `node architecture`) - adjustments to how broad components are managed within or by the node

* **Work generation** (label: `work generation`) - modifications to the methods generating valid work for transactions


## Network upgrades

Due to the Nano network being decentralized and having to manage global consensus, in order to ensure consistency and efficiency certain updates to the node must be enabled in phases and using mechanisms that activate them after initial software upgrade. Columns in the project beginning with `Upgrade:` represent time between node releases where a specific network upgrade is being targeted. All network upgrades are subject to timing changes (see the [disclaimer](#disclaimer)). Issues added to these columns will be tied to their related features and contain pertinent details about the upgrade.

Labels are also used on tickets to show the type of network upgrade required. Below these labels are listed with a brief explanation of how each upgrade type is typically handled. More details on the various methods and past upgrades can be found in the [Network Upgrades documentation](https://docs.nano.org/releases/network-upgrades/).

* **[Phased node upgrades](https://docs.nano.org/releases/network-upgrades/#phased-node-upgrades)** (label: `phased node upgrade`) - requiring multiple node upgrades before feature ready for activating; often in combination with other upgrade methods

* **[Hardcoded date](https://docs.nano.org/releases/network-upgrades/#hardcoded-date)** (label: `date upgrade`) - activation of feature done on specific date hardcoded into a specific node release version

* **[Canary block(s)](https://docs.nano.org/releases/network-upgrades/#canary-blocks)** (label: `canary upgrade`) - hardcoding of one or more block hashes in the node which cause feature activation once the blocks are distributed and confirmed by the network

* **[Epoch blocks](https://docs.nano.org/releases/network-upgrades/#epoch-blocks)** (label: `epoch upgrade`) - a special block type tied to a hardcoded private key in a node version that when distributed can upgrade account versions


## Disclaimer 

Any statement in this repository that is not purely historical is considered a forward-looking statement. Forward-looking statements included in this repository are based on information available to the Nano Foundation and community members managing the roadmap as of the date they are made, and the Nano Foundation and community members assumes no obligation to update any forward-looking statements. The forward-looking roadmap does not represent a commitment, guarantee, obligation or promise to deliver any feature or upgrade, or to deliver any feature or upgrade by any particular date, and is intended to outline the general development plans. Nobody should rely on this roadmap to make any decision related to the Nano network or otherwise.