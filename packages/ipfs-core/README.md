# ipfs-core w/ block storage access <!-- omit in toc -->

Experiment. A clone of the [original ipfs-core](https://github.com/ipfs/js-ipfs/tree/master/packages/ipfs-core) exposing the block storage to allow publishing precomputed CIDs.

## Usage

```js
import * as IPFS from '@dstanesc/ipfs-core-store-access'

const ipfs = await IPFS.create()

const cid = ...
const bytes = ...

// write
await ipfs.store.blocks.put(cid, bytes)

//read
const buf = await ipfs.store.blocks.get(cid)
```

## License

Licensed under either of

- Apache 2.0, ([LICENSE-APACHE](LICENSE-APACHE) / <http://www.apache.org/licenses/LICENSE-2.0>)
- MIT ([LICENSE-MIT](LICENSE-MIT) / <http://opensource.org/licenses/MIT>)

## Contribute

Contributions welcome! Please check out [the issues](https://github.com/ipfs/js-ipfs/issues).

Also see our [contributing document](https://github.com/ipfs/community/blob/master/CONTRIBUTING_JS.md) for more information on how we work, and about contributing in general.

Please be aware that all interactions related to this repo are subject to the IPFS [Code of Conduct](https://github.com/ipfs/community/blob/master/code-of-conduct.md).

Unless you explicitly state otherwise, any contribution intentionally submitted for inclusion in the work by you, as defined in the Apache-2.0 license, shall be dual licensed as above, without any additional terms or conditions.

[![](https://cdn.rawgit.com/jbenet/contribute-ipfs-gif/master/img/contribute.gif)](https://github.com/ipfs/community/blob/master/CONTRIBUTING.md)
