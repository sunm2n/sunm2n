### Hi, I'm Sunmin 👋

Backend developer working mainly with **Java** and **Spring Boot**.

I'm interested in open source 

---

## 🌍 Open Source Contributions

`✅ Merged / resolved` &nbsp;·&nbsp; `🔍 In review` &nbsp;·&nbsp; `📝 Draft` &nbsp;·&nbsp; `💬 Open discussion`

<details>
<summary><b>docker/docs</b> &nbsp;-&nbsp; 6 merged &nbsp;·&nbsp; 3 in review</summary>

<br>

Started with BuildKit caching docs: corrected a wrong description of the **local cache
backend**, documented its undocumented `tag` and `reset` parameters, then fixed arithmetic
in a build cache GC policy example. Since then, smaller fixes across install and admin docs.

| | Type | Title | Status |
|:--|:--|:--|:--|
| [#26197](https://github.com/docker/docs/pull/26197) | PR | Correct GitHub Actions cache version selection | 🔍 In review |
| [#26087](https://github.com/docker/docs/pull/26087) | PR | Fix install options on the Raspberry Pi OS 32-bit page | 🔍 In review |
| [#26054](https://github.com/docker/docs/pull/26054) | PR | Scope the SCIM note in the team removal section | 🔍 In review |
| [#26025](https://github.com/docker/docs/pull/26025) | PR | Restore `/docker-for-windows/troubleshoot/` alias | ✅ Merged |
| [#26016](https://github.com/docker/docs/pull/26016) | PR | Fix arithmetic in build cache GC policy example | ✅ Merged |
| [#25977](https://github.com/docker/docs/pull/25977) | PR | Replace GHA local cache workaround with `reset` | ✅ Merged |
| [#25976](https://github.com/docker/docs/pull/25976) | PR | Document `reset` parameter for local cache backend | ✅ Merged |
| [#25943](https://github.com/docker/docs/pull/25943) | PR | Document `tag` parameter and restructure local cache versioning | ✅ Merged |
| [#25942](https://github.com/docker/docs/pull/25942) | PR | Fix incorrect description in local cache page | ✅ Merged |

</details>

<details>
<summary><b>apache/kafka</b> &nbsp;-&nbsp; 1 merged &nbsp;·&nbsp; 4 in review</summary>

<br>

Kafka Streams state management: two JIRA-tracked fixes around state directory cleanup
after a corrupted store or an interrupted shutdown, plus ongoing test and Java 9+ cleanup
across tools, storage, and Streams.

| | Type | Title | Status |
|:--|:--|:--|:--|
| [#23636](https://github.com/apache/kafka/pull/23636) | PR | `MINOR`: Replace try/fail/catch with `assertThrows` in remaining Streams tests | 🔍 In review |
| [#23617](https://github.com/apache/kafka/pull/23617) | PR | `MINOR`: Replace `Collections` factory methods with Java 9+ equivalents in storage tests | 🔍 In review |
| [#23549](https://github.com/apache/kafka/pull/23549) | PR | `KAFKA-21070`: Fix task cleanup when state updater shutdown is interrupted | 🔍 In review |
| [#23390](https://github.com/apache/kafka/pull/23390) | PR | `KAFKA-21034`: Wipe the global state directory when the store is corrupted | 🔍 In review |
| [#23344](https://github.com/apache/kafka/pull/23344) | PR | `MINOR`: Replace `Collections`/`Arrays` factory methods with Java 9+ equivalents in tools | ✅ Merged |

</details>

<details>
<summary><b>moby/buildkit</b> &nbsp;-&nbsp; 1 issue resolved</summary>

<br>

While documenting `reset` for docker/docs, I found the flag can race with a concurrent
export and reported it as #7102. A maintainer opened #7153 to fix it; I built both branches
and re-ran the reproduction to confirm the patch closes the race. Merged to `master` after
v0.33.0, and #7102 closed as completed.

| | Type | Title | Status |
|:--|:--|:--|:--|
| [#7153](https://github.com/moby/buildkit/pull/7153#issuecomment-5785957508) | Verification | `client`: protect concurrent local cache exports from `reset`, a maintainer's fix for #7102 that I verified against the reported repro | ✅ Merged |
| [#7102](https://github.com/moby/buildkit/issues/7102) | Issue | local cache exporter: `reset=true` can delete blobs from a concurrent export | ✅ Resolved |

</details>

<details>
<summary><b>opensearch-project/OpenSearch</b> &nbsp;-&nbsp; 1 in review &nbsp;·&nbsp; 1 draft &nbsp;·&nbsp; 1 issue</summary>

<br>

Picked up [#22961](https://github.com/opensearch-project/OpenSearch/issues/22961): the DSL
query translators silently ignored `boost` and `_name` in some queries while rejecting them
in others. Working through that led to a second gap in the same area, filed as #23011.

| | Type | Title | Status |
|:--|:--|:--|:--|
| [#23014](https://github.com/opensearch-project/OpenSearch/pull/23014) | PR | Validate skipped optional `should` clauses | 📝 Draft |
| [#23011](https://github.com/opensearch-project/OpenSearch/issues/23011) | Issue | Unsupported `boost`/`_name` on optional `should` clauses is silently accepted | 💬 Open discussion |
| [#22981](https://github.com/opensearch-project/OpenSearch/pull/22981) | PR | Reject unsupported DSL query options | 🔍 In review |

</details>

<details>
<summary><b>Discussions</b> &nbsp;-&nbsp; 2 threads</summary>

<br>

Comments on other people's threads, mostly follow-on from the local cache work.

| Repo | Thread | What I added |
|:--|:--|:--|
| docker/buildx | [#310](https://github.com/docker/buildx/issues/310#issuecomment-5537817848) | Corrected which component gates `reset=true`, the **buildx** version rather than the builder's BuildKit, with the release each side landed in |
| docker/docs | [#13390](https://github.com/docker/docs/issues/13390#issuecomment-5564820406) | Traced which half of a 3-year-old report [#21420](https://github.com/docker/docs/pull/21420) had already fixed, and which part still stands. The reporter closed the thread a week later |

</details>
