# Keep relationship data encrypted across devices and at rest

The app holds personal information about other people. Cross-device sync must be end-to-end encrypted from its first release with real relationship data, so the relay cannot read that data. Local data must also be encrypted at rest. The user must be able to restore their data after losing both devices, using a recovery secret that the relay cannot use to decrypt it. We accept additional key-management and sync complexity to meet these requirements; the sync technology remains undecided.

CRDTs are preferred for learning, but are not a release requirement. Evaluate Evolu, Automerge Repo with Keyhive, and Yjs through focused spikes; a simpler encrypted sync design remains an option if none meets the gates. Classic Jazz is excluded by product decision.
