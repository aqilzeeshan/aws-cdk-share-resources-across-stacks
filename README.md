# How to share resources across stacks in AWS CDK

A repository for an article on: https://dannys.cloud/share-resources-across-stacks-aws-cdk

## How to Use this repository

1. Clone the repository

2. Install the dependencies

```bash
npm install
```

3. Synthesize the stacks

```bash
cdk synth
```

4. Deploy the stacks in the following order

```bash
cdk deploy SharedInfraStack

cdk deploy RdsStack
```

5. Open the AWS CloudFormation Console and the stack should be created in your
   default region

6. Cleanup - Delete the stacks in the following order

```bash
cdk destroy SharedInfraStack

cdk destroy RdsStack
```

---

## Author

**[Danny Steenman](https://dannys.cloud)**

<p align="left">
  <a href="https://dannys.cloud/twitter"><img src="https://img.shields.io/twitter/follow/dannysteenman?label=%40dannysteenman&style=social"></a>
</p>
