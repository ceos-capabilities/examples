# examples

Worked examples for the CEOS Capabilities API, the public read-only API behind the
[EO Capabilities Explorer](https://ceos-capabilities.org) (CEOS MIM Database).

| Example | Open |
|---|---|
| **Hello, MIM API** — download the identifier registry, count canonical entities by type, pull missions and instruments into pandas, plot a launch timeline. Start here. | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ceos-capabilities/examples/blob/main/hello-mim-api.ipynb) · [notebook](hello-mim-api.ipynb) |

## Running

- **Colab:** click the badge; no installation. The first cell sets `BASE_URL`
  (`https://ceos-capabilities.org/api`) and reads an optional API key from the
  `EOGOS_API_KEY` environment variable.
- **Locally:** `pip install pandas matplotlib requests jupyter`, then open the
  notebook. Python 3.10 or later.

## API access

The API is open without a key at 30 requests a second per address. A free key
raises that; ask at support@ceos-capabilities.org with your name, organisation
and intended use, and send it as the `X-API-Key` header (the notebook does this
when `EOGOS_API_KEY` is set). Keys are personal: keep them out of shared
notebooks and public code. Reference and rate limits:
https://ceos-capabilities.org/api · interactive docs: https://ceos-capabilities.org/api/docs

## Licence

Code in this repository: [MIT](LICENSE). The data the examples fetch is from the
CEOS MIM Database, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/);
cite "CEOS MIM Database (https://ceos-capabilities.org)" where you publish results.
