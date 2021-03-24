# AWS JS S3 Explorer

The original view-only [S3 Explorer](https://github.com/awslabs/aws-js-s3-explorer).
The [fork we forked](https://github.com/ninovanhooff/aws-js-s3-explorer) 

AWS JavaScript S3 Explorer (v2 alpha) is a JavaScript application that uses AWS's JavaScript SDK and S3 APIs to make the contents of an S3 bucket easy to browse via a web browser. We've created this to enable easier sharing and management of objects and data in Amazon S3.

[main-public]: https://raw.githubusercontent.com/awslabs/aws-js-s3-explorer/v2-alpha/screenshots/explorer-main-public.png


## Install

- No install required, all libs are used in cdn inside `index.html`

## Start it locally

- `cd aws-js-s3-explorer`
- `npx http-server . 8081`
- access it at [localhost:8081](localhost:8081)

## Link to it in front locally

- `cd pb2-front`
- edit `src/pages/Agent/index.tsx`
- set `const url = localhost:8081/?settings=${btoa(JSON.stringify(s3BrowserSettings))}`
- Start/Restart front

## Test in in stagging

- First open a PR pointing to the `prod` branch ☢️ It will automatically point to the original fork repository, first change to phantombuster then point to prod branch 🙏 ☢️
- After a while a netlify link will appear inside the PR check details, just click on `details` button to open the stagging test & copy the url
- `cd pb2-front`
- edit `src/pages/Agent/index.tsx`
- set `const url = ${url-to-generated-netlify-s3}:8081/?settings=${btoa(JSON.stringify(s3BrowserSettings))}`
- Start/Restart front

## Helpers/Docs

AWS config object doc could [be found here](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/Config.html)
