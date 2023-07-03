# giuppep.github.io

This is the source code for my website, which is published here: https://giuppep.github.io

## Development

The script `serve.sh` will start a [Jekyll](https://jekyllrb.com/) server locally on
port `4000` (requires [Docker](https://www.docker.com/)).

To test the website on other devices without publishing it, it's possible to use
[Cloudflare Tunnel](https://developers.cloudflare.com/cloudflare-one/connections/connect-apps/install-and-setup/tunnel-guide/local/)
to temporarily expose the locally served site on the public internet.
This can be easily done using Docker:

```bash
docker run --network="host" --rm cloudflare/cloudflared:latest tunnel --url http://127.0.0.1:4000/
```
