# @correxit/contracts Changelog

## 1.0.0

Initial release of `@correxit/contracts`.

- Published `Collector`, `Distributor`, `Registrar`, `Submitter`, and `Unlocker`
  types and tokens independently from Correxit.
- Uses Correxit's `AGPL-3.0-only` license and scheduled `BSD-3-Clause`
  transition on 1 January 2028.
- Replaced internal model parameters with plain-data payloads.
- Changed `Unlocker.request()` to yield credentials through an async iterable.
  `store()` retains author keys; Correxit handles authentication and decryption.
- Creation requests include a proposed rubric identity before credentials are
  acquired; the same ID is retained through key storage and workbook creation.

See the [migration guide](https://github.com/correxit/correxit/blob/main/docs/plugins.md#migrating-existing-plugins)
for changes required in existing plugins.
