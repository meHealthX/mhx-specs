# MEP 6: User Initialization
This document explains what happens once a user joins the system, and how they
collect information about themselves. This process should be repeatable
because:

- Users may loose their master key and would like to rejoin using a newly
  generated key.
- Users may choose to let the system forget their old ID and start over using a
  completely new digital identity; which is their right according to GDPR.
- Since we want to avoid any central place holding all users' data or metadata,
  the user should be the one holding the complete picture of their data, hence
  they should be able to collect that information upon joining the system.

Once the user creates a digital ID (through a master key/private key), and
connect that identity with their real world identity using a third party
authority such as [POSTIDENT](https://www.deutschepost.de/de/p/postident.html),
they can start interacting with the system. The first interaction is to
initialize their account on their own device. They would trigger a transaction
and request all the metadata belonging to their own account. That transaction
is then broadcast on the network and all parties holding user data, would
respond to that particular request if they hold data belonging to the real
world identity of that user holding that digital identity.

Once all parties holding this user's data have responded, the user receives the
information and will have a complete picture of their information and where the
information is held on their own device.

If a user for any reason chooses to change their digital identity, they would
ask the third party to invalidate their old digital identity, and register a
new one. Since the old information was only available to the old digital
identity, the user would need to re-initialize their account by triggering the
initial transaction again, and collect the information from parties in the
ecosystem from scratch.
