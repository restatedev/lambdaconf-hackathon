# Cron service

In this scenario you will build a [Fastcron](https://www.fastcron.com/) clone using Restate.

Cron service lets people schedule HTTP calls using the [cron format](https://en.wikipedia.org/wiki/Cron).
Users can configure different aspects of the call, such as path, headers, body.

Some ideas to spice up your project:

* You could check the response status code and, in case of failure, let the user provide a retry policy to retry the HTTP request.
* Why stop to only one HTTP request after the cron? Why even stop to HTTP?
* How about sending a notification back, e.g. via email, on every successful run?
* You could create a UI and use the [`restate-sdk-clients`](https://www.npmjs.com/package/@restatedev/restate-sdk-clients) to connect the UI to Restate services, as shown [here](https://github.com/restatedev/sdk-typescript/blob/main/packages/restate-sdk-examples/src/ingress.ts). There are some tools to easily create [UIs from json schema](https://ui-schema.bemit.codes/examples/List), perhaps you can bootstrap a nice yet simple UI starting from those.
* If you group cron jobs by type, you could aggregate their results to build a "status page"