# Email Authentication Example (with React & Apollo)

> **Attention**: This example uses the latest beta version of the CLI! Authentication is implemented using a `resolver` function instead of an authentication provider. For more information on the CLI Beta, read [the feedback thread in the forum](https://www.graph.cool/forum/t/feedback-new-cli-beta/949).

This is an authentication example based on the simple [Email & Password Authentication](https://github.com/graphcool/modules/tree/master/authentication/email-password) module.

## Getting Started

### 1. Clone the repository

```sh
git clone git@github.com:graphcool-examples/react-graphql.git
cd react-graphql/authentication-with-email-and-apollo/graphcool
```

### 2. Create your Graphcool project

```sh
# Install latest version of the Graphcool CLI
npm install -g graphcool@beta

# Create project
graphcool init
```

This will add a `.graphcoolrc` with a default `dev` environment to the project directory. This environment is backed by a new Graphcool project that was created in your Graphcool account.

The project's schema is created based on the type definitions in [`./types.graphql`](./types.graphql) and [`./graphcool/modules/email-password/types.graphql`](./graphcool/modules/email-password/types.graphql). The Graphcool CLI simply merges all `types.graphql`-files it finds in the project structure to generate the API.


#### 3. Connect the app with your GraphQL API

Copy the `Simple API` endpoint to `./src/index.js` as the `uri` argument in the `createNetworkInterface` call:

```js
const networkInterface = createNetworkInterface({ uri: '__SIMPLE_API_ENDPOINT__' })
```


### 4. Install dependencies & run locally

```sh
yarn install
yarn start 
```

You can now use the app at `http://localhost:3000`.


## Next steps

* [Advanced GraphQL features](https://www.graph.cool/docs/tutorials/advanced-features-eath7duf7d/)
* [Authentication & Permissions](https://www.graph.cool/docs/reference/authorization/overview-iegoo0heez/)
* [Implementing business logic with serverless functions](https://www.graph.cool/docs/reference/functions/overview-boo6uteemo/)


## Help & Community [![Slack Status](https://slack.graph.cool/badge.svg)](https://slack.graph.cool)

Say hello in our [Slack](http://slack.graph.cool/) or visit the [Graphcool Forum](https://www.graph.cool/forum) if you run into issues or have questions. We love talking to you!

![](http://i.imgur.com/5RHR6Ku.png)
