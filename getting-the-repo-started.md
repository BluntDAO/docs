---
description: This is how to get the BluntDAO App started
---

# 👨💻 Getting the Repo Started

{% hint style="info" %}
**Good to know:** A quick start guide can be good to help folks get up and running with your API in a few steps. Some people prefer diving in with the basics rather than meticulously reading every page of documentation!
{% endhint %}

## Set Up Your Environment Variables

In order to run the BluntDAO app you need the following keys

* Web3 Auth
* Shard Dog Api Key
* Few n Far API
* Underdog Api Key
* Shopify Key

## Start the Repo

In order to start the repo use yarn

1.  Clone the repo from the url below.

    `git clone https://github.com/BluntDAO/bluntdao-app.git`
2.  Open a terminal in the root of the cloned repo and run yarn install to install all the required dependencies

    `yarn install`
3. Rename `.env-example` to `.env` and fill it with your own data variables.
4.  Run yarn start and all should pop up.

    `yarn start`

{% tabs %}
{% tab title="Yarn" %}
```
# Install via yarn
yarn install; yarn start;
```
{% endtab %}
{% endtabs %}

## Working With ShardDog Api

PUT TEXT HERE LETER

{% swagger baseUrl="https://api.myapi.com/v1" method="post" path="/pet" summary="Get request to shard dog API." %}
{% swagger-description %}
Creates a new pet.
{% endswagger-description %}

{% swagger-parameter in="body" name="name" required="true" type="string" %}
The name of the pet
{% endswagger-parameter %}

{% swagger-parameter in="body" name="owner_id" required="false" type="string" %}
The 

`id`

 of the user who owns the pet
{% endswagger-parameter %}

{% swagger-parameter in="body" name="species" required="false" type="string" %}
The species of the pet
{% endswagger-parameter %}

{% swagger-parameter in="body" name="breed" required="false" type="string" %}
The breed of the pet
{% endswagger-parameter %}

{% swagger-response status="200" description="Pet successfully created" %}
```javascript
{
    "name"="Wilson",
    "owner": {
        "id": "sha7891bikojbkreuy",
        "name": "Samuel Passet",
    "species": "Dog",}
    "breed": "Golden Retriever",
}
```
{% endswagger-response %}

{% swagger-response status="401" description="Permission denied" %}

{% endswagger-response %}
{% endswagger %}
