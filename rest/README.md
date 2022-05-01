# Translate - leveraging Cognitive Services

TBD

## Structure

TBD

### Setup

You will need to create a .env file at the same location of the rest scripts - this is the content it will require:

```bash
cog_key= <your cognitive service key>
translate_base_url = <the name of your cognitive resource>
lang = <desired lang to translate to>
target_container = <sas token with r/a/c/w/d/l >
source_container = <sas token with r/l >
```

Each of the `rest` script files has few references to the `.env` file but also defines few variables, name and such.
