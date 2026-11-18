# Nabedra documentation

Mintlify site for Nabedra Database, the Python ORM, and Nabedra Events. The site documents [nabedra-database at `1418bad`](https://github.com/zPy52/nabedra-database/tree/1418bad88e1df1b8c868b88889a120e37059c1c0). See [docs.json](docs.json) for navigation and [index.mdx](index.mdx) for the landing page.

## Preview locally

Use Node.js 20.17 or newer. If `mint` is missing, run `npm install -g mint`.

```sh
mint dev
```

Open http://localhost:3000. To use another port, run `mint dev --port 3001`.

```sh
mint validate
mint broken-links
```

## Connect GitHub to Mintlify

1. Sign in at [Mintlify](https://mintlify.com/start) and create a project if needed.
2. Open the project's **Git settings** and select GitHub. Authorize GitHub when prompted and connect the existing `zPy52/nabedra-docs` repository. If your site already uses a Mintlify-hosted repository, select **Manual setup** to connect this one. Download any existing hosted docs from that wizard before switching.
3. Install the Mintlify GitHub App and grant it access to `zPy52/nabedra-docs` under **Only select repositories**.
4. Set the deployment branch to `main`. Keep the docs directory at the repository root, where `docs.json` is.
5. Save the connection and check the first deployment in the dashboard. Future pushes to `main` rebuild the site.

[Mintlify quickstart](https://www.mintlify.com/docs/quickstart) · [GitHub integration](https://www.mintlify.com/docs/deploy/github) · [CLI reference](https://www.mintlify.com/docs/cli)

## Update the docs

Add or edit an MDX file, then add new pages to the relevant navigation group in `docs.json`. Use site-root-relative links such as `/python/connect`. For behavior that depends on a particular release or acceptance run, cite the source revision or recorded evidence.

Portions of the documentation are adapted from the [Nabedra Database repository](https://github.com/zPy52/nabedra-database). See [LICENSE](LICENSE) for the upstream MIT notice.
