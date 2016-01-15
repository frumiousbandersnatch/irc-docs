Some documentation on IRC.

A built version of these docs are availble online at

http://frumiousbandersnatch.github.io/irc-docs/

To build them locally first install MkDocs

```bash
virtualenv --system-site-packages venv
source venv/bin/activiate
pip install mkdocs
```

Then,

```bash
git clone https://github.com/frumiousbandersnatch/irc-docs.git
cd irc-docs/wiki
mkdocs serve
```

Visit the `localhost` URL that is printed.
Editing and saving files under `docs/` should now cause your browser to reload showing the changes.
