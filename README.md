<a href="https://contextqaai.github.io/testing-lab/"><img src="lab/assets/contextqa-logo.svg" alt="ContextQA" width="200"></a>

# ContextQA Testing Lab

Real source. Explicit assertions. Reproducible failures.

Choose by stack, deployment platform, or modernization task. [Full stack/platform guidance](PLATFORMS.md) covers Vercel, Lovable, Replit, SAP old/new, and Salesforce Visualforce/Lightning.

Learn to test an application end to end, inspect the evidence, introduce a regression and repeat the workflow on an application you own.

| Track | Source / exercise | Environment |
|---|---|---|
| React payments | [Open guide](https://github.com/contextqaai/testing-lab-react-payments/blob/develop/lab/README.md) | Source + exercises; hosting pending |
| Angular workflows | [Open guide](https://github.com/contextqaai/testing-lab-angular-conduit/blob/main/lab/README.md) | Source + exercises; hosting pending |
| Java Spring Boot | [Open guide](https://github.com/contextqaai/testing-lab-java-petclinic/blob/main/lab/README.md) | Source + exercises; hosting pending |
| HTML / JavaScript starter | [Open guide](https://github.com/contextqaai/testing-lab-html-todomvc/blob/master/lab/README.md) | Hosted practice app |
| Modern .NET · eShop | [Open guide](https://github.com/contextqaai/testing-lab-dotnet-eshop/blob/main/lab/README.md) | Source + exercises; deployment pending |
| ASP.NET Core · monolith | [Open guide](https://github.com/contextqaai/testing-lab-dotnet-monolith/blob/main/lab/README.md) | Source + exercises; deployment pending |
| MERN · React + Express + MongoDB | [Open guide](https://github.com/contextqaai/testing-lab-mern-records/blob/main/lab/README.md) | Source + exercises; deployment pending |
| Java · Spring MVC / JSP | [Open guide](https://github.com/contextqaai/testing-lab-java-mvc-jsp/blob/main/lab/README.md) | Source + exercises; deployment pending |
| SAP web · Fiori / UI5 / CAP | [Open guide](https://github.com/contextqaai/testing-lab-sap-fiori-cap/blob/main/lab/README.md) | Source + exercises; deployment pending |
| Salesforce · Lightning / LWC | [Open guide](https://github.com/contextqaai/testing-lab-salesforce-lwc/blob/main/lab/README.md) | Requires Salesforce org |
| Salesforce · Visualforce → LWC | [Open guide](https://github.com/contextqaai/testing-lab-salesforce-visualforce/blob/main/lab/README.md) | Requires Salesforce org |
| Next.js · Vercel dashboard | [Open guide](https://github.com/contextqaai/testing-lab-nextjs-vercel/blob/main/lab/README.md) | Source + exercises; deployment pending |
| Node.js / Express API | [Open guide](https://github.com/contextqaai/testing-lab-mern-records/blob/main/lab/NODE-API.md) | Source + API lesson; hosting pending |
| Built with Lovable | [Open guide](PLATFORMS.md#lovable) | Platform guide; no Lovable-built deployment verified |
| Built with Replit | [Open guide](PLATFORMS.md#replit) | Platform guide; import/deployment unverified |
| SAP ECC / S/4HANA / classic GUI | [Open guide](PLATFORMS.md#sap-old-and-new-represent-the-real-boundary) | Sandbox/runner required; no live environment |

## The learning journey

1. Explore a real application's source and run your own copy.
2. Pick an explicit business assertion and create/review the test in your authenticated ContextQA workspace.
3. Execute and inspect the actual runner's verdict and evidence.
4. Introduce a disclosed regression, repeat the test, fix the app and rerun.
5. Repeat on an application you own or are authorized to test.

[ContextQA setup](https://contextqa.com/tutorials/getting-started-with-contextqa-test-automation/) · [MCP setup and FAQ](https://mcp.contextqa.com/docs/faq)

## Evidence policy

No ContextQA execution result has been produced for these forks yet. Exercises are not test receipts. Upstream tests are not ContextQA tests. Recorded examples, when published, will identify the app commit, fixture and scenario version, environment, tool/browser version and run timestamp. Fresh runs will be labeled separately. Failed assertions will remain visible.

## Local versus hosted

The HTML introduction uses localStorage in the browser. Other tracks require their backend and isolated data. A browser frontend alone is not a complete hosted React/Angular/Java lab. Localhost is not reachable from a cloud runner without a supported connection. Do not test upstream public demo services at scale.

## Courses and creator walkthroughs

The [content kit](content/README.md) includes a course outline, a flagship video script, an internal workshop and a creator brief. These are authoring assets; recordings, Udemy publication and creator agreements are not yet available.

## Attribution

React payments is an educational fork of Cypress's Real World App (MIT); Angular Conduit is a fork of realworld-apps/angular-realworld-example-app (MIT with separate Angular trademark notice); Java is a fork of Spring PetClinic (Apache-2.0); HTML is the vanilla JavaScript example from TodoMVC (MIT unless otherwise specified). Preserve upstream notices and inspect dependencies separately. These source projects do not imply upstream endorsement or production certification.

The [public hub](https://contextqaai.github.io/testing-lab/) and HTML app are deployed. The HTML lesson contrasts persistence across reloads with the original memory-only behavior. It is still not a ContextQA execution report.

## Expanded source attribution

Additional educational forks: dotnet/eShop and NimblePros/eShopOnWeb (MIT); mongodb-developer/mern-stack-example (Apache-2.0); spring-petclinic/spring-framework-petclinic (Apache-2.0); SAP-samples/ui5-cap-event-app (Apache-2.0 with exceptions in source); trailheadapps/ebikes-lwc and visualforce-to-lwc (CC0-1.0); vercel/next-learn (MIT). Source availability does not imply upstream endorsement, compatibility certification or hosted service availability.

## ContextQA learning resources

[Public learning hub](https://contextqaai.github.io/testing-lab/) · [Stack/platform setup](https://github.com/contextqaai/testing-lab/blob/main/PLATFORMS.md) · [Report or reproduce an issue](https://github.com/contextqaai/testing-lab/issues)

This is an educational learning resource. Original source, licenses and credits remain intact. Public report links appear only after actual execution; recorded evidence is labeled separately from a fresh run.

## Reproduce, triage and fix

[Explore the two evidence-backed cases](https://contextqaai.github.io/testing-lab/triage.html): a reproduced API status defect with an open fix PR, and a disclosed browser persistence regression with a verified baseline. [Walkthrough and verification limits](TRIAGE.md).

## Enterprise environments

[Enterprise access assessment](ENTERPRISE.md) · [Public enterprise guide](https://contextqaai.github.io/testing-lab/enterprise.html) · [Oracle APEX Customers source](https://github.com/contextqaai/testing-lab-oracle-apex/tree/26.2)

Oracle, SAP, Workday, ServiceNow, Pega and Infor are separated into installable samples and tenant-dependent qualification paths. Workday now advertises a personal developer-tenant beta. ServiceNow PDI and SAP basic-trial restrictions mean a commercial shared demo needs an appropriate approved environment. None of these vendor environments is claimed as live or tested.
