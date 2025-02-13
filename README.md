# λ AWSome Lambda Layers

**A curated list of awesome AWS Lambda Layers**

## What are Lambda Layers?

> Lambda Layers are a new type of artifact that can contain arbitrary code and data, and may be referenced by zero, one, or more functions at the same time. Lambda functions in a serverless application typically share common dependencies such as SDKs, frameworks, and now runtimes. With layers, you can centrally manage common components across multiple functions enabling better code reuse.

— https://aws.amazon.com/about-aws/whats-new/2018/11/aws-lambda-now-supports-custom-runtimes-and-layers/

## How to create and use Lambda Layers?

* [with Serverless Framework](https://serverless.com/blog/publish-aws-lambda-layers-serverless-framework/)
* [with SAM](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-template.html#serverless-sam-template-layerversion)
* [with AWS Console](https://aws.amazon.com/blogs/aws/new-for-aws-lambda-use-any-programming-language-and-share-common-components/)
* [with AWS CLI](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html) ([tutorial](https://github.com/nsriram/aws-lambda-layer-example)),
* [with Stackery](https://www.stackery.io/blog/lambda-layers/)

## How to share Lambda Layers publicly?

* [Tutorial with CLI examples](https://medium.com/@zaccharles/f1413b974f44)

## Layers

### Runtimes

| Name | ARN / Link | Compatible Runtimes |
|------|------------|---------------------|
| C++ (official) | Link: [awslabs/aws-lambda-cpp](https://github.com/awslabs/aws-lambda-cpp) | `provided` |
| Rust (official) | Link: [awslabs/aws-lambda-rust-runtime](https://github.com/awslabs/aws-lambda-rust-runtime) | `provided` |
| Bash | ARN: `arn:aws:lambda:<region>:744348701589:layer:bash:<version>`<br>Link: [`gkrizek/bash-lambda-layer`](https://github.com/gkrizek/bash-lambda-layer) | `provided` |
| [Ballerina](https://ballerina.io/) | Link: [ballerina.io/deployment/aws-lambda](https://ballerina.io/deployment/aws-lambda/) | `provided` |
| [Crystal](https://crystal-lang.org/) | Link: [lambci/crambda](https://github.com/lambci/crambda) | `provided` |
| [Nim](https://nim-lang.org/) | Link: [lambci/awslambda.nim](https://github.com/lambci/awslambda.nim) | `provided` |
| Node.js v8 - N\|Solid | ARN: `arn:aws:lambda:<region>:800406105498:layer:nsolid-node-8:<version>`<br>Link: [accounts.nodesource.com/downloads/nsolid-lambda](https://accounts.nodesource.com/downloads/nsolid-lambda) | `provided` |
| Node.js v10 | ARN: `arn:aws:lambda:<region>:553035198032:layer:nodejs10:<version>`<br>Link: [`lambci/node-custom-lambda`](https://github.com/lambci/node-custom-lambda) | `provided` |
| Node.js v10 - N\|Solid | ARN: `arn:aws:lambda:<region>:800406105498:layer:nsolid-node-10:<version>`<br>Link: [accounts.nodesource.com/downloads/nsolid-lambda](https://accounts.nodesource.com/downloads/nsolid-lambda) | `provided` |
| Node.js v12 | ARN: `arn:aws:lambda:<region>:553035198032:layer:nodejs12:<version>`<br>Link: [`lambci/node-custom-lambda`](https://github.com/lambci/node-custom-lambda) | `provided` |
| PHP 7.1 | ARN: `arn:aws:lambda:<region>:887080169480:layer:php71:3`<br>Link:[`stackery/php-lambda-layer`](https://github.com/stackery/php-lambda-layer) | `provided` |
| PHP 7.2 & 7.3<br>cli & fpm | ARN: [`arn:aws:lambda:<region>:209497400698:layer:php-73:<version>`](https://runtimes.bref.sh/)<br>Link:[`brefphp/bref`](https://github.com/brefphp/bref) | `provided` |
| Pypy 3.5 | ARN: `arn:aws:lambda:<region>:146318645305:layer:pypy35:<version>`<br>Link: [IOpipe Pypy Layer](https://github.com/iopipe/lambda-runtime-pypy3.5) | `pypy3.5` |
| Brainfuck | ARN: `arn:aws:lambda:<region>:444134189787:layer:brainfuck:1`<br>Built for fun, will not process events! | `provided` |
| LOLCODE | ARN: `arn:aws:lambda:<region>:444134189787:layer:lolcode:1`<br>Built for fun, will not process events! | `provided` |
| Java 11 | Link: [andthearchitect/aws-lambda-java-runtime](https://github.com/andthearchitect/aws-lambda-java-runtime) | `provided` |
| Haskell | ARN: `arn:aws:lambda:<YOUR REGION>:785355572843:layer:aws-haskell-runtime:2` <br>Link: [Getting Started with the Haskell AWS Lambda Runtime](https://medium.com/the-theam-journey/getting-started-with-the-haskell-aws-lambda-runtime-951b2322c7a3) | `provided` |


### Utilities

| Name | ARN / Link | Compatible Runtimes |
|------|------------|---------------------|
| AWS CLI | Link: [`aws-samples/aws-lambda-layer-awscli`](https://github.com/aws-samples/aws-lambda-layer-awscli) | all |
| [better-sqlite3](https://github.com/JoshuaWise/better-sqlite3) | ARN: `arn:aws:lambda:us-east-1:284387765956:layer:BetterSqlite3:4`<br>Link: [`seanfisher/better-sqlite3-lambda-layer`](https://github.com/seanfisher/better-sqlite3-lambda-layer) | `nodejs8.10` |
| chrome-aws-lambda | ARN: `arn:aws:lambda:us-east-1:764866452798:layer:chrome-aws-lambda:4`<br>Link: [`shelfio/chrome-aws-lambda-layer`](https://github.com/shelfio/chrome-aws-lambda-layer) | all |
| ClamAV | Link: [`kindlyops/lambda-clamav-layer`](https://github.com/kindlyops/lambda-clamav-layer) | all |
| FFmpeg/FFprobe | ARN: `arn:aws:lambda:us-east-1:145266761615:layer:ffmpeg:4`<br>Link: [`serverlesspub/ffmpeg-aws-lambda-layer`](https://github.com/serverlesspub/ffmpeg-aws-lambda-layer) | all |
| GDAL + PDAL | Link: [`arn:aws:lambda:us-east-1:163178234892:layer:pdal:8`](https://github.com/PDAL/lambda) | all |
| GeoIP | Link: [`dschep/geoip-lambda-layer`](https://github.com/dschep/geoip-lambda-layer) | all |
| Ghostscript | ARN: `arn:aws:lambda:us-east-1:764866452798:layer:ghostscript:1`<br>Link: [`shelfio/ghostscript-lambda-layer`](https://github.com/shelfio/ghostscript-lambda-layer) | all |
| Git + SSH | ARN: `arn:aws:lambda:<region>:553035198032:layer:git:<version>`<br>Link: [`lambci/git-lambda-layer`](https://github.com/lambci/git-lambda-layer) | all |
| GraphicsMagick | ARN: `arn:aws:lambda:<region>:175033217214:layer:graphicsmagick:<version>`<br>Link: [`rpidanny/gm-lambda-layer`](https://github.com/rpidanny/gm-lambda-layer) | all |
| headless chromium with CJK fonts | Link: [`pahud/lambda-layer-headless-chromium`](https://github.com/pahud/lambda-layer-headless-chromium) | all |
| kubectl for Amazon EKS | Link: [`aws-samples/aws-lambda-layer-kubectl`](https://github.com/aws-samples/aws-lambda-layer-kubectl) | all |
| LibreOffice | ARN: `arn:aws:lambda:us-east-1:764866452798:layer:libreoffice:7`<br>Link: [`shelfio/libreoffice-lambda-layer`](https://github.com/shelfio/libreoffice-lambda-layer) | all |
| MySQL PHP 7.1 | Link: [`aiir/php71-mysql-aws-lambda-layer`](https://github.com/aiir/php71-mysql-aws-lambda-layer) | [`stackery/php-lambda-layer`](https://github.com/stackery/php-lambda-layer) |
| OR-Tools | Link: [`matheusmessora/or-tools-layer`](https://github.com/matheusmessora/or-tools-layer) | `python3.6` |
| Pandoc | ARN: `arn:aws:lambda:us-east-1:145266761615:layer:pandoc:1`<br>Link: [`serverlesspub/pandoc-aws-lambda-binary`](https://github.com/serverlesspub/pandoc-aws-lambda-binary) | all |
| PostgreSQL libpq | https://github.com/DrLuke/postgres-libpq-aws-lambda-layer | all |
| Puppeteer | ARN: `arn:aws:lambda:us-east-1:085108115628:layer:chrome:6`<br>Link: [`RafalWilinski/serverless-puppeteer-layers`](https://github.com/RafalWilinski/serverless-puppeteer-layers) | all |
| psycopg2  | Link: [`jetbridge/psycopg2-lambda-layer`](https://github.com/jetbridge/psycopg2-lambda-layer)  | `python3.6` `python3.7` |
| Python Toolkit | Link: [`keithrozario/Klayers`](https://github.com/keithrozario/Klayers)<br>Python packages incl. requests, aiohttp, pyOpenSSL etc.| `python3.7`|
| rsvg-convert | ARN: `arn:aws:lambda:us-east-1:145266761615:layer:rsvg-convert:2`<br>Link: [`serverlesspub/rsvg-convert-aws-lambda-binary`](https://github.com/serverlesspub/rsvg-convert-aws-lambda-binary) | all |
| SoX | ARN: `arn:aws:lambda:us-east-1:145266761615:layer:sox:1`<br>Link: [`serverlesspub/sox-aws-lambda-binary`](https://github.com/serverlesspub/sox-aws-lambda-binary) | all |
| SQLite Python | Link: [`dschep/sqlite-lambda-layer`](https://github.com/dschep/sqlite-lambda-layer) | `python3.6` |
| Tesseract | Link: [`bweigel/aws-lambda-tesseract-layer`](https://github.com/bweigel/aws-lambda-tesseract-layer) | all |



### Monitoring

| Name | ARN / Link | Compatible Runtimes |
|------|------------|---------------------|
| Datadog | ARN: `arn:aws:lambda:<region>:464622532012:layer:Datadog-Python37:1`<br>Link: [Datadog's Lambda Layer](https://www.datadoghq.com/blog/datadog-lambda-layer/) | `python2.7, python3.6, python3.7`, |
| Epsagon Node | ARN: `arn:aws:lambda:<region>:066549572091:layer:epsagon-node-layer:1`<br>Link: [Epsagon Node Layer](https://epsagon.com/blog/bring-your-epsagon-layer-to-aws-lambda/) | `nodejs6.10, nodejs8.10` |
| Epsagon Python | ARN: `arn:aws:lambda:<region>:066549572091:layer:epsagon-python-layer:1`<br>Link: [Epsagon Python Layer](https://epsagon.com/blog/bring-your-epsagon-layer-to-aws-lambda/) | `python2.7, python3.6, python3.7` |
| IOpipe Node | ARN: `arn:aws:lambda:<region>:146318645305:layer:IOpipeNodeJS810:<version>`<br>Link: [IOpipe Node Layer](https://github.com/iopipe/iopipe-js/releases) | `nodejs6.10, nodejs8.10` |
| IOpipe Python | ARN: `arn:aws:lambda:<region>:146318645305:layer:IOpipePython:<version>`<br>Link: [IOpipe Python Layer](https://github.com/iopipe/iopipe-python/releases) | `python2.7, python3.6, python3.7` |
| IOpipe Java | ARN: `arn:aws:lambda:<region>:146318645305:layer:IOpipeJava8:<version>`<br>Link: [IOpipe Java Layer](https://github.com/iopipe/iopipe-java/releases) | `java8` |
| Lumigo Node | ARN: `arn:aws:lambda:YOUR-REGION:724777057400:layer:lumigo-node-tracer:<version>`<br>Link: [Lumigo Node Layer](https://github.com/lumigo-io/lumigo-node) | `nodejs8.10, nodejs10.X` |
| Lumigo Python | ARN: `arn:aws:lambda:YOUR-REGION:724777057400:layer:lumigo-python-tracer:<version>`<br>Link: [Lumigo Python Layer](https://github.com/lumigo-io/python_tracer) | `python3.6, python3.7` |
| Thundra Java | ARN: `arn:aws:lambda:<region>:269863060030:layer:thundra-lambda-java-layer:1`<br>Link: [Thundra Java Layer](https://docs.thundra.io/docs/java-custom-runtime-and-layer-support) | `java8` |
| Thundra Node | ARN: `arn:aws:lambda:<region>:269863060030:layer:thundra-lambda-node-layer:1`<br>Link: [Thundra Node Layer](https://docs.thundra.io/docs/node-custom-runtime-and-layer-support) | `nodejs8.10` |


### Security
| Name | ARN / Link | Compatible Runtimes |
|------|------------|---------------------|
| [Protego](https://protego.io/) | Link: [Protego Layers and Runtimes](https://www.protego.io/layers-and-runtimes-protego/) | `python2.7, python3.6, python3.7, nodejs6.10, nodejs8.10, java8, dotnetcore2.0, dotnetcore2.1` |
| [PureSec](https://www.puresec.io/) | Link: [PureSec Lambda Protection Layer](https://www.puresec.io/blog/aws-lambda-security-with-zero-overhead-by-puresec) | `nodejs8.10, nodejs6.10, python2.7, python3.6, python3.7, java8, dotnetcore2.x`|
