// Here is your easy win to get started: integrate the payment gateway in line 20.
// Make sure you do not add extra spaces for code validation purposes.
const nearAPI = require("near-api-js");
const { connect, utils } = nearAPI;
const { config } = require('./config'); // loads config settings

// configure accounts, network, and amount of NEAR to send
const sender = "sender.testnet";
const receiver = "receiver.testnet";
const networkId = "testnet";
const amount = utils.format.parseNearAmount("1.5");

async function main() {
  // connect to NEAR! :)
  const near = await connect(config);
  // create a NEAR account object
  const sender = await near.account(sender);

  // TODO send those tokens here
  const result = 
  console.log("Transaction Results: ", result.transaction);
}