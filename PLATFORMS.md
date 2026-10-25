# Find the lab that looks like your work

The catalog separates application stacks from platforms where people build or deploy them. “Source available” means the repository and exercises exist. It does not mean the application is hosted, a platform import has been verified, or a ContextQA test has passed.

## Choose your application

| Your environment | Public learning example | What you practice |
|---|---|---|
| Modern .NET / distributed services | .NET eShop | Catalog, basket, authentication and checkout assertions; multi-service setup |
| ASP.NET Core / monolith | eShopOnWeb | Server-rendered commerce and domain workflows; compare architecture with modern eShop |
| Java / Spring Boot | Spring PetClinic | Owners, pets, visits and persisted relationships |
| Older Java MVC / JSP | Spring Framework PetClinic | Server-rendered forms, validation and navigation; repeat equivalent business assertions across a modernization |
| Node.js / Express API | MERN example's server | Create/read/update/delete records; compare UI observations with API state |
| MERN | MongoDB employee-records sample | React → Express → MongoDB CRUD, persistence and invalid input |
| Angular | Conduit | Authentication, publishing, comments, profiles and pagination |
| React | Simulated payments sample | Recipient, amount, history and filtering |
| Next.js / Vercel | Next.js Learn dashboard | Authentication, invoice forms, search, pagination and server/client boundaries |
| SAP Fiori / UI5 / CAP | SAP event registration sample | End-user forms, administrator view, OData V4 and draft behavior |
| Salesforce Lightning / LWC | E-Bikes | Product search and reseller workflow in an authorized Salesforce org |
| Salesforce Visualforce → LWC | Official migration examples | Preserve a chosen behavior while moving from Visualforce to Lightning components |
| Plain HTML / JavaScript | TodoMVC | A short add/edit/filter/persistence exercise and a disclosed failing variant |

ASP.NET Core monolith is not classic .NET Framework/Web Forms. Spring MVC/JSP is an older architectural style, not proof of compatibility with an arbitrary old Java runtime. Keep versions explicit and supported for public hosting.

## Choose where you built it

### Vercel / Next.js

Start with the Next.js dashboard fork. Choose the finished application under `dashboard/final-example` after checking the current source tree; do not publish a starting skeleton as a complete demo. Follow its database, auth and environment setup before importing into Vercel. A protected preview must be reachable by an authorized runner through a supported method; never switch off deployment protection merely to make a test pass.

Lesson: create an invoice, assert the rendered amount and customer, reject invalid input, edit it and verify the list after reload. Repeat against an explicitly selected preview deployment after a code change. Source code, environment settings and data fixtures are separate parts of reproducibility. A GitHub import is not a verified deployment.

Source: https://vercel.com/docs/frameworks/full-stack/nextjs

### Lovable

Lead with **“Test the app you just built.”** Use the learner's own published app URL and inspect its actual business flow; a React/Vite reference exercise is a familiar starting point, not evidence that the reference was authored in Lovable.

Current Lovable documentation describes GitHub export/two-way sync. Existing repository code can be imported as a ZIP into a new project; Git sync itself creates a new repository rather than attaching an arbitrary existing one. Check compatibility and credentials before import. Do not offer a fake “Open in Lovable” button for every stack.

Lesson: create an example booking or record, verify its saved state, reject invalid input, then check isolation between two authorized test users where the application implements authentication. For Supabase-backed apps, separately verify the permission boundary; a hidden button is not authorization. No Lovable-authored lab or Supabase policy check is claimed yet.

Source: https://docs.lovable.dev/integrations/github

### Replit

Start with the MERN repository or a learner-owned Node/React app. Replit documents GitHub imports; importing files does not import secrets, external service configuration or database contents. Check client/server startup commands and database connectivity. Do not claim that importing a repo makes it runnable without configuration.

Lesson: import → configure the actual server/client and synthetic database → run → publish an authorized deployment → test CRUD → inspect persistence after reload. A workspace preview and a published deployment may have different URLs and settings; record which one was tested. No Replit import or deployment is verified in this release.

Source: https://docs.replit.com/build/import-from-providers

## SAP old and new: represent the real boundary

The public SAP sample demonstrates UI5/Fiori web interfaces with a Node CAP backend and OData V4 drafts. It is not SAP ECC, S/4HANA or an ABAP backend. Its own documentation says deployment authentication/database considerations are not covered; its development credentials must not become shared public production credentials.

Separate enterprise lessons require real, authorized environments:

* ECC/classic browser surfaces, including SAP GUI for HTML/WebGUI or Web Dynpro: use a dedicated sandbox and synthetic business records. Record the exact surface and version. A WebGUI test is not a native Windows SAP GUI test.
* S/4HANA/Fiori: verify actual launchpad navigation, role, application, backend and allowed OData access in a tenant. A UI5 sample alone does not prove a tenant business transaction works.
* Native SAP GUI for Windows: keep this as a distinct desktop-runner qualification task. Do not promise it from the browser examples or display it as runnable here.

Source sample: https://github.com/SAP-samples/ui5-cap-event-app

## Salesforce old and new

The E-Bikes and Visualforce-to-LWC source forks require Salesforce Platform. Use an authorized scratch org, Developer Edition org or suitable sandbox per upstream instructions. A GitHub fork is not a Salesforce deployment. Avoid a shared admin login. Users, permission sets, seeded records, org expiry and cleanup need a separate setup path.

The migration sample provides paired Visualforce/LWC patterns. Choose an actual pair in the source and repeat its behavioral assertions on both. This is not automatic proof of Salesforce Classic coverage, and it is not permission to test a customer production org. Classic workflows need an explicitly configured Classic environment.

Sources: https://github.com/trailheadapps/ebikes-lwc ; https://github.com/trailheadapps/visualforce-to-lwc

## Beyond this release

Requested future examples can include Python/Django/FastAPI, PHP/Laravel, Vue/Nuxt, Ruby/Rails, Svelte and classic ASP.NET Framework/Web Forms. They remain unselected until a maintained, appropriately licensed real application and useful business journey pass review. Users can still bring an authorized reachable application URL; that is not a blanket compatibility certification.

## Content that connects to each audience

Build four playlists: modern developer stacks; older-app modernization; enterprise SAP/Salesforce; and AI app builders. Every episode links to its precise source, version, setup requirements and actual report when available.

Use a migration challenge for Java MVC → Spring Boot and Visualforce → LWC: “Did the behavior survive the migration?” Use a release challenge for Vercel/Lovable/Replit: “Did this change break the app I just shipped?” Use an enterprise scenario only in a genuine sandbox with role-appropriate records. The common promise is inspectable business assertions, not identical infrastructure.
