# ContextQA Testing Lab

Real source. Explicit assertions. Reproducible failures.

Learn to test an application end to end, inspect the evidence, introduce a regression and repeat the workflow on an application you own.

| Track | Public source | Exercises | Hosted app status |
|---|---|---|---|
| React payments | [React/Express sample](https://github.com/contextqaai/testing-lab-react-payments) | [Five exercises](https://github.com/contextqaai/testing-lab-react-payments/blob/develop/lab/README.md) | Local setup available; public hosting pending |
| Angular Conduit | [Angular workflow sample](https://github.com/contextqaai/testing-lab-angular-conduit) | [Five exercises](https://github.com/contextqaai/testing-lab-angular-conduit/blob/main/lab/README.md) | Local setup available; owned backend/public hosting pending |
| Java PetClinic | [Spring business forms sample](https://github.com/contextqaai/testing-lab-java-petclinic) | [Five exercises](https://github.com/contextqaai/testing-lab-java-petclinic/blob/main/lab/README.md) | Local setup available; isolated public hosting pending |
| HTML/JavaScript | [Vanilla TodoMVC starter](https://github.com/contextqaai/testing-lab-html-todomvc) | [Five exercises](https://github.com/contextqaai/testing-lab-html-todomvc/blob/master/lab/README.md) | Static package in docs; see deployment status before using its URL |

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
