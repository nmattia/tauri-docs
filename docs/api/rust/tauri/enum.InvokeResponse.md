---
title: Enum tauri::InvokeResponse
sidebar_label: enum.InvokeResponse
custom_edit_url: null
---

  # Enum tauri::InvokeResponse,

```rs
pub enum InvokeResponse {
    Ok(JsonValue),
    Err(InvokeError),
}
```

Expand description

Response from a [`InvokeMessage`](/docs/api/rust/tauri/struct.InvokeMessage "InvokeMessage") passed to the [`InvokeResolver`](/docs/api/rust/tauri/struct.InvokeResolver "InvokeResolver").

## Variants

`Ok(JsonValue)`

Resolve the promise.

`Err(InvokeError)`

Reject the promise.

## Implementations

### impl [InvokeResponse](/docs/api/rust/tauri/enum.InvokeResponse "enum tauri::InvokeResponse")[\[src\]](/docs/api/rust/tauri/../src/tauri/hooks.rs#88-97 "goto source code")

#### pub fn [into_result](/docs/api/rust/tauri/about:blank#method.into_result)(self) -> [Result](https://doc.rust-lang.org/1.54.0/core/result/enum.Result.html "enum core::result::Result")&lt;[JsonValue](https://docs.rs/serde_json/1.0.66/serde_json/value/enum.Value.html "enum serde_json::value::Value"), [JsonValue](https://docs.rs/serde_json/1.0.66/serde_json/value/enum.Value.html "enum serde_json::value::Value")>[\[src\]](/docs/api/rust/tauri/../src/tauri/hooks.rs#91-96 "goto source code")

Turn a [`InvokeResponse`](/docs/api/rust/tauri/enum.InvokeResponse "InvokeResponse") back into a serializable result.

## Trait Implementations

### impl [Debug](https://doc.rust-lang.org/1.54.0/core/fmt/trait.Debug.html "trait core::fmt::Debug") for [InvokeResponse](/docs/api/rust/tauri/enum.InvokeResponse "enum tauri::InvokeResponse")[\[src\]](/docs/api/rust/tauri/../src/tauri/hooks.rs#80 "goto source code")

#### fn [fmt](https://doc.rust-lang.org/1.54.0/core/fmt/trait.Debug.html#tymethod.fmt)(&self, f: &mut [Formatter](https://doc.rust-lang.org/1.54.0/core/fmt/struct.Formatter.html "struct core::fmt::Formatter")&lt;'\_>) -> [Result](https://doc.rust-lang.org/1.54.0/core/fmt/type.Result.html "type core::fmt::Result")[\[src\]](/docs/api/rust/tauri/../src/tauri/hooks.rs#80 "goto source code")

Formats the value using the given formatter. [Read more](https://doc.rust-lang.org/1.54.0/core/fmt/trait.Debug.html#tymethod.fmt)

### impl [From](https://doc.rust-lang.org/1.54.0/core/convert/trait.From.html "trait core::convert::From")&lt;[InvokeError](/docs/api/rust/tauri/struct.InvokeError "struct tauri::InvokeError")> for [InvokeResponse](/docs/api/rust/tauri/enum.InvokeResponse "enum tauri::InvokeResponse")[\[src\]](/docs/api/rust/tauri/../src/tauri/hooks.rs#112-116 "goto source code")

#### fn [from](https://doc.rust-lang.org/1.54.0/core/convert/trait.From.html#tymethod.from)(error: [InvokeError](/docs/api/rust/tauri/struct.InvokeError "struct tauri::InvokeError")) -> Self[\[src\]](/docs/api/rust/tauri/../src/tauri/hooks.rs#113-115 "goto source code")

Performs the conversion.

### impl&lt;T: [Serialize](https://docs.rs/serde/1.0.129/serde/ser/trait.Serialize.html "trait serde::ser::Serialize")> [From](https://doc.rust-lang.org/1.54.0/core/convert/trait.From.html "trait core::convert::From")&lt;[Result](https://doc.rust-lang.org/1.54.0/core/result/enum.Result.html "enum core::result::Result")&lt;T, [InvokeError](/docs/api/rust/tauri/struct.InvokeError "struct tauri::InvokeError")>> for [InvokeResponse](/docs/api/rust/tauri/enum.InvokeResponse "enum tauri::InvokeResponse")[\[src\]](/docs/api/rust/tauri/../src/tauri/hooks.rs#99-110 "goto source code")

#### fn [from](https://doc.rust-lang.org/1.54.0/core/convert/trait.From.html#tymethod.from)(result: [Result](https://doc.rust-lang.org/1.54.0/core/result/enum.Result.html "enum core::result::Result")&lt;T, [InvokeError](/docs/api/rust/tauri/struct.InvokeError "struct tauri::InvokeError")>) -> Self[\[src\]](/docs/api/rust/tauri/../src/tauri/hooks.rs#101-109 "goto source code")

Performs the conversion.

## Auto Trait Implementations

### impl [RefUnwindSafe](https://doc.rust-lang.org/1.54.0/std/panic/trait.RefUnwindSafe.html "trait std::panic::RefUnwindSafe") for [InvokeResponse](/docs/api/rust/tauri/enum.InvokeResponse "enum tauri::InvokeResponse")

### impl [Send](https://doc.rust-lang.org/1.54.0/core/marker/trait.Send.html "trait core::marker::Send") for [InvokeResponse](/docs/api/rust/tauri/enum.InvokeResponse "enum tauri::InvokeResponse")

### impl [Sync](https://doc.rust-lang.org/1.54.0/core/marker/trait.Sync.html "trait core::marker::Sync") for [InvokeResponse](/docs/api/rust/tauri/enum.InvokeResponse "enum tauri::InvokeResponse")

### impl [Unpin](https://doc.rust-lang.org/1.54.0/core/marker/trait.Unpin.html "trait core::marker::Unpin") for [InvokeResponse](/docs/api/rust/tauri/enum.InvokeResponse "enum tauri::InvokeResponse")

### impl [UnwindSafe](https://doc.rust-lang.org/1.54.0/std/panic/trait.UnwindSafe.html "trait std::panic::UnwindSafe") for [InvokeResponse](/docs/api/rust/tauri/enum.InvokeResponse "enum tauri::InvokeResponse")

## Blanket Implementations

### impl&lt;T> [Any](https://doc.rust-lang.org/1.54.0/core/any/trait.Any.html "trait core::any::Any") for T where T: 'static + ?[Sized](https://doc.rust-lang.org/1.54.0/core/marker/trait.Sized.html "trait core::marker::Sized"),[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/any.rs.html#131-135 "goto source code")

#### pub fn [type_id](https://doc.rust-lang.org/1.54.0/core/any/trait.Any.html#tymethod.type_id)(&self) -> [TypeId](https://doc.rust-lang.org/1.54.0/core/any/struct.TypeId.html "struct core::any::TypeId")[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/any.rs.html#132 "goto source code")

Gets the `TypeId` of `self`. [Read more](https://doc.rust-lang.org/1.54.0/core/any/trait.Any.html#tymethod.type_id)

### impl&lt;T> [Borrow](https://doc.rust-lang.org/1.54.0/core/borrow/trait.Borrow.html "trait core::borrow::Borrow")&lt;T> for T where T: ?[Sized](https://doc.rust-lang.org/1.54.0/core/marker/trait.Sized.html "trait core::marker::Sized"),[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/borrow.rs.html#208-213 "goto source code")

#### pub fn [borrow](https://doc.rust-lang.org/1.54.0/core/borrow/trait.Borrow.html#tymethod.borrow)(&self) -> [&](https://doc.rust-lang.org/1.54.0/std/primitive.reference.html)T[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/borrow.rs.html#210 "goto source code")

Immutably borrows from an owned value. [Read more](https://doc.rust-lang.org/1.54.0/core/borrow/trait.Borrow.html#tymethod.borrow)

### impl&lt;T> [BorrowMut](https://doc.rust-lang.org/1.54.0/core/borrow/trait.BorrowMut.html "trait core::borrow::BorrowMut")&lt;T> for T where T: ?[Sized](https://doc.rust-lang.org/1.54.0/core/marker/trait.Sized.html "trait core::marker::Sized"),[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/borrow.rs.html#216-220 "goto source code")

#### pub fn [borrow_mut](https://doc.rust-lang.org/1.54.0/core/borrow/trait.BorrowMut.html#tymethod.borrow_mut)(&mut self) -> [&mut](https://doc.rust-lang.org/1.54.0/std/primitive.reference.html)T[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/borrow.rs.html#217 "goto source code")

Mutably borrows from an owned value. [Read more](https://doc.rust-lang.org/1.54.0/core/borrow/trait.BorrowMut.html#tymethod.borrow_mut)

### impl&lt;T> [From](https://doc.rust-lang.org/1.54.0/core/convert/trait.From.html "trait core::convert::From")&lt;T> for T[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/convert/mod.rs.html#544-548 "goto source code")

#### pub fn [from](https://doc.rust-lang.org/1.54.0/core/convert/trait.From.html#tymethod.from)(t: T) -> T[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/convert/mod.rs.html#545 "goto source code")

Performs the conversion.

### impl&lt;T, U> [Into](https://doc.rust-lang.org/1.54.0/core/convert/trait.Into.html "trait core::convert::Into")&lt;U> for T where U: [From](https://doc.rust-lang.org/1.54.0/core/convert/trait.From.html "trait core::convert::From")&lt;T>,[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/convert/mod.rs.html#533-540 "goto source code")

#### pub fn [into](https://doc.rust-lang.org/1.54.0/core/convert/trait.Into.html#tymethod.into)(self) -> U[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/convert/mod.rs.html#537 "goto source code")

Performs the conversion.

### impl&lt;T, U> [TryFrom](https://doc.rust-lang.org/1.54.0/core/convert/trait.TryFrom.html "trait core::convert::TryFrom")&lt;U> for T where U: [Into](https://doc.rust-lang.org/1.54.0/core/convert/trait.Into.html "trait core::convert::Into")&lt;T>,[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/convert/mod.rs.html#581-590 "goto source code")

#### type [Error](https://doc.rust-lang.org/1.54.0/core/convert/trait.TryFrom.html#associatedtype.Error) = [Infallible](https://doc.rust-lang.org/1.54.0/core/convert/enum.Infallible.html "enum core::convert::Infallible")

The type returned in the event of a conversion error.

#### pub fn [try_from](https://doc.rust-lang.org/1.54.0/core/convert/trait.TryFrom.html#tymethod.try_from)(value: U) -> [Result](https://doc.rust-lang.org/1.54.0/core/result/enum.Result.html "enum core::result::Result")&lt;T, &lt;T as [TryFrom](https://doc.rust-lang.org/1.54.0/core/convert/trait.TryFrom.html "trait core::convert::TryFrom")&lt;U>>::[Error](https://doc.rust-lang.org/1.54.0/core/convert/trait.TryFrom.html#associatedtype.Error "type core::convert::TryFrom::Error")>[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/convert/mod.rs.html#587 "goto source code")

Performs the conversion.

### impl&lt;T, U> [TryInto](https://doc.rust-lang.org/1.54.0/core/convert/trait.TryInto.html "trait core::convert::TryInto")&lt;U> for T where U: [TryFrom](https://doc.rust-lang.org/1.54.0/core/convert/trait.TryFrom.html "trait core::convert::TryFrom")&lt;T>,[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/convert/mod.rs.html#567-576 "goto source code")

#### type [Error](https://doc.rust-lang.org/1.54.0/core/convert/trait.TryInto.html#associatedtype.Error) = &lt;U as [TryFrom](https://doc.rust-lang.org/1.54.0/core/convert/trait.TryFrom.html "trait core::convert::TryFrom")&lt;T>>::[Error](https://doc.rust-lang.org/1.54.0/core/convert/trait.TryFrom.html#associatedtype.Error "type core::convert::TryFrom::Error")

The type returned in the event of a conversion error.

#### pub fn [try_into](https://doc.rust-lang.org/1.54.0/core/convert/trait.TryInto.html#tymethod.try_into)(self) -> [Result](https://doc.rust-lang.org/1.54.0/core/result/enum.Result.html "enum core::result::Result")&lt;U, &lt;U as [TryFrom](https://doc.rust-lang.org/1.54.0/core/convert/trait.TryFrom.html "trait core::convert::TryFrom")&lt;T>>::[Error](https://doc.rust-lang.org/1.54.0/core/convert/trait.TryFrom.html#associatedtype.Error "type core::convert::TryFrom::Error")>[\[src\]](https://doc.rust-lang.org/1.54.0/src/core/convert/mod.rs.html#573 "goto source code")

Performs the conversion.

### impl&lt;V, T> VZip&lt;V> for T where V: MultiLane&lt;T>,

#### pub fn [vzip](/docs/api/rust/tauri/about:blank#tymethod.vzip)(self) -> V
  