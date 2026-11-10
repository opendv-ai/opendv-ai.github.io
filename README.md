# OpenDV: Crowdsourced drone videos for open drone vision and reasoning

Crowdsourced drone videos, flight logs and descriptions, released to the public for building perception and reasoning AI models for drone applications such as package delivery, search and rescue, and first response.

**Website:** https://opendv-ai.github.io/ </br>
**Contribute:** https://opendv-ai.github.io/collect.html

## What's collected

Each sample has three files with the same name:

| File | Example | Contents |
|---|---|---|
| Video | `DJI_0042.MP4` | Downward-facing camera, continuous recording |
| Flight log | `DJI_0042.SRT` | Per-frame altitude, GPS, camera settings |
| Description | `DJI_0042.txt` | One paragraph: time, weather, delivery spot, nearby objects, anything blocking the spot |

Flight profile: hover at 100–150 ft (30–45 m) → slow descent → hover at 25–30 ft (about 8–9 m). Full guide: [CONTRIBUTING.md](CONTRIBUTING.md).

## How submissions become data

```
Contributor ──upload──▶ Private Dropbox folder ──team review──▶ Hugging Face dataset (public)
```

Reviews cover safety, the flight profile and privacy (faces, plates, GPS). Rejected submissions are deleted.

## Dataset access

Hugging Face: https://huggingface.co/datasets/aarifahullah/OpenDV. Each published sample, including the team's own samples, includes its one-paragraph description.

## Privacy

Exact GPS locations are removed before release. Contributor names and emails are never published.

## License

- **Data:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Contributors keep copyright of their own videos and license them under CC BY 4.0. See [LICENSE-DATA](LICENSE-DATA).
- **Code** (website, tools): MIT. See [LICENSE](LICENSE).

## Team

The George Washington University: [Aarifah Ullah](https://aarifahullah.github.io/) (aarifahullah@gwu.edu), [Mahyar Ghazanfari](https://mahyar-gh79.github.io/) (mahyar.ghazanfari@gwu.edu), [Peng Wei](https://web.seas.gwu.edu/pwei/) (pwei@gwu.edu)
