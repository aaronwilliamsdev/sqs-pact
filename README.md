# sqs-pact

## Purpose of Repo

Simple example of using pact contract testing with SQS.

## Installing

To install the dependencies run `npm i`

## Setup

Ensure you have terraform and AWS cli setup.

You can create a new SQS queue running:
`terraform init`
`terraform verify`
`terraform apply`

Then set the queue URL in this project.

Be sure you have set your pact broker URL and token in the files.

Do a global search on the project for `{YOUR_` to find all the values to replace.

## Running

`provide:consume` - run the script to publish a new message and consume it

`pact:consumer ` - run the pact consumer test

`pact:publish` - publish the pact to the broker

`pact:provider` - run the pact provider test to varify the pact
