# Split your bills

In this scenario you will build a [Splitwise](https://www.splitwise.com/) clone using Restate.

Split your bills is an app that allows roommates to share their bills.
Users add bills to a bill list; then, at the end of the month, the app processes all the bills in a list, paying them by withdrawing money from the list's participants.

Some ideas to spice up your project:

* Rather than mocking the payment system, connect your app to Stripe webhooks, as shown [here](https://github.com/restatedev/examples/tree/main/patterns-use-cases/async-signals-payment/async-signals-payment-typescript).
* You could create a UI and use the [`restate-sdk-clients`](https://www.npmjs.com/package/@restatedev/restate-sdk-clients) to connect the UI to Restate services, as shown [here](https://github.com/restatedev/sdk-typescript/blob/main/packages/restate-sdk-examples/src/ingress.ts). There are some tools to easily create [UIs from json schema](https://ui-schema.bemit.codes/examples/List), perhaps you can bootstrap a nice yet simple UI starting from those.
* Before processing the bills at the end of the month, perhaps ask a confirmation to each user involved. Awakeables can be quite handy for that!
* What if a user can add an already paid expense?
* Add a chatbot/AI assistant. Restate can keep around the AI context for you.