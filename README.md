# Azure WAF Manager ARM templates
This repo contains ARM templates for Azure WAF policies, Azure Front Door, custom roles and Azure Lighthouse. They can be used to operate in Azure WAF Manager or independently.

## Onboard Customer Resource Group (Azure Lighthouse)
This template will give us Log Analytics Reader access to your Log Analytics workspaces in the Resrouce Group you provide.

[![Azure Lighthouse Resource Group](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fawm-azure-lighthouse-resourcegroup.json)

[![Visualize](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.svg?sanitize=true)](http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fawm-azure-lighthouse-resourcegroup.json)

or copy link

```jsx
https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fawm-azure-lighthouse-resourcegroup.json
```
<sub>This is mandatory step if you use our service. This allows us to query your workspace for WAF logs. You either provide us CSP access to a resource group or an entire subscription</sub>

## Azure Lighthouse Subscription

This template will provide us with LogAnalytics Reader role over the subscription in quesiton

[![Azure Lighthouse Subscription](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fawm-azure-lighthouse-subscription.json)

[![Visualize](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.svg?sanitize=true)](http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fawm-azure-lighthouse-subscription.json)

or copy link

```jsx
https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fawm-azure-lighthouse-subscription.json
```
<sub>This is mandatory step if you use our service. This allows us to query your workspace for WAF logs. You either provide us CSP access to a resource group or an entire subscription</sub>

## WAF Editor Custom rule
This template will deploy a custom RBAC role called **WAF Policies Editor** which can only edit and not even delete WAF policies. This is a good role to assign to the **Service Princial** that you register in our portal

[![Azure Lighthouse Subscription](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fwaf-editor-custom-rbac-role.json)

[![Visualize](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.svg?sanitize=true)](http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fwaf-editor-custom-rbac-role.json)

or copy link

```jsx
https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fwaf-editor-custom-rbac-role.json
```
<sub>This is NOT a mandatory step to use our service. This is just a free template we provide you, so you can very specifically provision a custom role that can only edit WAF policies and nothing else</sub>

## Deploy Classic Front Door WAF Policy
This template will quickly deploy a Classic Front Door WAF Policy for you with some good practice custom rules and a beautiful custom block page.

[![Azure Lighthouse Subscription](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fclassic-front-door-wafpolicy.json)

[![Visualize](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.svg?sanitize=true)](http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fclassic-front-door-wafpolicy.json)

or copy link

```jsx
https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fclassic-front-door-wafpolicy.json
```
<sub>This is NOT a mandatory step to use our service. This is just a free arm template we provide you, so you can quickly deploy a WAF Policy</sub>

## Deploy Premium Front Door WAF Policy
This template will quickly deploy a Premium Front Door WAF Policy for you with some good practice custom rules and a beautiful custom block page.

[![Azure Lighthouse Subscription](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fpremium-front-door-wafpolicy.json)

[![Visualize](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.svg?sanitize=true)](http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fpremium-front-door-wafpolicy.json)

or copy link

```jsx
https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fpremium-front-door-wafpolicy.json
```
<sub>This is NOT a mandatory step to use our service. This is just a free arm template we provide you, so you can quickly deploy a WAF Policy</sub>

## Deploy Application Gateway WAF Policy
This template will quickly deploy a Application Gateway WAF Policy for you with some good practice custom rules and a beautiful custom block page.

[![Azure Lighthouse Subscription](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fapp-gateway-wafpolicy.json)

[![Visualize](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.svg?sanitize=true)](http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fapp-gateway-wafpolicy.json)

or copy link

```jsx
https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Fapp-gateway-wafpolicy.json
```
<sub>This is NOT a mandatory step to use our service. This is just a free arm template we provide you, so you can quickly deploy a WAF Policy</sub>

## Deploy Classic Front Door + WAF Policy
This template will quickly deploy a whole Classic Front Door instance with a new WAF Policy with some best practices already set up for you like best practices security headers and custom rules on the WAF policy.

[![Azure Lighthouse Subscription](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Ffront-door-and-classic-wafpolicy.json)

[![Visualize](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.svg?sanitize=true)](http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Ffront-door-and-classic-wafpolicy.json)

or copy link

```jsx
https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Ffront-door-and-classic-wafpolicy.json
```
<sub>This is NOT a mandatory step to use our service. This is just a free arm template we provide you, so you can quickly deploy a Classic Front Door + WAF Policy. This template also requires Log Analytics workspace</sub>

## Deploy Premium Front Door + WAF Policy
This template will quickly deploy a whole Premium Front Door instance with a new WAF Policy with some best practices already set up for you like best practices security headers and custom rules on the WAF policy.

[![Azure Lighthouse Subscription](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Ffront-door-premium-and-premium-wafpolicy.json)

[![Visualize](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.svg?sanitize=true)](http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Ffront-door-premium-and-premium-wafpolicy.json)

or copy link

```jsx
https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSunwell-Solutions-LTD%2Fazure-waf-manager-arm-templates%2Fmain%2Ffront-door-premium-and-premium-wafpolicy.json
```
<sub>This is NOT a mandatory step to use our service. This is just a free arm template we provide you, so you can quickly deploy a Premium Front Door + WAF Policy</sub>
