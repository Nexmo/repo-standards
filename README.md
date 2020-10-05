# Nexmo Repository Standards

<img src="https://developer.nexmo.com/assets/images/Vonage_Nexmo.svg" height="48px" alt="Nexmo is now known as Vonage" />

_These are our internal-facing guidelines, published in the open in case anyone else finds them useful._

This project contains checklists, templates and other resources to include with your open source repository. Whether you're starting a new project or improving an existing one, please include any or all of the elements suggested below as appropriate to your repo.

## Which GitHub Org?

Historically, we have had a number of GitHub orgs:

- `nexmo` Our libraries, code snippet repos and other formally supported projects go here.
- `nexmo-community` The community repo where we put sample apps, blog post examples, and other assorted items (things can be promoted into the main repo at a later date if widely adopted).
- `opentok` This is where our libraries, server SDKs and officially supported repos live. You can filter out "labs" projects using the "opentok-labs" topic.
- `opentok-community` The community repo where we put OpenTok related sample apps, blog post examples, and other assorted items (things can be promoted into the main repo at a later date if widely adopted).

If you're not sure where something goes, or you don't have permission to create a repo, talk to us in `#ask-devrel` on slack.

## Get the Basics Right

Naming things is hard, this part is very important! Best practice: name the project after what it does rather than what it is made of. E.g. "joke telephone answering service" rather than "sinatra voice demo".

- [ ] Give your repo **a description** and **some topics** - you can set these at the very top of the web interface, before the file listings. The description should cover the purpose and scope of the project. The tags should include `vonage` as well as the technologies used and the features of the project. For example you could have tags: `vonage` `python` `redis` `verify` `2fa`.

- [ ] Every repo must have a **license**, this will be [MIT](https://opensource.org/licenses/MIT) in most cases. See also: [GitHub docs for adding a license to your repo](https://help.github.com/en/articles/adding-a-license-to-a-repository) and always choose a standard OSI-approved license.

- [ ] Use the [basic README template](basic-readme-template.md) as a starting point for your repository. Look at the [project types](#what-type-of-project) section for what else to include for your project.

### What Type of Project?

While most of our `READMEs` should have some common features, different repo types have different requirements. Here is what we expect from the different types of repo.

| Library (e.g Node.js lib)                                        | Demo/Tool (e.g. Demo for booth/customer use)                    | Supporting code (e.g. for blog post)          |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------- |
| [Installation instructions](write-installation-instructions.md) | [Installation instructions](write-installation-instructions.md) | Link to what this repo is supporting          |
| Detailed [usage docs](write-usage-docs.md) for all features     | [Usage examples](write-usage-docs.md)                           | App may [set `User-Agent`](set-user-agent.md) |
| A [CONTRIBUTING](contributing-template.md) FILE                 | A [CONTRIBUTING](contributing-template.md) FILE                 |
| A [CODE_OF_CONDUCT](code-of-conduct-template.md) FILE           | A [CODE_OF_CONDUCT](code-of-conduct-template.md) FILE           |
| App **must** [set `User-Agent`](set-user-agent.md)              | App _may_ [set `User-Agent`](set-user-agent.md)                 |
| &nbsp;                                                          | Docker setup                                                    |
| &nbsp;                                                          | [One-click deployment setup](one-click-deploy.md)               |

## More README Resources

You may find these resources useful for structuring your project's README file (edit and add your favourites!)

- [Art of Readme](https://github.com/noffle/art-of-readme)
- [A template to make good README.md](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
- [Developer Experience: GitHub READMEs](https://betta.io/blog/2017/02/07/developer-experience-github-readmes)
- [Make a README](https://www.makeareadme.com/)
