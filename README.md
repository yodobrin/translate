# Translate - leveraging Cognitive Services

TBD what?

## Structure

TBD

## Components

### Functions

#### Create Container

Inputs: name, required sas behaviour (flags)
Output: SAS token based on the flags

#### Upload to Container

Inputs: byte [], name
Output: boolean

#### Translate

Inputs: source, target (SAS tokens), translateTo
Output: operationID

#### Status

Inputs: operationID
Output: boolean

### REST Setup

You will need to create a .env file at the same location of the rest scripts - this is the content it will require:

```bash
cog_key= <your cognitive service key>
translate_base_url = <the name of your cognitive resource>
lang = <desired lang to translate to>
target_container = <sas token with r/a/c/w/d/l >
source_container = <sas token with r/l >
```

Each of the `rest` script files has few references to the `.env` file but also defines few variables, name and such.
