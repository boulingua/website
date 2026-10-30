# Boulingua website

The suite's public introduction, language map and navigation hub, authored by
S. Le Boulanger. It connects the three established courses, fifteen developing
courses, resource catalogue and reading products. See the organisation's
[architecture](https://github.com/boulingua/.github/blob/main/docs/suite-architecture.md)
and this repository's [refinement record](REFINEMENT.md) for current scope.

Live site: <https://boulingua.github.io/website/>. The local refinement candidate
has not been deployed.

## Build and preview

Prerequisites: Hugo extended 0.159.2, Go 1.26.1, Python 3.12 and Node 22.
Place matching `kit`, `curriculum`, `.github` and `website` checkouts beside one
another. The refinement candidate requires its matching unpublished checkouts;
existing public dependency tags do not contain these changes yet.

From this repository:

```sh
python3.12 -m venv .venv
. .venv/bin/activate
pip install -r ../kit/requirements.txt
npm ci --prefix ../kit
npm exec --prefix ../kit -- playwright install chromium
go work init ../kit
export HUGO_MODULE_WORKSPACE="$PWD/go.work"
python ../kit/bin/kit build .
python ../kit/bin/kit check . --ci --owner-root curriculum=../curriculum --owner-root .github=../.github
mkdir -p build/preview
ln -s "$PWD/public" build/preview/website
python -m http.server 1317 --bind 127.0.0.1 --directory build/preview
```

Open <http://127.0.0.1:1317/website/>. The workspace and preview link are first-use
commands; reuse an existing matching workspace/link on subsequent runs.

Code is MIT; original content is CC BY-SA 4.0. Third-party assets retain their
documented licences. Release/deployment requires compatible published pins and
observed hosted checks; a local build alone is not a production deployment.
