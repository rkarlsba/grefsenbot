# README for GrefsenBot

## Konfigfil

Lag ei fil som heter grefsenbot_secrets.py og som inneholder noe sånt

```python
#!/usr/bin/env python3

from zoneinfo import ZoneInfo

HOST_IDENTIFIER = "somebot.example.com"
USER_AGENT = "GrefsenBot/0.6 somebot.example.com"
#OPENAI_API_KEY = "din-openai-nøkkel"               # Ikke i bruk (ennå?)
GROQ_API_KEY = "gsk_din_faktiske_nøkkel"            # Ikke i bruk (ennå?)

HOST = "::1"                                        # eller 127.0.0.1 hvis du ikke har fått med deg IPv6
PORT = 5234                                         # ellerno
LOCAL_TIMEZONE = ZoneInfo("Europe/Oslo")

CHANNELS = {
    0: "Public",
    1: "#noe",
    2: "#rart",
    3: "#bla",
}
```

Lag et python virtual environment:

```sh
python3 -m venv .venv
source .venv/bin/activate
```

Installér nødvendige biblioteker

```sh
pip install --upgrade pip
pip install -r requirements.txt
```

Snurr film!
