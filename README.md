## Jait Ramadandi Jeke

Founding AI / Backend Engineer. I build production AI systems, distributed
backends, and the data infrastructure underneath them.

Most of my work is the unglamorous part of "AI product": making agent pipelines
survive restarts, making scraped data idempotent, making a model's answer
traceable to the document it came from, and keeping the cloud bill finite.

- **Now** — Founding AI Engineer at [Avvista.ai](https://avvista.ai), building
  tender intelligence for public procurement. Acquired by [Cato](https://get-cato.com).
- **Working on** — multi-agent systems, RAG and document extraction pipelines,
  event-driven backends, infrastructure-as-code.
- **Stack** — Python · Go · FastAPI · Django · PostgreSQL · Redis · Elasticsearch ·
  GCP · AWS · Terraform/OpenTofu · Kubernetes
- **Reach me** — [LinkedIn](https://linkedin.com/in/jait-rj) · jaitramadandij@gmail.com

---

### Selected work

**[SupplyMe](https://github.com/fillateo/SupplyMe)** — Autonomous multi-agent
supplier sourcing. Seven Gemini agents decompose a product into its supply
chain, find candidate factories, research them against the live web, email what
they can't find out, and rank the survivors with a deterministic score that
explains itself line by line.

The design constraint was that sourcing data isn't published, it's disclosed —
so most of the wall-clock time is spent waiting on a human. Every arrow in the
pipeline is a persisted event on Pub/Sub, so a Cloud Run restart mid-mission
loses nothing and a supplier replying three days later resumes the same mission.
LLM calls decide routing; scoring stays deterministic and auditable. Every fact
in the final report is clickable back to the source excerpt that produced it.

`FastAPI · Next.js · Vertex AI · Firestore · Pub/Sub · Cloud Tasks · Cloud Run · OpenTofu`

---

<img src="https://github-readme-stats.vercel.app/api?username=fillateo&show_icons=true&hide_border=true&locale=en" alt="GitHub stats" />
