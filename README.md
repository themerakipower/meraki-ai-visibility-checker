# Meraki AI Visibility Readiness Checker

Free homepage assessment by [The Meraki Power](https://www.themerakipower.com/).

## Deployment

1. Create a free Cloudflare Worker at https://dash.cloudflare.com/ and paste the contents of `worker.js` into it.
2. Deploy the Worker and copy its public `workers.dev` URL.
3. Replace `YOUR_WORKER_URL_HERE` in `index.html` with that URL and commit the change.
4. In GitHub go to Settings > Pages > Deploy from a branch > `main` > `/ (root)` > Save.
5. Test with a public HTTPS domain.

## Assessment

Title (15 points), meta description (15), H1 (15), JSON-LD presence (20), about/company information (10), contact cues (10), and readable homepage text (15).

This is a heuristic homepage readiness check, not a measurement of AI search rankings, citations or ChatGPT recommendations. It does not validate schema. Sites using client-rendered content, redirects, or bot protection may not be assessed correctly. Before promoting the public endpoint, implement rate limiting and stronger network-level SSRF protection. The code does not store scan history, but hosting infrastructure may log requests.
