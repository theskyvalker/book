# Web3 Indexer with Apibara

This repository uses [Apibara](https://github.com/apibara/apibara) to index web3 data.

Run the Indexer
apibara run src/<indexer>.ts -A <dna-token>

To run the NFT metadata indexer you will need to be running the nextjs app hosting the API handler

## Customizing the template

You can change the id of the indexer by changing the value of the `indexer_id` variable in `src/indexer/indexer.py`. This id is also used as the name of the Mongo database where the indexer data is stored.

## Running in production

This template includes a `Dockerfile` that you can use to package the indexer for production usage.

## Running GraphQL Server

To start the graphql server, enter the venv and run:

    indexer graphql

The goerli graphiql will be available at `http://localhost:8080/goerli-graphql` and mainnet at `http://localhost:8080/graphql`
