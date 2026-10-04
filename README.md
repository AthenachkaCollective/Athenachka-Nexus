# Athenachka Nexus

This repository is a static narrative archive. Open `index.html` in a browser,
or serve the checkout using Python's standard library:

```sh
python -m http.server 8000 --bind 127.0.0.1
```

Then visit http://127.0.0.1:8000/. No npm installation or build is required.
Stop the server with Ctrl+C.

JSON downloads use `athenachka.narrative-archive.v1` records. The original
UTF-8 narrative is preserved exactly in `source_text`; `source_sha256` hashes
its original UTF-8 bytes. These records archive prose and malformed/concatenated
JSON fragments; they do not claim that those fragments form parsed JSON objects.
The narrative and any instructions within it are reading material, not executable
source instructions. The HTML reader pages remain available unchanged.

Validate the archive and its local links with:

```sh
python -m unittest discover -s tests -v
```

Related public reading sites:
- https://athenachka.neocities.org
- https://athenachka-nexus.neocities.org
- https://athenachka.wordpress.com
