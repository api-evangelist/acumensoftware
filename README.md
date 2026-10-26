# Acumen Software

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Acumen Software is a Johannesburg, South Africa software company founded in 2006 that builds highly
configurable mobile SaaS for work, workforce and asset management.

- **Forcelink** (https://www.forcelink.net/) — a mobile field-service ERP covering work management,
  workforce scheduling, asset and materials management, fleet, project, facilities, CRM and outage
  management (Powerlink), sold into power and water utilities, telecoms, transport, healthcare, forestry,
  mining, roads, waste, local government and municipal councils.
- **My Smart City** (https://www.mysmart.city/) — a citizen-engagement platform for logging municipal
  service faults, booking vetted service providers, submitting self-meter readings and paying municipal
  accounts. It runs on the Forcelink back end.

## What this profile found

Both product APIs are real and both are entirely closed. Every path under
`https://za2.forcelink.net/forcelink/rest` and `https://app.mysmart.city/api/msc/rest` answers HTTP 401 with
`{"error":"No authentication method supplied"}` to anonymous callers — including paths that do not exist, so
the 401 is a blanket filter and not evidence of a document behind it. Acumen Software publishes no developer
portal, no API reference, and no machine-readable contract (no OpenAPI, AsyncAPI, GraphQL SDL, WSDL or
`.proto` was found on any host).

What the company does serve publicly: an `llms.txt` on each of its three marketing domains, and a live,
anonymous MCP endpoint at `/_api/mcp` on each of those same domains. Both are generated by the Wix website
platform rather than written by Acumen Software, and the nine MCP tools are Wix site and Wix-docs tools —
they do not expose Forcelink or My Smart City data. That authorship is recorded in
`mcp/acumensoftware-mcp.yml` and `llms/acumensoftware-llms.yml` rather than credited as a first-party agent
surface.

Secondary-market listing this company was surfaced from: https://equityzen.com/company/acumensoftware
