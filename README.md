# Apillon’s Bug Bounty

With the recent launch of the NCTR token, Apillon is launching its first incentivization-based program. With this bounty program, we are looking for experienced developers who want to collaborate with Apillon over a longer period and help us with testing, product feedback, bug hunting, and general improvements to our features. The program will utilize NCTR tokens as a reward vehicle for all participants.

## Security Issues

**Important:** This bug bounty is not meant for reporting issues concerning the security or integrity of the Apillon platform or toolkit.

For reports regarding security vulnerabilities and similar matters which must not be publicly exposed, please refer to our [security bug bounty](https://github.com/Apillon/apillon-services/blob/master/BUG_BOUNTY.md).

## Process overview

You don’t need to apply to the program; you can start testing immediately.

Here you’ll find the repo with the report template, so you can check beforehand what action to take and what to report.
1. **Register and start:** Sign up for the Apillon platform on https://app.apillon.io
2. **Create a new project**
3. **Visit your profile and connect the EVM compatible wallet, where you will receive the reward**
4. **Find your project UUID and copy it** - you will need to include the UUID in the bug bounty report, so we can match your report with your project. You can find the UUID in the "Settings" section of your project.
5. **Provide feedback:** Dive into the features, share your thoughts, write the report, include screenshots and submit it here on GitHub.
6. **Collect your bounty:** NCTR rewards for effort and dedication — straight to your wallet.

*By submitting the project UUID you agree that Apillon can reach out to your provided email and or process transactions to your target wallet*

## Which features are eligible and what should the testing involve?

The Bug Bounty Program is split into two parts. The first focuses on testing Apillon's **Web3** **services**, while the second (optional but eligible for bonus rewards) part invites feedback on **feature usability and overall user experience**.

What should your report include?

* Screenshots and detailed steps to reproduce any bugs or issues.
* Comments and suggestions for each feature.
* A link to GitHub repos with implementation code (if applicable).

### Testing Web3 services

##### Web3 Storage

* **Creating buckets:** Test the creation of multiple buckets via the dashboard, SDK, and CLI. Validate naming conventions and duplication restrictions.
* **Storing files:** Upload various file types (text, images, videos) and verify successful uploads and error handling for unsupported formats.
* **Receiving CID records:** Ensure proper generation of CID records for stored files and their retrievability from IPFS gateways.
* **Using IPNS:** Test IPNS record creation, linking it to a CID, and updating records. Verify persistence and access after updates.
* **Using buckets over SDK and CLI:** Perform all bucket operations via the CLI, including creating, listing, and deleting buckets. Confirm results against the dashboard.

#### Web3 Hosting

* **Creating a new website:** Deploy static websites via the dashboard and CLI. Verify successful build completion and error messaging for invalid file formats.
* **Publishing website to staging/production:** Test seamless deployment to both staging and production environments, ensuring version control.
* **Domain setup:** Test the integration of custom domains, including DNS propagation and SSL certificate generation.
* **GitHub Actions:** Set up a GitHub repository with automated deployment actions using Apillon's hosting. Verify push-triggered builds and deployments.

#### NFT Collections

* **NFT collection creation on various protocols:** Test creating NFT collections on multiple supported blockchains, verifying successful minting and transaction completion.
* **Metadata creation:** Create metadata files (JSON) with both manual and automated inputs. Verify proper linking to minted tokens.
* **CLI NFT collection creation and management:** Perform NFT collection creation, token minting, and token burning using the CLI. Confirm metadata integrity and transaction finalization.

#### Embedded Wallets

* **EW instance creation:** Test the creation of multiple wallet instances via the dashboard and SDK.
* **EW integration:** Integrate the embedded wallet SDK with a test dApp and verify the wallet’s visibility and functionality.
* **EW wallet generation:** Generate wallets for multiple users and test secure key storage and recovery mechanisms.
* **EW flow testing:** Perform transaction flows, including token transfers, signature requests, and error handling for invalid transactions.

#### Web3 Smart Contracts

* **Smart contract deployment:** Test deploying smart contracts from the dashboard, SDK, and CLI.
* **Contract interaction:** Execute contract functions, validate event emissions, and test interaction through different wallets.
* **Permission management:** Test the implementation of role-based access control on deployed contracts.
* **Multichain support:** Deploy and test smart contracts across multiple supported blockchains to ensure compatibility.

#### RPC Service

* **API key creation:** Test the creation of API keys through the platform, and add various networks to your list of favorites
* **Endpoint testing:** Verify the availability and responsiveness of RPC endpoints for different supported blockchains.
* **Method validation:** Test various RPC methods, ensuring correct responses and error handling for invalid requests.
* **Rate limiting:** Check the rate limits imposed on RPC calls and validate the system's behavior when limits are exceeded.

#### Indexing Service

* **Data indexing:** Test the indexing of blockchain data, ensuring accurate and timely updates.
* **Query performance:** Evaluate the performance of data queries, including response times and result accuracy.
* **API integration:** Integrate the indexing service API with a test application and verify the correctness of the returned data.
* **Error handling:** Test the system's ability to handle errors gracefully, including invalid queries and data retrieval issues.

### Testing feature usability and general UX

We would appreciate some clear, actionable feedback on main feature usability (documenting the whole flow and your experience), general UX vibe, clarity of the docs and feature integration complexity (documenting hard-to-understand steps, examples inputs, or points where people may get stuck), any potential limitations of these services, comparison to other similar services and/or any creative ideas for improvement.

## Rewards

Every user in the program can earn NCTR rewards, regardless of feature complexity. Once testers submit their deliverables, the Apillon team will review them. If they meet the minimum requirements, the tester will receive the set NCTR reward for that feature. If the requirements aren't met, we'll provide feedback, giving the tester a chance to revise and resubmit their report to qualify for the reward.

Each user in the beta program is eligible to receive NCTR rewards by the following criteria:

- **Grade A - 5,000 $NCTR:** Feature well tested, GitHub repo with integration code available (if applicable), report is extensive and covers most of the required criteria
- **Grade B - 1,000 $NCTR:** Report is short and lacking, report does not include any new findings or areas of improvemen
- **Grade C - 10 $NCTR:** A “thank you for trying” amount is reserved for users who do not execute any of the testing but still file the reports.

## Scope

- [Apillon Website](https://apillon.io/)
- [Apillon App](https://app.apillon.io/)
- [Apillon API](https://api.apillon.io/)
- [Apillon SDK](https://github.com/Apillon/sdk)
- [Apillon CLI](https://github.com/Apillon/sdk)

## Final thoughts

If you want to test Apillon’s features and provide valuable feedback, apply to the Bug Bounty Program. There is no formal selection process, but we aim to identify testers demonstrating potential for long-term collaboration with Apillon.