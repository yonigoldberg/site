---
title: Lambda Node.js 0.10 Update Instructions
author: Noah Zoschke
twitter: nzoschke
---

Is your inbox full of messages like this?

> AWS Lambda to end-of-life Node.js v0.10 runtime on April 30, 2017. Please migrate to Node.js v4.3 or v6.10 immediately

Well I'm happy to announce that the Convox fully-automated migration to Node.js v4.3 is available in every region.

Pieces of this have been released over the past weeks and months, so many of you don't need to take additional action.

But if you're still getting those emails from AWS, you can:

1. Perform a `convox rack update`. This will automatically update all your Rack Lambda functions.
2. Re-deploy your apps. This will automatically update all your app Lambda functions.
3. Re-create any syslog resources with `convox services create syslog` and delete old ones. This will update your logging Lambda functions.

You can expect to receive a couple more updates from both AWS and Convox between now and April 30th, to make sure nobody is affected when the Lambda runtime is shut off for good.

Happy automatic infrastructure updates! 🎉🎉
