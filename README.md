# cfn-modules: AWS Route53 hosted zone (public)

AWS Route53 hosted zone public accessible. For a hosted zone accessible inside VPC only look at the [route53-hosted-zone-private](https://www.npmjs.com/package/@cfn-modules/route53-hosted-zone-private) module.

## Install

> Install [Node.js and npm](https://nodejs.org/) first!

```
npm i @cfn-modules/route53-hosted-zone-public
```

## Usage

```
---
AWSTemplateFormatVersion: '2010-09-09'
Description: 'cfn-modules example'
Resources:
  Function:
    Type: 'AWS::CloudFormation::Stack'
    Properties:
      Parameters:
        Name: 'widdix.de' # required
      TemplateURL: './node_modules/@cfn-modules/route53-hosted-zone-public/module.yml'
```

## Parameters

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Description</th>
      <th>Default</th>
      <th>Required?</th>
      <th>Allowed values</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Name</td>
      <td>The name of the domain (hosted zone)</td>
      <td></td>
      <td>yes</td>
      <td></td>
    </tr>
  </tbody>
</table>
