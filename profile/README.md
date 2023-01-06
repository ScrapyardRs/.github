# ![](../assets/logo.png?raw=true) Scrapyard

Welcome to scrapyard.

# Projects and why they exist

## (Drax)[../Drax]

Drax is a library/sdk which provides a simple way of defining packets. <br />
In some example case you'd have some packet which needs to send an integer, a varint, and a string. If we'd like to represent that we simply write:

```rust
drax::struct_packet_components! {
  ExamplePacket {
    field_integer: i32,
    field_varint: VarInt,
    field_string: String
  }
}
```

The library handles adding encoding, decoding, and sizing methods.

## (MCProtocol.rs)[../MCProtocol.rs]

MCProtocol.rs is a mirrored protocol of [Minecraft](https://minecraft.net/) built in rust.
