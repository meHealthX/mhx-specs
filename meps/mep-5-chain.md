# The Chain
A chain is used in our system to handle:
- The access control layer (ACL)
- The tokens and the economy of the data and artifacts related to the data

We won't be using any of the global open networks for a few reasons:
- In healthcare the trusted parties are known and it's a rather regulated
  ecosystem. There's no need for letting potentially malicious players try and
  get access to patients' data.
- In a permissioned network there's absolutely no need for a PoW consensus
  mechanism. We'll most probably be using a [variant of] PoS consensus
  algorithm.
- Handling a sensitive data such as healthcare, requires fast transition
  between old and buggy systems and smart contracts to the fixed ones, and a
  permissioned network facilitates that. Those issues with the system are bound
  to happen since it's the nature of software, and our system should be ready
  to fix them smoothly.

As of now, [Parity's Substrate](https://www.parity.io/substrate/) seems the
most viable option for an implementation of the chain and the contracts on top
of it.
