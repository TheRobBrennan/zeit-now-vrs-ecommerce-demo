[![](https://assets.zeit.co/image/upload/v1556749417/front/blog/serverless-ecommerce/serverless-vrs.now.sh.png)](https://serverless-vrs.now.sh)

<div align="center">
<a href="https://zeit.co/blog/serverless-ecommerce">Read the blog post</a>
<span>&nbsp;&nbsp;&nbsp;&nbsp;</span>
<a href="https://serverless-vrs.now.sh">Checkout the demo</a>
</div>

---

VRS is a fully-functional e-commerce store, built on the [serverless paradigm](https://zeit.co/now).

With a single command `now`, the store deploys instantly, scales automatically, and requires zero supervision. The underlying infrastructure can handle peak time traffic with consistent, blazing-fast performance.

## Deploy

You can deploy VRS to our scalable serverless infrastructure free of cost.
Thanks to the on-demand pricing model, you don’t pay a cent for infrastructure during idle time.

Once you have [Now CLI](https://zeit.co/download) installed, clone this repo, specify the necessary secrets with Now CLI, and run `now` — that’s it. The [deployment section](https://zeit.co/blog/serverless-ecommerce#deploying-and-infrastructure) on our blog post explains how you can specify the secrets.


You will need to setup:

+ A new [GitHub app](https://github.com/settings/apps)
 - https://zeit-now-vrs-ecommerce-demo.therobbrennan.now.sh
 - https://zeit-now-vrs-ecommerce-demo.therobbrennan.now.sh/auth/github

Please copy the `.env.sample` file to `.env` and store your development secrets there.

To define the required secrets on ZEIT Now, please run the following:

```sh
$ now secret add vrs-github-client-id "YOUR_GITHUB_CLIENT_ID"

> Success! Secret vrs-github-client-id added (therobbrennan) [250ms]

$ now secret add vrs-github-client-secret "YOUR_GITHUB_CLIENT_SECRET"

> Success! Secret vrs-github-client-secret added (therobbrennan) [250ms]

$ now secret add vrs-mongodb-atlas-uri "YOUR_MONGODB_ATLAS_URI"

> Success! Secret vrs-mongodb-atlas-uri added (therobbrennan) [250ms]

$ now secret add vrs-stripe-secret "YOUR_STRIPE_SECRET_KEY"

> Success! Secret vrs-stripe-secret added (therobbrennan) [250ms]
```

## About

Our mission at ZEIT is to make the cloud accessible to everyone. We do that by creating products that improve developer experience, provisioning infrastructure that is globally available, and by teaching the developer community about serverless-related technology. We made VRS to showcase that it’s possible to create a fully functional, high-performance e-commerce store without requiring infrastructure know-how.

Follow us on [Twitter](https://twitter.com/zeithq).

<br/>
<br/>

[![](https://assets.zeit.co/image/upload/v1556749970/repositories/vrs/zeit.svg)](https://zeit.co)
