### Hi, I'm Sunmin 👋

Backend developer working mainly with **Java** and **Spring Boot**.

I'm interested in open source 

---

## 🌍 Open Source Contributions

`✅ Merged` &nbsp;·&nbsp; `🔍 In review` &nbsp;·&nbsp; `📝 Draft` &nbsp;·&nbsp; `💬 Open discussion`

<details>
<summary><b>docker/docs</b> &nbsp;—&nbsp; 6 merged</summary>

<br>

Mostly BuildKit caching docs: corrected a wrong description of the **local cache backend**,
documented its undocumented `tag` and `reset` parameters, then fixed arithmetic in a
build cache GC policy example.

| | Type | Title | Status |
|:--|:--|:--|:--|
| [#26025](https://github.com/docker/docs/pull/26025) | PR | Restore `/docker-for-windows/troubleshoot/` alias | ✅ Merged |
| [#26016](https://github.com/docker/docs/pull/26016) | PR | Fix arithmetic in build cache GC policy example | ✅ Merged |
| [#25977](https://github.com/docker/docs/pull/25977) | PR | Replace GHA local cache workaround with `reset` | ✅ Merged |
| [#25976](https://github.com/docker/docs/pull/25976) | PR | Document `reset` parameter for local cache backend | ✅ Merged |
| [#25943](https://github.com/docker/docs/pull/25943) | PR | Document `tag` parameter and restructure local cache versioning | ✅ Merged |
| [#25942](https://github.com/docker/docs/pull/25942) | PR | Fix incorrect description in local cache page | ✅ Merged |

</details>

<details>
<summary><b>apache/kafka</b> &nbsp;—&nbsp; 1 merged &nbsp;·&nbsp; 1 in review</summary>

<br>

| | Type | Title | Status |
|:--|:--|:--|:--|
| [#23390](https://github.com/apache/kafka/pull/23390) | PR | `KAFKA-21034`: Wipe the global state directory when the store is corrupted | 🔍 In review |
| [#23344](https://github.com/apache/kafka/pull/23344) | PR | `MINOR`: Replace `Collections`/`Arrays` factory methods with Java 9+ equivalents in tools | ✅ Merged |

</details>

<details>
<summary><b>opensearch-project/OpenSearch</b> &nbsp;—&nbsp; 1 draft</summary>

<br>

Picking up [#22961](https://github.com/opensearch-project/OpenSearch/issues/22961): the DSL
query translators silently ignored `boost` and `_name` in some queries while rejecting them
in others. Making the policy uniform across translators.

| | Type | Title | Status |
|:--|:--|:--|:--|
| [#22981](https://github.com/opensearch-project/OpenSearch/pull/22981) | PR | Reject unsupported DSL query options | 📝 Draft |

</details>

<details>
<summary><b>moby/buildkit</b> &nbsp;—&nbsp; 1 open</summary>

<br>

While documenting `reset` for docker/docs, I found the flag can race with a concurrent
export and reported it upstream.

| | Type | Title | Status |
|:--|:--|:--|:--|
| [#7102](https://github.com/moby/buildkit/issues/7102) | Issue | local cache exporter: `reset=true` can delete blobs from a concurrent export | 💬 Open discussion |

</details>
