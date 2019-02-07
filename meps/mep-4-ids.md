# MEP 4: ID Management
Every entity interacting with the system has a digital ID. The same physical
entity may have more than one ID if needed, _e.g._ as a producer and owner of
data.

The digital entities may have to be linked to the real entities. For instance,
only a real person really owning a data, _i.e._ a patient whose data is about
to be shared, should be able to consent to it and allow that to happen.
However, a digital entity producing data on a digital platform, doesn't have to
prove their real world identity to allow transferring of that digital data.

For instance, if a user is producing data using a fitbit platform, they don't
have to prove their real world identity to share the fitbit data.

The digital identity will be one of the standards promoted by the
[Decentralized Identity Foundation (DIF)](https://identity.foundation/), and
implemented by groups such as [jolocom.io](https://jolocom.io/).

Connecting the digital identities to the physical world will be done with a
mechanism not much different from how it's done using [uPort in the city of
Zug](https://www.ethnews.com/uport-announces-zug-digital-ethereum-id-pilot).

However, since we're dealing with healthcare data and privacy has to come
first, there's the need for a completely privacy driven wallet and identity
management. Further detailing this document will outline how it should be done,
and will specify the requirements.
