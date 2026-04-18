## Project structure

```
src/
  client.ts            # SignalClient — main entry point & event emitter
  chatApi.ts           # Low-level authenticated chat API calls
  decrypt.ts           # Envelope decryption (all envelope types)
  provisioningCipher.ts # QR provisioning flow
  stores.ts            # Protocol stores (session, identity, pre-keys)
  state.ts             # Account state persistence
  contacts.ts          # Contact details parsing
  attachments.ts       # Attachment fetch & decrypt
  sync.ts              # Sync message requests
  protos.ts            # Protobuf type re-exports
  deviceName.ts        # Device name encryption
  demo/
    index.ts           # Demo CLI — links & prints incoming messages
protos/                # .proto files & generated JS/TS
store/                 # Persisted protocol stores (JSON)
state.json             # Persisted account credentials & keys
```
