# MEP 0: Overview
This document is an overview of the system, with a very short description of
each part. Each of these concepts/sections are described in more detail in
their own MEP. This is mostly a high level description of what is involved in
the ecosystem, and each corresponding MEP defines in detail how they should be
implemented.

_Note_: We are at a highly volatile stage and all these definitions may change
significantly without any prior notice.

## Data
mhx is designed to handle health related data and it covers the following
categories:

- Electronic Medical Records (EMR)
- Digital health data

EMR includes all the data recorded and produced at the clinics, hospitals, and
doctor's offices, whereas digital health data is either stored on the patients'
phones/devices, or on the platform providing the service (digital health SMEs
for instance). Each of these data have their own specific ownership models and
mhx needs to handle them accordingly.

## Roles
Not all players have the same permissions on the system, and they interact
with the modules and smart contracts according to their role. These roles
include:

- Patients/users
- Doctors/hospitals
- Insurance companies
- Pharmaceutical companies
- Research institutes

Each role has their own specific permissions which consequently define how they
interact with the system.

## ID Management
There needs to be a way to authenticate players and users of the system. There
are two categories here, users and businesses.

For the users, there needs to be a way to authenticate and authorize the users
initially, and have a way to generate their private keys accordingly. There are
already a few methods in place for that at least in Germany, and we'd make use
of them.

On the other hand, the businesses have more sensitive permissions on the system
and they need to go through more scrutiny to get their corresponding keys and
permissions.

## Storage
mhx does NOT store any data other than the permissions to the hashes of the
data. We borrow many concepts from the [Ocean
Protocol](https://oceanprotocol.com/) and use them in our system. The data
stays where it is, and is transferred between players outside the scope of mhx.
We only handle the permissions and the users and businesses talk through this
system to give and gain access to different data.

However, we do provide SDKs and pieces of software to better integrate the
existing storage systems to one another, while using the data on the chain as
the backbone for the access control layer (ACL).

## The Chain
We use a permissioned network based on Ethereum using proof of stake.
