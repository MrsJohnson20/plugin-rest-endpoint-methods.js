---
name: Update a release
example: octokit.rest.repos.updateRelease({ owner, repo, release_id })
route: PATCH /repos/{owner}/{repo}/releases/{release_id}
scope: repos
type: API method
---

# Update a release

Users with push access to the repository can edit a release.

```js
octokit.rest.repos.updateRelease({
  owner,
  repo,
  release_id,
});
```

## Parameters

<table>
  <thead>
    <tr>
      <th>name</th>
      <th>required</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>owner</td><td>yes</td><td>

</td></tr>
<tr><td>repo</td><td>yes</td><td>

</td></tr>
<tr><td>release_id</td><td>yes</td><td>

release_id parameter

</td></tr>
<tr><td>tag_name</td><td>no</td><td>

The name of the tag.

</td></tr>
<tr><td>target_commitish</td><td>no</td><td>

Specifies the commitish value that determines where the Git tag is created from. Can be any branch or commit SHA. Unused if the Git tag already exists. Default: the repository's default branch (usually `master`).

</td></tr>
<tr><td>name</td><td>no</td><td>

The name of the release.

</td></tr>
<tr><td>body</td><td>no</td><td>

Text describing the contents of the tag.

</td></tr>
<tr><td>draft</td><td>no</td><td>

`true` makes the release a draft, and `false` publishes the release.

</td></tr>
<tr><td>prerelease</td><td>no</td><td>

`true` to identify the release as a prerelease, `false` to identify the release as a full release.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/reference/repos#update-a-release).
